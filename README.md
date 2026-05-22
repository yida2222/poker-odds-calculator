# Poker Odds Calculator · 德州扑克胜率计算器

A single-file Texas Hold'em equity calculator. Pick your hole cards and the
board, and it estimates your win probability via Monte Carlo simulation,
shows your current made hand, and uses pot odds to tell you whether a call is
profitable. Bilingual (English / 中文), no dependencies, runs entirely in the browser.

一个单文件的德州扑克胜率计算器：选好手牌和公共牌，通过蒙特卡洛模拟估算你的
胜率，显示当前牌型，并用底池赔率判断这一注该不该跟。中英双语、零依赖、纯前端。

**▶ Live demo:** https://yida2222.github.io/poker-odds-calculator/

---

## Features · 功能

- **Win equity** — Monte Carlo simulation (~25,000 random deals) against
  1–8 random opponents. 蒙特卡洛模拟胜率，可设 1–8 个对手。
- **Made hand** — shows your current best hand in real time.
  实时显示你当前已成的牌型。
- **Pot odds** — enter pot and call amounts to see whether the call is +EV.
  输入底池与跟注金额，判断该跟还是该弃。
- **Bilingual** — one-click English / 中文 toggle. 一键中英切换。
- **Beginner guide** — built-in hand rankings and how-to-play. 内置牌型与玩法介绍。

## How it works · 原理

Exact equity requires enumerating a huge number of card combinations, so this
tool uses **Monte Carlo simulation**: it deals the remaining cards at random
many times and counts how often you win. A hand evaluator finds the best
5-card hand out of each 7-card combination. Accuracy is validated against
known benchmarks (e.g. AA vs KK preflop ≈ 82%).

精确胜率需要枚举海量牌组，因此本工具采用**蒙特卡洛模拟**：随机发剩余的牌很多次，
统计你赢的比例。牌力评估器会从 7 张牌中找出最好的 5 张牌型比大小。胜率已用公认
基准验证（如 AA vs KK 翻前约 82%）。

## Usage · 使用

Open `index.html` in any browser — that's it. No build step, no install.
直接用浏览器打开 `index.html` 即可，无需构建或安装。

## Disclaimer · 声明

For education and entertainment only. Not gambling advice. Estimates carry
~±1% statistical error and assume opponents hold uniformly random hands.
仅供学习与娱乐，非赌博建议。结果有约 ±1% 统计误差，且假设对手手牌均匀随机。
