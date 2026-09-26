<div align="center">

# 🌊 PierPulse

**Your computer is the cloud.**
Browse, discuss, and edit files together with anyone - right in the browser.

No uploads. No cloud storage. No accounts.

[![Website](https://img.shields.io/badge/website-pierpulse.com-0A84FF?style=flat-square)](https://pierpulse.com)
[![Cloud Storage](https://img.shields.io/badge/cloud%20storage-none-success?style=flat-square)](#how-it-works)
[![Single File App](https://img.shields.io/badge/app-single%20HTML%20file-orange?style=flat-square)](#how-it-works)
[![Accounts](https://img.shields.io/badge/accounts-not%20needed-blue?style=flat-square)](#faq)
[![License: MIT](https://img.shields.io/badge/license-MIT-informational?style=flat-square)](#license)

[**Live Demo**](https://pierpulse.com) · [Features](#-features) · [How It Works](#-how-it-works) · [Getting Started](#-getting-started) · [FAQ](#-faq)

![PierPulse screenshot](./Screenshot.png)

</div>

---

## 📖 Table of Contents

- [What is PierPulse?](#-what-is-pierpulse)
- [Features](#-features)
- [How It Works](#-how-it-works)
- [Getting Started](#-getting-started)
- [Supported File Types](#-supported-file-types)
- [Browser Compatibility](#-browser-compatibility)
- [Privacy & Security Model](#-privacy--security-model)
- [FAQ](#-faq)
- [Roadmap](#-roadmap)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🧭 What is PierPulse?

PierPulse lets other people **see and work on the files on your computer**, live, from their own browser, anywhere in the world - with no uploading, no syncing, and no "I'll email you the latest version."

It works in four simple steps:

| Step | Action |
|------|--------|
| 1️⃣ | **You host.** Open [pierpulse.com](https://pierpulse.com), pick the folders (or entire drives) you want to share, and a "pier" opens for your session. |
| 2️⃣ | **You invite.** Send the session link to whoever needs access - coworkers, clients, friends. |
| 3️⃣ | **They dock.** Guests open the link in any modern browser. Nothing to install, no account to create. |
| 4️⃣ | **You work together.** Everyone browses the same files at the same time, edits documents together, and talks it over in the built-in chat sidebar. |

The core idea: **your files never leave your computer.** They're not copied to Google Drive, Dropbox, or any server. While a pier is open, PierPulse streams your files directly from your machine to your guests. Close it, and your files exist in exactly one place - yours.

> Think of it as letting someone look over your shoulder at your screen - except they can be on another continent, and you can both point at cell B7 in the same spreadsheet at the same time.

---

## ✨ Features

### 🗂️ One File Browser, Shared Live
Everyone in a session sees the same folder at the same time. A presence line ("3 people viewing this folder"), live typing indicators, and one-click jumps (mention a file in chat and everyone can fly straight to it) keep the room feeling real. Prefer to give a guided tour instead of letting people wander? **Follow Mode** lets one person drive while everyone else rides along - and the wheel can be handed off at any time.

### 💬 A Chat That Lives Next to Your Files
The sidebar is scoped to wherever you are - the conversation happening in `Invoices` stays in `Invoices`. React to messages, send voice notes when typing is too slow, and paste in screenshots you can annotate with a quick markup tool before sending. Need to make a call on something? Fire off a quick poll, and the result is saved to a **decision log** so it never gets lost in the scroll. A **pinned-files shelf** keeps whatever matters one click away.

### 📄 PDFs, Reviewed Together
Open a PDF with your team and page turns stay in sync - nobody is ever asking "wait, which page are you on?" Draw on the document live, with everyone's ink rendered in their own color. Need actual edits instead of comments? The built-in page toolkit reorders, rotates, deletes, extracts, and merges pages, and you can export with the annotations burned in when you're done.

### 📊 Office Files, No Office Needed
Open, view, **and edit** Word (`.docx`), Excel (`.xlsx`), and PowerPoint (`.pptx`) files directly in the browser. When you save, the edited file is written straight back to the host's drive - the original file, in place. No exports, no downloads, no `final_v7_REAL_this_time.docx`.

### 💽 Dock Every Drive You Own
**Multi-Drive Docking** lets a host attach several drives or folders at once - `C:`, `D:`, `F:`, an external disk - and the whole group navigates between them like ordinary folders. Your entire computer becomes one shared workspace.

### ⏪ Never Miss a Thing
Joined the session late? **Catch-Me-Up Replay** shows exactly what was opened, said, and decided while you were away - the meeting minutes nobody had to write.

---

## ⚙️ How It Works

PierPulse has no backend storage layer. The relay server that connects host and guests is a pass-through, not a warehouse - it moves bytes and remembers nothing.

```
      YOUR COMPUTER                  THE RELAY                    GUESTS
 ┌─────────────────────┐        ┌────────────────┐        ┌─────────────────────┐
 │    Host browser     │        │  a small relay │        │   Guest browsers    │
 │                     │        │                │        │                     │
 │  • your real files  │ ◀────▶│  passes bytes │ ◀────▶ │  • view + edit      │
 │  • reads them       │        │  through,      │        │  • chat + draw      │
 │    straight off     │        │  stores        │        │  • any modern       │
 │    the disk         │        │  NOTHING       │        │    browser          │
 │  • saves edits      │        │                │        │                     │
 │    back to disk     │        │                │        │                     │
 └─────────────────────┘        └────────────────┘        └─────────────────────┘
```

- The **host's browser** reads files directly from the host's computer and writes every edit straight back to it.
- The **relay** forwards traffic between host and guests, storing nothing along the way.
- When the host closes the pier, guest access ends immediately - and since nothing was ever copied anywhere, there's nothing left to clean up.

---

## 🚀 Getting Started

The fastest way to use PierPulse is the hosted app - no installation required.

1. Go to **[pierpulse.com](https://pierpulse.com)**
2. Click **Host** and select the folder(s) or drive(s) you want to share
3. Send the generated invite link to your collaborators
4. They open the link - that's the entire setup

**Good to know:**

| Role | Requirement |
|------|-------------|
| **Host** | Desktop **Chrome**, **Edge**, or **Opera** (Chromium-based browsers support direct, sandboxed read/write access to local files via the File System Access API) |
| **Guest** | Any modern browser - desktop or mobile |

---

## 📁 Supported File Types

| Type | Capability |
|------|------------|
| Folders & general files | Browse, download, discuss |
| Images | View inline |
| PDF | View, annotate live, reorder/rotate/delete/extract/merge pages, export |
| Word (`.docx`) | View and edit collaboratively |
| Excel (`.xlsx`) | View and edit collaboratively |
| PowerPoint (`.pptx`) | View and edit collaboratively |

More formats are on the way - see the [Roadmap](#-roadmap).

---

## 🌐 Browser Compatibility

Hosting requires a browser with support for direct local file system access:

- ✅ Google Chrome (desktop)
- ✅ Microsoft Edge (desktop)
- ✅ Opera (desktop)

Guests can join a session from virtually any modern browser, on desktop or mobile, with no special requirements.

---

## 🔒 Privacy & Security Model

- **No cloud storage.** Files are never copied to or persisted on any server.
- **No accounts.** There's nothing to sign up for and nothing tied to an identity.
- **Host-controlled access.** The host decides who can view and who can edit; permissions can be revoked at any time by closing the pier.
- **Ephemeral by design.** The relay only forwards data in transit - it retains no copy of anything that passes through it. Once a session ends, there's no residual data to secure or delete.

---

## ❓ FAQ

**So where do my files actually go?**
Nowhere. That's the entire point. Files are read from the host's disk, streamed through the relay to guests' screens, and any edits are saved back to the host's disk. Nothing is stored on a server along the way. Once the session ends, the files exist only on the host's computer, exactly as before.

**What happens when the host goes offline?**
The pier closes immediately, and guests lose access - there's no copy of the files anywhere else to fall back on. A new session can be opened at any time.

**Can guests edit my files?**
Only if you explicitly grant edit permission. The host always stays in control of who can view and who can change things.

**Do I need an account?**
No. No sign-up, no login, no profile - just open the site and start.

**Is it free?**
Yes, PierPulse is currently free to use.

**Which files can we work on together?**
Folders, images, PDFs, and Microsoft Office documents (Word, Excel, PowerPoint), with more formats planned.

---

## 🗺️ Roadmap

- [ ] Additional supported file formats
- [ ] Richer in-browser editing capabilities

Have a feature request? Open an issue to discuss it.

---

## 📜 License

Released under the **MIT License**. See [`LICENSE`](./LICENSE) for full details.

---

<div align="center">

*PierPulse - the heartbeat of your workspace.*

[pierpulse.com](https://pierpulse.com)

</div>
