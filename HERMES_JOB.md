# PASTE INTO HERMES

GOAL: Win a paid place on make.fun `tiny-chess-01` by shipping a ≤4096-byte Python chess engine in this public repo that beats the sunfish 4 KB baseline on practice grading.

SCOPE:
- In: this repo only (`C:\Powercore-repo-main\makefun-tiny-chess-01`)
- In: download + unpack kit from `https://make.fun/c/tiny-chess-01/kit`
- In: implement UCI bot that talks to `MAKEFUN_ENV_URL` per kit docs
- Hard out: do not invent session transcripts; do not commit API keys / `.env` / wallets
- Hard out: do not submit the entry yourself unless operator says SUBMIT

INVARIANTS:
- Public repo: `https://github.com/ianmxaof/makefun-tiny-chess-01`
- Entry must include `LICENSE` (MIT already present) and the bot entrypoint the kit expects (`main.py` unless kit says otherwise)
- Source ≤ 4096 bytes of Python (measure after minify; keep a readable draft + a size-gated ship file if needed)
- Hermes sessions must stay on disk (native logs) — `handed_over_places=none` so handed-over JSON wins no cash
- Never put `MAKEFUN_API_KEY` / `af_*` in git

PRIMARY MOVE: Read the unpacked kit README + `kit.json`, implement the strongest legal ≤4KB engine, push one commit to `main`, then run local grade from the kit (`node cli/makefun.mjs grade-local --kit . --bot <repo> --driver docker` if Docker works; else report blocker).

FALSIFIABLE GATES:
1. `git remote -v` shows `ianmxaof/makefun-tiny-chess-01`
2. Kit unpacked under `.kit/` (gitignored) with matching sha256 from competition page
3. Bot file(s) present; Python byte size ≤ 4096 for the shipped engine module(s) the kit counts
4. `git push origin main` succeeds; print full 40-char `commit_sha`
5. Local grade produces a practice Elo (or a clear Docker/node error paste)

OUTPUT ≤12 lines:
- commit_sha
- engine path + byte size
- practice Elo or exact grade error
- next need: BUNDLE | SUBMIT | BLOCKED:<reason>

ANTI-DRIFT:
- Do not switch bounty slug
- Do not rewrite LICENSE to non-OSS
- Do not open other make.fun contests in this job
- Stop after one strong push + grade attempt; ask before submit
