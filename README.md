# Diamond Shape Ratio Calculator

A free, responsive, browser-based educational calculator from **Laxmi Jewellers Dubai**.

**Demo:** Publish with GitHub Pages using the steps below. No account, backend, database, cookies or paid services are needed for the tool.

![Diamond Shape Ratio Calculator desktop preview](docs/desktop-preview.png)

## Features

- Live length ÷ width calculation (2 decimal places)
- Interactive shape illustration for **oval, pear, marquise, emerald, radiant, cushion, asscher, princess, and round**
- Side-by-side comparison of two diamonds
- Measurement validation and error messages
- Copy a result or a shareable URL with the entered measurements
- Example cards, educational explanations and FAQs
- Responsive layout for mobile, tablet and desktop
- Keyboard-friendly controls, reduced-motion support and semantic HTML
- No analytics, external JavaScript, API calls or user-data uploads

## Run locally

Open `index.html` using a local HTTP server because the calculator uses ES modules.

```bash
python -m http.server 8000
```

Visit `http://localhost:8000/`.

Alternative:

```bash
npx serve .
```

## Publish on GitHub Pages

1. Create a new **public** GitHub repository, for example `diamond-shape-ratio-calculator`.
2. Upload **all files and folders** in this project to the repository root (not just `index.html`).
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Choose branch **main**, folder **/(root)** and click **Save**.
6. Once GitHub displays the public URL, open it and test the calculator.

The resulting link normally resembles:

`https://YOUR-USERNAME.github.io/diamond-shape-ratio-calculator/`

Replace `YOUR-USERNAME` with your actual GitHub username. This is an example, not a confirmed live URL.

## How the calculation works

`length-to-width ratio = length in mm / width in mm`

Example: `9.00 / 6.00 = 1.50`, displayed as `1.50:1`.

Use the longer face-up dimension as length. The interface flags reversed measurements instead of silently swapping them. Only outline proportions are described; the tool does **not** grade cut quality, brightness, value, authenticity or symmetry.

## Privacy and links

All calculations run locally in the browser. No entries are sent to a server. The **Copy share link** action adds the entered dimensions to the URL query string, so anyone with that link can read them. It does not automatically transmit the URL.

The external `https://laxmijewellers.ae/` links are publisher attribution, not checkout links. Before publishing, verify all business information, brand-authorisation and product/platform policy requirements.

## Testing

Requires Node.js 20+ and no additional packages:

```bash
npm test
```

Browser acceptance testing should also be performed after publishing.

## Sources for the mathematical and educational approach

- [GIA: How to Buy a Quality Diamond](https://4cs.gia.edu/en-us/blog/how-to-buy-a-quality-diamond/)
- [GIA: Oval Cut Diamond Guide](https://4cs.gia.edu/en-us/blog/oval-cut-diamond-guide/)

These sources inform the distinction between length-to-width ratio and overall cut grade. The app does not use arbitrary "ideal" ratios to score diamonds.

## Publisher

Laxmi Jewellers is a trade name owned and operated by Amit Verma Jewellery LLC, a company registered in the UAE.

## Licence

MIT. See `LICENSE`.
