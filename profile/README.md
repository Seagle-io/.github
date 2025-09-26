<!-- README -->

<h1 align="center">Sofia IA</h1>

<p align="center">
  <em>Desktop visual coach — overlay, UI Automation, OCR — no browser extension required.</em>
</p>

<p align="center">
  <img alt="AI" src="https://img.shields.io/badge/AI-0ea5e9?logo=openai&logoColor=white&labelColor=000&style=flat-square" />
  <img alt="Desktop Overlay" src="https://img.shields.io/badge/Windows-Desktop%20Overlay-0ea5e9?logo=windows11&logoColor=white&labelColor=000&style=flat-square" />
  <img alt="UI Automation" src="https://img.shields.io/badge/Windows-UI%20Automation%20-8b5cf6?logo=windowsxp&logoColor=white&labelColor=000&style=flat-square" />
  <img alt="Local-first" src="https://img.shields.io/badge/Local--first-2b3137?logo=shield&logoColor=white&labelColor=000&style=flat-square" />
</p>

<hr />

<blockquote>
  <strong>Mission</strong> — Build a desktop visual coach that guides users step-by-step via an intelligent <strong>overlay</strong> (UI Automation + OCR + icon templates), <u>without</u> a browser extension.
</blockquote>

## MVP Scope
<ul>
  <li>Desktop overlay (halo + arrow + tooltip) — <strong>Windows first</strong>.</li>
  <li>Multi-sensor detection: <strong>UIA</strong> (Windows), <strong>OCR</strong> (Tesseract), <strong>template matching</strong> (OpenCV).</li>
  <li>Step engine driven by a <strong>JSON/YAML DSL</strong> (targets <code>uia</code>/<code>text</code>/<code>icon</code>, fallbacks, manual assist).</li>
  <li><strong>Manual assist</strong>: point it yourself, text search, plan B, skip/force.</li>
  <li><strong>Local-first</strong> processing (privacy: on-device).</li>
</ul>

## Proposed Repos
<table>
  <thead>
    <tr><th>Repo</th><th>Role</th><th>Language</th></tr>
  </thead>
  <tbody>
    <tr><td><code>sofia-desktop</code></td><td>Desktop app + overlay + step engine</td><td>C# / .NET (WPF)</td></tr>
    <tr><td><code>sofia-vision</code></td><td>OCR + templates + heuristics</td><td>Python / C# bindings</td></tr>
    <tr><td><code>sofia-dsl</code></td><td>DSL schema + examples + authoring tools</td><td>TypeScript / JSON</td></tr>
    <tr><td><code>sofia-docs</code></td><td>Guides, conventions, playbooks</td><td>Markdown</td></tr>
  </tbody>
</table>

##  Short Roadmap
<details open>
  <summary><strong>See milestones</strong></summary>
  <ul>
    <li><strong>Sprint 1</strong>: WPF overlay, UIA finder, step runner (DSL), manual assist (point/skip), local logs.</li>
    <li><strong>Sprint 2</strong>: OCR + fuzzy search, template matching, Plan B, recorder → DSL generation, FR/EN i18n.</li>
  </ul>
</details>

## Contributing
Developer Guide: [https://github.com/DracJulien/dev-guide](https://github.com/DracJulien/dev-guide)
<ol>
  <li>Open an issue (bug/feature) using a clear <strong>template</strong>.</li>
  <li>Fork → branch (<code>feat/...</code>) → PR to <code>main</code>.</li>
  <li>Follow lint/tests & commit conventions.</li>
</ol>

## Shortcuts (overlay)
- Exit help: <kbd>Esc</kbd><br/>
- Replay step: <kbd>R</kbd><br/>
- Force “found”: <kbd>F</kbd><br/>
- Help: <kbd>?</kbd>

## Security & Privacy
<ul>
  <li><strong>On-device</strong> processing.</li>
  <li>No browser extension.</li>
  <li>Blur sensitive data in debug captures.</li>
  <li>Report vulnerabilities: <em>juliendrac@pm.me</em>.</li>
</ul>
