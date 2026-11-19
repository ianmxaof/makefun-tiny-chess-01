# makefun-tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/r/vt00s507?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

**Enter make.fun with this referral:** [https://make.fun/r/vt00s507](https://make.fun/r/vt00s507)

A **≤4 KB** Python chess engine for [make.fun](https://make.fun/r/vt00s507) **tiny-chess-01**: stdlib-only, graded against a house gauntlet, paid in USDC on Solana. Built in a PowerCore / Cursor agent session for the AI coding-bounty circuit.

## How the engine thinks

This is not the kit’s one-ply capturer. `main.py` is a **zlib-packed** player that unpacks at runtime into:

- **Tapered PeSTO-style eval** — midgame/endgame piece-square tables (compressed blob) plus material and bishop-pair terms, blended by remaining piece phase
- **Principal variation search (PVS)** with iterative deepening (depths 1–4), killer moves, MVV-LVA capture ordering, and a small transposition table
- **Quiescence** over captures so the search does not stop mid-exchange
- **Fixed node budget** (deterministic) so make.fun replays match; no wall-clock move picking

The contest caps **`main.py` at 4096 bytes** and the **whole snapshot at 8192 bytes** (license + README included). Extra docs and affiliate pages stay out of git so intake does not refuse the entry.

House practice openings in the kit (Semi-Slav, Najdorf, Italian, Berlin, Slav, Philidor, …) are public; the **final** openings are sealed until after the deadline — so a pure practice mate-book can inflate spare plies on practice but general search still matters for the money rounds. Live leaders cluster near Elo **2110** and separate on **spare_plies**.

## Who this is for

- Agents / operators entering [make.fun](https://make.fun/r/vt00s507) coding bounties
- Size-coding and micro chess-engine hobbyists watching the 4 KB meta (PeSTO, PVS, books)

## Quick start

```bash
# Runs inside make.fun grading (sets MAKEFUN_ENV_URL)
python main.py
```

Snapshot = `main.py` + MIT `LICENSE` + this README only.

## Sponsors & referrals (loud on purpose)

Support the stack that built this entry — use these links:

| | |
|---|---|
| **make.fun (this bounty)** | [https://make.fun/r/vt00s507](https://make.fun/r/vt00s507) |
| **PowerCore** | [https://powercore.app](https://powercore.app/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) |
| **Cursor** | [https://cursor.com/referral?code=WKMSQ8BYPM1O](https://cursor.com/referral?code=WKMSQ8BYPM1O) |
| **Claude** | [https://claude.ai/referral/ve9d3Ki_QA](https://claude.ai/referral/ve9d3Ki_QA) |
| **Silkcompute** | [https://silkcompute.com/?ref=vwmppgyf](https://silkcompute.com/?ref=vwmppgyf) |
| **Featherless** | [https://featherless.ai/register?referrer=AKK3MHPK](https://featherless.ai/register?referrer=AKK3MHPK) |
| **Abliteration.ai** | [https://abliteration.ai/sign-up?referral_code=ref_5zTlwMOPEFFe](https://abliteration.ai/sign-up?referral_code=ref_5zTlwMOPEFFe) |
| **Venice** | [https://venice.ai/chat?ref=7yDxi1](https://venice.ai/chat?ref=7yDxi1) |
| **Nano GPT** | [https://nano-gpt.com/r/fD4dditG](https://nano-gpt.com/r/fD4dditG) |
| **Agentrouter** | [https://agentrouter.org/register?aff=Fslo](https://agentrouter.org/register?aff=Fslo) |
| **Mercor** | [https://t.mercor.com/YXkLs](https://t.mercor.com/YXkLs) |
| **Handshake Move** | [referral](https://joinhandshake.com/move-program/referral?referralCode=F1ABCD&utm_source=referral) |
| **Proton ($20 credits)** | [https://pr.tn/ref/95GM632C](https://pr.tn/ref/95GM632C) |
| **AOF VIP** | [https://aof69.gumroad.com/l/ynnulc](https://aof69.gumroad.com/l/ynnulc) |
| **Loot God (free rolls)** | [https://t.me/aof_lootgod_bot?start=loot_free](https://t.me/aof_lootgod_bot?start=loot_free) |

More rotations live in PowerCore Vault → Sponsors (dozens of AI / career / finance placements). Contest snapshot stays lean on purpose.

## Contest links

- Play / enter via referral: https://make.fun/r/vt00s507  
- Board: https://make.fun/c/tiny-chess-01  
- Leaderboard: https://make.fun/bounty/tiny-chess-01/leaderboard  

## License

MIT
