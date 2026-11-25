# Investment Growth Projection Calculator

A lightweight, single-file interactive web calculator that visualizes long-term wealth creation through **lump-sum investing** and **Systematic Investment Plans (SIPs)** using monthly compounding.

---

## ✨ Features

* **Real-Time Interactive Controls:** Adjust starting lump sum, monthly SIP, expected annual return (`%`), and time horizon (`years`) using synchronized range sliders or direct numeric inputs.
* **Dynamic SVG Area Chart:** Renders smooth, responsive growth curves comparing **Total Money Invested** against **Projected Portfolio Value** with automatic axis scaling (`K`, `M`, `Cr`).
* **Live Summary Metrics:** Instant top-level cards displaying total principal invested, expected return rate, and projected maturity value.
* **Zero Build Step:** Built as a self-contained `index.html` file using vanilla JavaScript, native SVG DOM rendering, and Tailwind CSS via CDN.

---

## 🚀 Getting Started

No installation, package manager, or local server is required.

1. Download or save `index.html` to your computer.
2. Double-click `index.html` to open it in any modern web browser (Chrome, Edge, Safari, or Firefox).
3. Drag any slider or type custom numbers into the dark pill boxes to simulate different investment scenarios.

---

## 🧮 Financial Formula Used

The calculator models **monthly compounding** over $t$ years ($n = 12 \times t$ total months) at an annual interest rate $r$ (expressed as a decimal, e.g., $12\% = 0.12$):

* **Monthly Interest Rate ($i$):**
  $$i = \frac{r}{12}$$

* **Total Money Invested ($I$):**
  $$I = P + (M \times n)$$

* **Projected Portfolio Value ($A$):**
  $$A = P(1 + i)^n + M \left( \frac{(1 + i)^n - 1}{i} \right)$$

Where:
* $P$ = Starting lump sum (`₹`)
* $M$ = Monthly SIP contribution (`₹`)
* $n$ = Total number of months ($\text{years} \times 12$)

---

## 📁 Project Structure

```text
├── index.html      # Complete application (HTML structure, custom slider CSS, Tailwind, & SVG chart engine)
└── README.md       # Project documentation
```

---

## 🛠️ Customization

* **Default Values & Slider Ranges:** Edit the `min`, `max`, `step`, and `value` attributes on the `<input type="range">` and `<input type="number">` tags inside `index.html`.
* **Currency Formatting:** Update the `"₹"` symbol and `"en-US"` locale inside `formatCurrency()` and `formatShortY()` in the `<script>` block if you wish to switch currencies or numbering formats.