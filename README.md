# Secret Book

A responsive, notebook-inspired online diary built as a single static HTML page.

## Features

- Public landing and preview page
- Passphrase-protected journal with create, edit, delete, and search
- AES-GCM encryption for journal data stored in this browser
- Responsive layout for desktop and mobile

## Run locally

Open `index.html` in a modern browser, or serve this folder over localhost:

```sh
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Publish with GitHub Pages

1. Create a GitHub repository.
2. Upload `index.html`, `README.md`, and `.gitignore` to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and the `/(root)` folder, then save.
6. Open the published URL shown in the Pages settings.

Before publishing, replace the example contact address `hello@secretbook.example` in `index.html` with an address you control.

## Privacy and limitations

This is a static, browser-only demo—not a production account or cloud diary service. A passphrase derives the encryption key locally; journal content is encrypted in this browser's local storage and is not synced or backed up. Clearing browser data or forgetting the passphrase means the journal cannot be recovered. Anyone with access to an unlocked browser session or compromised device may still access the journal. Do not rely on this app to store highly sensitive information.
