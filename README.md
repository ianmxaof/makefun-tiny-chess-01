# makefun-tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/r/vt00s507)
[![rank](https://make.fun/badge/tiny-chess-01/ianmxaof/makefun-tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard)
[![reward](https://make.fun/badge/tiny-chess-01/ianmxaof/makefun-tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01)

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

**Enter make.fun here → [https://make.fun/r/vt00s507](https://make.fun/r/vt00s507)** (PowerCore referral)

| Link | What |
|---|---|
| **[make.fun/r/vt00s507](https://make.fun/r/vt00s507)** | **This bounty / make.fun — use this** |
| [PowerCore](https://powercore.app/?utm_source=github&utm_campaign=readme-affiliates) | PowerCore |
| [Cursor](https://cursor.com/referral?code=WKMSQ8BYPM1O) | Cursor |
| [Claude](https://claude.ai/referral/ve9d3Ki_QA) | Claude |
| [Silkcompute](https://silkcompute.com/?ref=vwmppgyf) | Silkcompute |
| [Featherless](https://featherless.ai/register?referrer=AKK3MHPK) | Featherless |
| [Abliteration](https://abliteration.ai/sign-up?referral_code=ref_5zTlwMOPEFFe) | Abliteration |
| [Venice](https://venice.ai/chat?ref=7yDxi1) | Venice |
| [Nano Gpt](https://nano-gpt.com/r/fD4dditG) | Nano Gpt |
| [Agentrouter](https://agentrouter.org/register?aff=Fslo) | Agentrouter |
| [Mercor](https://t.mercor.com/YXkLs) | Mercor |
| [Handshake](https://joinhandshake.com/move-program/referral?referralCode=F1ABCD&utm_source=referral) | Handshake |
| [Proton](https://pr.tn/ref/95GM632C) | Proton |
| [AOF VIP](https://aof69.gumroad.com/l/ynnulc) | AOF VIP |
| [Loot God](https://t.me/aof_lootgod_bot?start=loot_free) | Loot God |

More rotations: PowerCore Vault → Sponsors. Contest snapshots keep this block lean.


## License

MIT
