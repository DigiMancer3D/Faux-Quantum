# Faux-Quantum (Faux-Qbit Generator)

**Faux-Quantum** is a single-file creative coding experiment that turns any short text into dense, visually rich pseudo-quantum binary structures. It feels like a miniature quantum computer simulator, but everything runs instantly in your browser using clever (and intentionally over-the-top) mathematics.

Type something → watch it get transformed through stacked roots, parity checks, prime detection, bit recombination, and "mining" layers.

## Live Demo
Just open **`Faux-Qbit-Generator.html`** in any browser (100% offline).

---

## How This Demo Works

### Step-by-Step Transformation

1. **Input → Base64 + Character Codes**
   - Text is turned into Base64 (`btoa()`).
   - Each character’s ASCII value is extracted.

2. **Length Magic**
   - `len` = input length + Base64 length.
   - Multiple reference values are calculated:
     - `mq` = 16th root of a derived number (extreme compression feel)
     - `vc` = stacked power/square-root
     - `sr` = square root
     - `po` = squared value

3. **Core Bit Generation (ck1–ck8)**
   - Each `ck` bit is decided by a combination of:
     - Even/Odd (`% 2`)
     - Divisible by 3 (`% 3`)
     - Comparison against the reference values (`len > mq`, `len < vc`, etc.)

4. **Prime Detection**
   - A simple trial-division loop checks if derived numbers are prime → sets flags that influence later bits.

5. **Multi-Layer Bit Fields**
   - `set1`–`set16` → first 4×4 grid of bits
   - `joinset` arrays → recombine bits in different orders (forward, reverse, shifted)
   - `rest` arrays → detect equality between layers (creates repeating patterns)
   - `left` arrays → further cross-checks and flips

6. **Mining Simulation**
   - Creates additional "mined" layers (`mine1a`–`mine16d`) by comparing the original bits against the recombined ones.
   - Final output shows the "entangled" result + packed signatures.

This is **not** real quantum computing, it’s artistic chaos designed to look and feel quantum-inspired.

---

## Math Highlights (Simplified)

| Operation              | What it does                              | Why it feels "quantum"                     |
|------------------------|-------------------------------------------|--------------------------------------------|
| Stacked roots (`mq`)   | 16th root of a derived value              | Extreme compression / "deep levels"       |
| Parity + Modulo        | `% 2`, `% 3`, length comparisons          | Simple rules create complex-looking grids |
| Prime checker          | Trial division loop                       | Classic number-theory flavor               |
| Bit recombination      | `joinset`, `rest`, `left` arrays          | Entanglement-style mixing of bits          |
| Mining layers          | Multiple passes of equality checks        | Simulated "proof-of-work" feel             |
| Signature packing      | Everything Base64’d together              | Final "proof" that can be copied           |

---

## Features

- Instant transformation from plain text to rich binary art
- Live display of **Core**, **Square**, **Field**, and **Mined** sections
- Clickable "📝" icons that expand full Base64 signatures
- Optional 5-character secret code for personalization
- Fully self-contained, no server, no install

## Terminology Table

| Term in UI/Code       | What it actually is                        | Plain English                              |
|-----------------------|--------------------------------------------|--------------------------------------------|
| **Faux-Qbit**         | The entire generator                       | Fake quantum bit toy                       |
| **BIN Core**          | First 8 bits from length/math checks       | The "engine" of the binary output          |
| **BIN Square**        | Visual 2×4 grid of core bits               | Pretty square version                      |
| **BIN Field**         | Full expanded multi-line bit pattern       | The complete "quantum landscape"           |
| **Mining**            | Extra comparison layers + display          | The fun "processing" animation             |
| **Signatures**        | Packed Base64 of everything + secret       | The final signed proof package             |
| `ck1`–`ck8`           | Decision bits (parity, modulo, prime)      | Hidden flags that decide every 0 or 1      |
| `joinset` / `rest` / `left` | Recombination & equality checks     | Ways of mixing and checking bits           |

---

## Project Status

**🚧 Under Construction • Pure Creative Math Playground**

- Extremely fun and satisfying to play with.
- The code is intentionally dense and artistic, a love letter to mathematical chaos.
- Future ideas: Save outputs, more transformation modes, canvas visualizer, export as SVG, real quantum-inspired algorithms.

Contributions, new math layers, visual upgrades, or help cleaning/refactoring are **very welcome**!

---

**Made by** 3Douglas Pihl (DigiMancer3D)  

---
