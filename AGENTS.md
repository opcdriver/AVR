# AGENTS.md

## Cursor Cloud specific instructions

### What this repo is
This repository is a single **static HTML landing page** for the "Smart AVR System" product. The page is trilingual (Ukrainian / English / Russian) with a client-side language switcher.

- The only source file is `README.md`, which despite its extension contains a full standalone HTML document (`<!DOCTYPE html> ...`), not markdown.
- Styling comes from **CDN-hosted Tailwind CSS and Font Awesome** (`cdn.tailwindcss.com`, `cdnjs.cloudflare.com`), so full styling/icons require outbound internet access. The language switcher itself works offline because its show/hide rules live in the inline `<style>` block and inline `<script>`.
- `README.md` references an image `image_1.png` that does not exist in the repo, so that one image renders broken. This is expected and does not affect the rest of the page.

### No build / lint / test tooling
There is no package manager, build system, linter, or test suite in this repo. There is nothing to compile.

### Running the app in dev
Serve the repo root over HTTP. Because the file is named `README.md`, map `.md` to `text/html` so browsers render it instead of showing source:

```
python3 -c "import http.server,socketserver; h=http.server.SimpleHTTPRequestHandler; h.extensions_map['.md']='text/html'; socketserver.TCPServer(('',8000),h).serve_forever()"
```

Then open `http://localhost:8000/README.md`. The core interaction is the language dropdown in the top-right (UA / EN / RU), which updates all page text instantly.
