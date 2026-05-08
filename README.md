# BIB Solution Calculator · 袋中袋方案速算器

> A professional calculator for Bag-in-Bag (BIB) secondary packaging solutions.  
> 专业的袋中袋二次包装方案速算工具。

**Live Demo / 在线工具**: [Open Calculator →](https://YOUR-USERNAME.github.io/bib-calculator/)

![Calculator preview](https://img.shields.io/badge/status-live-success) ![License](https://img.shields.io/badge/license-MIT-blue)

---

## What it does / 功能

Input pouch specifications and stacking configuration, get instant engineering output:

输入小袋规格与堆叠配置，即时得到完整工程数据：

- **Theoretical stack** (A × B × H) — based on `n × a` formula
- **Actual stack** (A₁ × B₁ × H₁) — accounting for 18mm pouch overlap
- **Empty bag spec** (A' × B' × H') — for direct quotation to bag suppliers
- **Capacity** — bags/min, tons/hour, annual output (300 days × 2 shifts)
- **Machine recommendation** — VBIB-120 (roll film) or WBIB-90 (woven)

---

## Stack diagram engine / 垛型示意引擎

The calculator renders an engineering-style stack diagram with:

- Pillow-pouch lens shape with vertical sealing tails
- Horizontal overlap (18mm) between adjacent pouches in a layer
- Vertical compression between stacked layers
- Remainder layer placement (on top, horizontally centered)
- Real-time response to all parameter changes

---

## Engineering formulas / 工程公式

```
Bag Weight     = pouch_weight × pouch_count

Theoretical:   A  = n × a    (top-to-top)  or  n × b  (side-to-side)
               B  = b  or  a
               H  = layers × c

Actual:        A₁ = A − (n−1) × 18
               B₁ = B
               H₁ = H

Empty (Film):  A' = A − (n−1) × 18
               B' = B
               H' = 1.1H + 1.0B + 100

Empty (Woven): A' = A − (n−1) × 18
               B' = B
               H' = 1.1H + 1.0B + 50
```

---

## Designed by / 设计者

**Hefei Zengran Intelligent Packaging Technology Co., Ltd**  
合肥正远智能包装科技有限公司

Specialized in BIB secondary packaging machinery, VFFS systems, and rotary pre-made bag machines for sugar, salt, flour, seeds, and detergent industries.

---

## License

MIT — free to use, modify, and distribute.
