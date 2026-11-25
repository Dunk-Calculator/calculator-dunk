# Dunk Calculator

Open-source, dependency-free HTML/JS calculator for figuring out the vertical jump needed to dunk a basketball — standard mode and reverse ("can I dunk?") mode, imperial and metric.

Built and maintained by [calculator-dunk.com](https://calculator-dunk.com) — a live, maintained version of this same calculator (plus a dunk-improvement simulator) runs there.

## What it does

- **Standard mode** — enter height, standing reach, rim height and dunk style to get the required vertical jump
- **Reverse mode** — enter your current vertical to check whether you can already dunk
- **Imperial & metric** — switch units instantly, all values convert automatically
- **6 dunk styles** — touch rim, basic, power, windmill, 360°, between-the-legs, each with its own rim clearance
- **Jump physics** — estimated hang time and takeoff velocity, assumptions shown

## Formula

```
Required vertical = (Rim height + Dunk clearance) − Standing reach
```

Hang time and takeoff velocity use the standard vertical-projectile equations:

- takeoff velocity: `v = √(2gh)`
- hang time: `t = √(8h/g)`

## Structure

```
index.html              — the calculator (open directly in a browser)
calculators/
  dunk-calculator.html   — same calculator, for embedding/reuse in a multi-calculator project
LICENSE
README.md
```

## Usage

No build step, no dependencies — just open `index.html` in a browser, or copy the `<body>` contents into any page. All CSS and JS are inlined and scoped under `#dcw`, so it won't collide with existing page styles.

## License

MIT — see [LICENSE](LICENSE).

## Disclaimer

This tool provides estimates for general information and is not a guarantee of athletic outcome or a substitute for coaching or medical advice.
