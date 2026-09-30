# Aura

**Say it. Stay anonymous. Trusted circles only.**

Aura is an anonymous social app built around honesty and trust — instead of posting to the open internet, you share inside small, invite-only **circles** (your class, your fellowship, your friend group). Posts are anonymous to other members, but every circle has real structure, leadership, and moderation behind the scenes.

Built as a 2026 holiday project — from idea to a working, installable app, entirely from an Android phone with no laptop.

🔗 **Live app:** [auraappbyjet.netlify.app](https://auraappbyjet.netlify.app)

---

## Features

- **Anonymous accounts** — email/password auth, anonymous display name shown to others instead of your identity
- **Circles** — invite-code based groups, each with a leader and optional co-leaders
- **Posts** — text, photos, and voice notes, mixed freely in one feed
- **Public or private** — post to the whole circle, or hand-pick exactly who sees it
- **Reactions** — ❤️ 👍 😂 😢 on any post
- **Forwarding** — send a post from one of your circles into another
- **Circle leadership** — leaders can promote co-leaders, remove members, and disband a circle
- **History control** — leaders can choose whether new joiners see a circle's past posts
- **Moderation** — report a post to circle leadership, or personally block another member
- **Notifications** — optional in-app alerts for new posts, fully toggleable
- **Installable app** — full PWA with offline app shell, home-screen install, and a packaged Android build (via PWABuilder) ready for the Play Store

## Tech stack

- **Frontend:** Vanilla HTML/CSS/JavaScript — no framework, single-file app
- **Backend:** [Firebase](https://firebase.google.com/) (Authentication + Firestore)
- **Media storage:** [Cloudinary](https://cloudinary.com/) for photo/voice note uploads
- **Hosting:** [Netlify](https://www.netlify.com/)
- **Android packaging:** [PWABuilder](https://www.pwabuilder.com/)

## Security

Firestore access is controlled by rules enforcing:
- Only circle members can read that circle's posts
- Only a post's author or a circle leader/co-leader can delete it
- Only leaders/co-leaders can view or act on reports
- Only a circle's leader can disband it

## Why circles instead of a fully open feed

Fully anonymous, fully open apps (Yik Yak, early confession apps) tend to struggle with abuse and low trust once anyone can see anyone. Aura starts from an existing real community instead — same anonymity, but grounded in a circle people actually chose to join, with real leadership able to step in.

## Project background

Built solo over a Nigerian university holiday break, entirely on an Android phone — no laptop, no local dev environment. Every part of the stack (backend setup, code, deployment, Android packaging) was done through mobile browser tools.

---

*Mechanical Engineering student, Federal University of Technology Akure (FUTA).*
