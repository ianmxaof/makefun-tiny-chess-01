# makefun-tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/r/vt00s507)

**Enter make.fun here → [https://make.fun/r/vt00s507](https://make.fun/r/vt00s507)** (PowerCore referral)

≤4 KB Python engine for **tiny-chess-01**: stdlib only, house gauntlet, USDC on Solana. Built in a PowerCore / Cursor agent session.

## How it plays

Not the kit’s one-ply capturer. Packed `main.py` unpacks to:

- **Tapered PeSTO-style eval** (compressed MG/EG PST + material + bishop pair, phase-blended)
- **PVS** with iterative deepening (1–4), killers, MVV-LVA, small TT
- **Quiescence** on captures; **fixed node budget** (deterministic for make.fun replay)

Contest caps: `main.py` ≤4096 B; whole snapshot ≤8192 B. Leaders sit near Elo **2110** and split on **spare_plies**. Practice openings are public in the kit; final openings are sealed — general search still pays.

## Who / run

Agents and size-coders on [make.fun](https://make.fun/r/vt00s507). Graded only with `MAKEFUN_ENV_URL`:

```bash
python main.py
```

## Sponsors & referrals

| Link | What |
|---|---|
| **[make.fun/r/vt00s507](https://make.fun/r/vt00s507)** | **This bounty — use this** |
| [powercore.app](https://powercore.app/?utm_source=github&utm_campaign=tiny-chess) | PowerCore |
| [Cursor](https://cursor.com/referral?code=WKMSQ8BYPM1O) | Editor that built this |
| [Claude](https://claude.ai/referral/ve9d3Ki_QA) | Claude referral |
| [Silkcompute](https://silkcompute.com/?ref=vwmppgyf) | Inference |
| [Featherless](https://featherless.ai/register?referrer=AKK3MHPK) | Open-weight API |
| [Abliteration.ai](https://abliteration.ai/sign-up?referral_code=ref_5zTlwMOPEFFe) | Uncensored weights |
| [Venice](https://venice.ai/chat?ref=7yDxi1) · [Nano GPT](https://nano-gpt.com/r/fD4dditG) · [Agentrouter](https://agentrouter.org/register?aff=Fslo) | More AI |
| [Mercor](https://t.mercor.com/YXkLs) · [Handshake](https://joinhandshake.com/move-program/referral?referralCode=F1ABCD&utm_source=referral) | AI work |
| [Proton](https://pr.tn/ref/95GM632C) · [AOF VIP](https://aof69.gumroad.com/l/ynnulc) · [Loot God](https://t.me/aof_lootgod_bot?start=loot_free) | Tools / AOF |

Dozens more rotate in PowerCore Vault → Sponsors (kept out of this snapshot for the byte cap).

Board: [contest](https://make.fun/c/tiny-chess-01) · [leaderboard](https://make.fun/bounty/tiny-chess-01/leaderboard) · **ref [vt00s507](https://make.fun/r/vt00s507)**

## License

MIT
