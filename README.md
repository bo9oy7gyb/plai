# Plai Proposal Site

Static, single-file proposal site hosted via GitHub Pages.

## What this is

A self-contained HTML proposal site behind a soft password gate. Single `index.html` file — no build step, no framework, no dependencies. All CSS, JavaScript, and content live inside the one file.

## Access

The site is gated by a client-side password. The password is shared separately from the URL.

> **Note on the gate:** The password gate is JavaScript-enforced and the proposal content is present in the HTML source, so a determined viewer can read it by inspecting the page source. The gate is a soft deterrent that prevents the URL from being passively shareable, not a security boundary. For true access control, this would need to move to a host that supports server-side gating (Vercel/Netlify with a serverless function, or Cloudflare Access).

## Deploying

1. Push this repo to GitHub (already done if you're reading this on github.com).
2. Repo Settings → Pages → Source: "Deploy from a branch" → Branch: `main` → Folder: `/ (root)` → Save.
3. Wait a few minutes for the first build. The URL appears in the Pages settings panel once live.

## Updating

Edit `index.html` directly in the GitHub web editor (pencil icon), or replace the file via Add file → Upload files. Commits to `main` trigger an automatic rebuild; the new version is live in 1–5 minutes.

## Local preview

To preview locally without GitHub Pages, just open `index.html` in a browser. No server needed.
