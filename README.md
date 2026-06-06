# FireForm Website

[![Digital Public Good](https://img.shields.io/badge/Digital_Public_Good-United_Nations-blue.svg)](https://fireform-core.github.io/FireForm/dpg.html)

The official public website for **FireForm** — a UN-recognized Digital Public Good and **1st Place Winner** of the Reboot the Earth Hackathon, hosted by the United Nations and UC Santa Cruz.

This repository contains the static website only. For the desktop application source code, see the [main FireForm repository](https://github.com/fireform-core/FireForm).

---

## About FireForm

FireForm is an open-source, AI-powered system built to solve administrative overhead for first responders. When a firefighter responds to an incident, they are typically required to file the same report to multiple agencies — county sheriff, local police, emergency medical services — each using their own unique forms. This forces firefighters to spend hours at the end of their shift re-entering the same information, taking them away from critical duties.

FireForm solves this with a **"report once, file everywhere"** approach:

1. A firefighter records a single voice memo or fills out one master field describing the incident.
2. An open-source, locally-run LLM (Mistral via Ollama) extracts all key information into a structured JSON file.
3. FireForm uses that single JSON object to automatically populate every required PDF template for all relevant agencies.

The result is hours saved per shift, per firefighter — with no data ever leaving the local machine.

---

## What This Repo Contains

This is a plain HTML/CSS static site serving as the public-facing presence for the FireForm project.

| File | Description |
|---|---|
| `index.html` | Main landing page with project overview and download links for macOS, Windows, and Linux |
| `dpg.html` | FireForm's Digital Public Good certification and UN Sustainable Development Goal (SDG) relevance |
| `privacy.html` | Full privacy policy detailing FireForm's local-first, offline data handling and compliance with HIPAA, CCPA, and GDPR |
| `terms.html` | Terms of service |
| `styles.css` | Shared stylesheet across all pages |

---

## Running Locally

No build step is required — this is a plain static site.

```bash
# Clone the repository
git clone https://github.com/fireform-core/fireform-website.git
cd fireform-website

# Open directly in your browser
open index.html
```

To serve it with a local HTTP server (recommended to avoid font/asset CORS issues):

```bash
npx serve .
# or
python3 -m http.server 8080
```

---

## Deployment

The site is deployed via **GitHub Pages** from the `main` branch. Every push to `main` is reflected on the live site automatically. No CI pipeline or build process is needed.

The live site is linked from the main FireForm repository as the canonical source for DPG documentation, the privacy policy, and terms of service.

---

## Contributing

Contributions to the website (copy improvements, accessibility fixes, new pages) are welcome. Please read the [Contributing Guide](https://github.com/fireform-core/FireForm/blob/main/CONTRIBUTING.md) and [Code of Conduct](https://github.com/fireform-core/FireForm/blob/main/CODE_OF_CONDUCT.md) in the main repository before submitting a pull request.

---

## License

This project is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.
