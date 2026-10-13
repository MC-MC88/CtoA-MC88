README.md

```markdown
# MC88 STUDIO

A hub for three small tools that share one idea: simple utilities running entirely in your browser, talking straight to your own GitHub account. No servers, no subscriptions, no tracking.

**Live:** `https://MC-MC88.github.io/MC88-STUDIO/`

---

## What's inside

| Tool | What it does | Folder |
|------|--------------|--------|
| **MC88 STUDIO** | Landing page — pick one of the three tools | `/` |
| **CtoA88** | Turn an HTML project into an Android APK, built in the cloud | `/ctoa88/` |
| **push88** | Push files from your phone into a GitHub repo, pull them back anywhere | `/push88/` |
| **issues88** | Capture GitHub issues in one tap, offline-friendly, multi-repo | `/issues88/` |

---

## The three tools

### CtoA88 — HTML to APK

Drop an HTML file or a ZIP of a project, and CtoA88 generates a complete Android project, pushes it to your repo, and lets GitHub Actions build the APK for you. When it's done, the APK downloads back to your phone.

- Supports single `.html` files, ZIP archives, and folder uploads
- Auto-sanitizes the project (fixes paths, adds charset, removes junk)
- Live phone preview inside the page
- Built-in guide, 5 themes

### push88 — File bridge

A two-way bridge between your device and any GitHub repository. Push files with one tap, pull them back on any other device, browse and delete from anywhere.

- Push tab — upload files, folders or ZIPs to a chosen path
- Pull tab — browse the repo and download any file
- Files tab — full file manager (navigate, open, delete)
- Activity tab — log of every action and error
- 5 themes cycled by one button

### issues88 — One-tap issue capture

Write a GitHub issue the moment you notice it, without opening a laptop. Queues offline if you have no signal, sends itself the moment you are back online.

- Single-field capture, optional details and labels
- Multi-repo — track several projects from one screen
- Pending / Sent lists with retry and GitHub links
- 5 themes cycled by one button
- Built-in guide for first-time users

---

## Structure

```

MC88-STUDIO/
├── index.html       hub page
├── ctoa88/
│   └── index.html
├── push88/
│   └── index.html
├── issues88/
│   └── index.html
└── README.md

```

Each tool is one HTML file. No build step, no dependencies to install.

---

## Setup

1. Clone or download the repository.
2. Host it on GitHub Pages, Netlify, Cloudflare Pages, or any static host — or just open `index.html` locally.
3. If you rename folders, edit the `CONFIG.links` block inside the hub `index.html` so the cards point to the right places.

### GitHub token (per tool)

CtoA88, push88 and issues88 all need a personal access token to talk to the GitHub API. Create one at:

`https://github.com/settings/tokens/new`

Scopes needed:
- **CtoA88** → `repo` + `workflow`
- **push88** → `repo`
- **issues88** → `repo`

Paste the token into each tool's Settings panel once. It stays only on that device.

---

## Common features

- Single HTML file per tool, no backend, no build
- 5 themes cycled by a single button
- Installable as a PWA (Add to Home screen)
- Arabic and Latin text both render cleanly
- Zero tracking, zero analytics, zero cookies

## Privacy

Your tokens and files stay on your device and go directly to `api.github.com`. Nothing is logged, proxied or stored anywhere else. To revoke access, delete the token from GitHub settings.

## License

Personal project. Use at your own risk.

---

**Mohamed Cheikh (MC88)**
[mohamed005cheikh@gmail.com](mailto:mohamed005cheikh@gmail.com) · [+222 30 72 64 75](https://wa.me/22230726475) · [github.com/MC-MC88](https://github.com/MC-MC88)
```

---

Repository description (one line)

```
MC88 STUDIO — hub for three personal tools: HTML→APK builder, phone↔GitHub file bridge, and one-tap issue capture. Single files, no backend, installable PWA.
```
