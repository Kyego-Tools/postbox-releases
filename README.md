<p align="center">
  <img src="https://raw.githubusercontent.com/YOUR_ORG/postbox-releases/main/banner.png" alt="PostBox" width="600" />
</p>

<h1 align="center">PostBox</h1>
<p align="center">
  <strong>The free, self-hosted social media scheduler.</strong><br/>
  Schedule posts across Facebook, Instagram, TikTok, Twitter/X, and Threads — with team collaboration and approval workflows.
</p>

<p align="center">
  <a href="https://github.com/YOUR_ORG/postbox-releases/releases"><img src="https://img.shields.io/github/v/release/YOUR_ORG/postbox-releases?label=latest&color=7C3AED" alt="Latest Release" /></a>
  <img src="https://img.shields.io/badge/self--hosted-Docker-2496ED?logo=docker" alt="Docker" />
  <img src="https://img.shields.io/badge/backend-Convex-EE342F" alt="Convex" />
  <img src="https://img.shields.io/badge/license-MIT-green" alt="License" />
</p>

---

> **This is the public releases repository for PostBox.**  
> It contains version history and release notes. Source code is available to approved contributors.

---

## What is PostBox?

PostBox is a free alternative to Buffer, Hootsuite, and Later — built to be self-hosted on your own server. No subscription fees. Your data stays yours.

**Key features:**
- 📅 Schedule posts across 5 platforms from one dashboard
- 👥 Team roles — admin, full access, approval required
- ✅ Post approval workflow before anything goes live
- 📊 Analytics pulled directly from your connected accounts
- 🔥 Posting streak tracker across app and native posts
- 🐳 One-command Docker deploy

---

## Quick Install

**Requirements:** Docker, a free [Convex](https://convex.dev) account

```bash
# 1. Clone the repo (requires access)
git clone https://github.com/YOUR_ORG/postbox.git
cd postbox

# 2. Copy and fill in your environment file
cp .env.docker.example .env.docker
# Edit .env.docker with your Convex URL, deploy key, and platform credentials

# 3. Start
docker compose up --build -d
```

Open [http://localhost:3000](http://localhost:3000) — the first account you create becomes the admin.

---

## Updating

```bash
git pull
docker compose up --build -d
```

The app will show you when a new version is available under **Settings → About**.

---

## Connecting Platforms

| Platform | Credentials needed |
|----------|--------------------|
| Facebook | App ID + Secret |
| Instagram | Same Meta app as Facebook |
| TikTok | Client Key + Secret |
| Twitter/X | Client ID + Secret (OAuth 2.0) |
| Threads | Same Meta app as Facebook |

Full setup guides are in the docs (coming soon).

---

## Releases

All releases are listed in the [Releases tab](https://github.com/YOUR_ORG/postbox-releases/releases).  
Each release includes:
- What's new
- Bug fixes
- Breaking changes (if any)
- Update instructions

---

## License

MIT — free to use, modify, and self-host.
