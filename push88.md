# push88

A personal file bridge between your device and GitHub. Push files from your phone to a repository, pull them back on any other device. No backend, no server, no subscription — just one HTML file and your own GitHub account.

## Features

- **Push** — upload files, folders, or ZIP archives straight to your repo
- **Pull** — browse any folder in the repo and download files with one tap
- **Files** — full file manager: navigate, open, delete
- **Activity** — timestamped log of every action and error
- **Settings** — username, repo, branch, token, default upload path
- **5 themes** — Day, Night, Sunset, Sunrise, Rain
- **Installable PWA** — add to home screen, runs full-screen like a native app
- **Direct API calls** — the browser talks to GitHub. Your token never leaves the device.

## Quick start

1. Create an empty repository on GitHub (private or public).
2. Create a [personal access token](https://github.com/settings/tokens/new) with the **repo** scope.
3. Open `index.html` in Chrome or Edge.
4. Open **Settings** and fill in: username, repo name, branch (`main`), token, default path (e.g. `uploads/`).
5. Click **Save & test** — the connection strip turns green.
6. Go to **Push**, pick files, upload.

## Install as an app

Chrome menu → **Install push88** → opens full-screen from your home screen, with native file picker and download support.

## How it works

The browser calls the GitHub REST API directly. Files are base64-encoded and committed to your repository via the Contents API. No proxy, no intermediate server, no analytics, no third party ever sees your data.

## Limits

- 40 MB per upload batch (browser memory)
- GitHub Contents API: ~1 MB per file recommended, up to 100 MB hard limit
- One commit per file — for large batches, prefer ZIP uploads

## Privacy

- Token stored only in `localStorage` on this device
- All traffic goes directly to `api.github.com`
- Nothing is logged, tracked, or sent anywhere else

## License

Personal project. Use at your own risk.

---

**Mohamed Cheikh** · [mohamed005cheikh@gmail.com](mailto:mohamed005cheikh@gmail.com) · [+222 30 72 64 75](https://wa.me/22230726475) · by MC88
