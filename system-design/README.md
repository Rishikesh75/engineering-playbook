# system-design-playbook

## Excalidraw image exports

Every `.excalidraw` file in this repo is exported to an SVG under `output/image` at the repo root, keeping the same relative path. For example, `system-design/HLD/AlexuPart-1/Chapter1.excalidraw` becomes `output/image/system-design/HLD/AlexuPart-1/Chapter1.svg`.

One-time setup after cloning, from the repo root:

```powershell
npm install
npm run setup:browser
npm run setup:hooks
```

Run the export manually from the repo root with:

```powershell
npm run export:diagrams
```

The configured Git `pre-commit` hook runs the export and stages the generated SVG files automatically, so source diagrams and their images are committed together and visible on GitHub.
