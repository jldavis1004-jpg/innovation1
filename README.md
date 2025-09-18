# innovation1
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>README — iPhone Legacy Map</title>
  <link rel="stylesheet" href="style.css" />
  <style>
    body { max-width: 900px; margin: 0 auto; padding: 24px; }
    code { background: rgba(255,255,255,.08); padding: 2px 6px; border-radius: 6px; }
    pre { background: rgba(255,255,255,.06); padding: 12px; border-radius: 10px; overflow: auto; }
    h1,h2,h3 { margin-top: 1.6em; }
    a { color: var(--accent); }
  </style>
</head>
<body>
  <h1>iPhone Legacy Map — Template</h1>
  <p>This repo is a fully offline, single‑page HTML/CSS/JS prototype that frames your content inside an <strong>iPhone 14‑style</strong> device. Tap app icons on the Home Screen to open in‑phone infographic panels.</p>

  <h2>Quick Start</h2>
  <ol>
    <li>Open <code>index.html</code> in any modern browser.</li>
    <li>Edit <code>app.js</code> and replace placeholder content in the <code>APPS</code> object.</li>
    <li>To add icons, place SVG/PNG files in <code>assets/icons</code> and swap the <code>&lt;img src&gt;</code> for each <code>.app-icon</code> in <code>index.html</code>.</li>
  </ol>

  <h2>Customize App Content</h2>
  <p>All content lives in the <code>APPS</code> constant in <code>app.js</code>. Each app has a <code>title</code> and a list of <code>sections</code>. Built‑in section types:</p>
  <ul>
    <li><code>kpis</code>: small stat tiles</li>
    <li><code>text</code>: heading + rich text</li>
    <li><code>figure</code>: placeholder box for your charts/graphics</li>
  </ul>
  <p>You can define your own section types. Add a new <code>type</code> and extend <code>renderSection()</code> to render it.</p>

  <h2>Interaction Model</h2>
  <ul>
    <li>Launch animation emulates native feel (scales up, fades in).</li>
    <li><strong>Home</strong> returns to the icon grid; <strong>Back</strong> is future‑proofed for deeper screens.</li>
    <li>Keyboard shortcuts: <code>Esc</code> = Home, <code>Backspace</code> = Back.</li>
  </ul>

  <h2>Theme</h2>
  <p>Toggle light/dark with the <em>Theme</em> button. Preference is saved in <code>localStorage</code>.</p>

  <h2>Packaging</h2>
  <p>This is a static app; zip these files and you’re ready to present or host (GitHub Pages, Netlify, etc.).</p>

  <h2>Attribution</h2>
  <p>Icons are simple inline SVGs you can replace. No external libraries are used.</p>
</body>
</html>
