<div align="center">

<img src="assets/banner.svg" alt="cspbuilder" width="100%">

<p>
  <a href="https://cyberloop-dev.github.io/cspbuilder/"><img alt="Live demo" src="https://img.shields.io/badge/live%20demo-open-be123c?style=for-the-badge"></a>
  <img alt="Dependencies" src="https://img.shields.io/badge/dependencies-zero-818cf8?style=for-the-badge">
  <img alt="Runs in browser" src="https://img.shields.io/badge/runs-in%20your%20browser-22c55e?style=for-the-badge">
</p>

**Build a Content-Security-Policy without guessing: toggle sources, start from presets, copy the header.**

</div>

---

## ✨ Features

- 🧱 **12 directives** covered: `default-src`, `script-src`, `style-src`, `img-src`, `font-src`, `connect-src`, `media-src`, `object-src`, `frame-src`, `frame-ancestors`, `base-uri`, `form-action`
- 🎛️ **One-click source chips** (`'self'`, `'none'`, `https:`, `data:` and more) plus a field to add your own hosts
- 🚀 **Presets**: Strict start, Lockdown, Static site + HTTPS images, or Empty
- ⚠️ **Live warnings** for risky choices like `'unsafe-inline'`, `'unsafe-eval'`, wildcards, and missing `object-src`, `base-uri` or `frame-ancestors`
- 🧪 **Report-Only mode** to log violations without blocking anything
- 📋 **Copy-ready output** as an HTTP header or a `<meta>` tag
- 🔒 100% in your browser, one HTML file, nothing is uploaded

## 🚀 Quick start

Open the [live demo](https://cyberloop-dev.github.io/cspbuilder/), or:

```bash
git clone https://github.com/CyberLoop-dev/cspbuilder.git
cd cspbuilder
open index.html
```

## 🧪 Example output

```text
Content-Security-Policy: default-src 'self'; img-src 'self' data:; object-src 'none'; base-uri 'self'; frame-ancestors 'self'; form-action 'self'
```

## ⚖️ Notes

- `frame-ancestors`, `report-uri` and `sandbox` are ignored in `<meta>` tags by browsers, so the meta output leaves them out. Use the HTTP header for those.
- Roll out with **Report-Only** first, watch for violations, then enforce.

## 📄 License

MIT
