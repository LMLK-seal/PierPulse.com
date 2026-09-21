# PierPulse.com

> **Your computer is the cloud.**
> Browse, discuss, and edit files together with anyone - right in the browser.
> No uploads. No cloud storage. No accounts.

[![Website](https://img.shields.io/website?url=https%3A%2F%2Fpierpulse.com)](https://pierpulse.com)
![Cloud storage](https://img.shields.io/badge/cloud_storage-none-success)
![Single file app](https://img.shields.io/badge/app-a%20single%20HTML%20file-orange)
![Accounts](https://img.shields.io/badge/accounts-not%20needed-blue)

![PierPulse in light mode](https://github.com/LMLK-seal/PierPulse.com/blob/main/Screenshot.png?raw=true)

---

## What is PierPulse? 

PierPulse lets other people **see and work on the files on your computer**, from their own browser, anywhere in the world. No uploading, no syncing, no "I'll email you the latest version."

The whole idea fits in four steps:

1. **You host.** Open [pierpulse.com](https://pierpulse.com), pick the folders (or whole drives) you want to share, and a "pier" opens for your session.
2. **You invite.** Send the session link to your crew - coworkers, clients, friends.
3. **They dock.** Guests open the link in any browser. Nothing to install, no account to create.
4. **You work together.** Everyone browses the same files at the same time, edits documents together, and talks it over in the chat sidebar.

The important part: **your files never leave your computer.** They are not copied to Google Drive, Dropbox, or any server. While the pier is open, PierPulse streams your files straight from your machine to your guests. When you close it, your files exist in exactly one place — yours.

Think of it like letting a friend look over your shoulder at your screen, except they can be on another continent, and you can both point at the same spreadsheet and argue about cell B7 in real time.

---

## Features

### One file browser, shared live

Everyone in the session sees the same folder at the same time. You can feel the room: a quiet "3 people are viewing this folder" presence line, typing indicators in chat, and one-click jumps - mention a file in chat and everyone can fly straight to it. If you'd rather tour than wander, **Follow mode** lets one person drive while the rest ride along, with the option to hand the wheel over at any time.

### A chat that lives next to your files

The sidebar is scoped to wherever you are - the conversation in `Invoices` stays in `Invoices`. React to messages, send voice notes when typing is too slow, and paste screenshots you can annotate with a quick markup tool before sending. Need to decide something? Fire a quick poll, and the result lands in a **decision log** so it doesn't get lost in the scroll. A **pinned-files shelf** keeps the important stuff one click away.

### PDFs, reviewed together

Open a PDF with your crew and page turns stay in sync - nobody is ever "wait, which page are you on?" Draw on it live, with everyone's ink in their own color. Need surgery instead of comments? The page toolkit reorders, rotates, deletes, extracts, and merges pages. Export with the ink burned in when you're done.

### Office files, no Office needed

Open, view, **and edit** Word (`.docx`), Excel (`.xlsx`), and PowerPoint (`.pptx`) files directly in the browser. When you save, the edited file goes right back onto the host's drive - the original, in place. No exports, no downloads, no `final_v7_REAL_this_time.docx`.

### Dock every drive you own

**Multi-Drive Docking** lets the host dock several drives or folders at once - `C:`, `D:`, `F:`, an external disk — and the whole crew moves between them like ordinary folders. Your entire computer becomes one shared workspace.

### Never miss a thing

Late to the session? **Catch-me-up replay** shows you what was opened, said, and decided while you were away. It's the meeting minutes nobody had to write.

---

## How it works (the 60-second version)

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

- The host's browser reads files directly from the host computer, and saves every edit back to it.
- The relay is a hallway, not a warehouse: it forwards traffic between host and guests and keeps nothing.
- When the host closes the pier, guest access ends — and since nothing was ever copied anywhere, there is nothing to clean up.

---

## Getting started

**Use the hosted app (easiest):**

1. Go to <https://pierpulse.com>
2. Click **Host** and choose the folder or drives you want to share
3. Send the invite link to your crew
4. They open it. That's the whole setup.

**Good to know:**

- **Hosting** works in desktop Chrome, Edge, or Opera (they support direct, safe read/write access to local files).
- **Guests** can join from any modern browser - desktop or phone.

---

## FAQ

**"So where do my files actually go?"**
Nowhere. That is the entire point. Files are read from the host's disk, streamed through the relay to your guests' screens, and edited versions are saved back to the host's disk. Nothing is stored on any server along the way. When the session ends, the files exist only on the host's computer - same as before it started.

**"What happens when the host goes offline?"**
The pier closes. Guests lose access immediately, because there is no copy of the files anywhere else to fall back on. Reopen a session whenever you like.

**"Can guests edit my files?"**
Only if you grant edit permission - you stay in control of who can view and who can change things.

**"Do I need an account?"**
No. No sign-up, no login, no profile. Open the site and start.

**"Is it free?"**
Right now, yes - PierPulse is completely free to use.

**"Which files can we work on together?"**
Folders, images, PDFs, and Microsoft Office documents (Word, Excel, PowerPoint). More formats are on the way.

---

## Roadmap

- More file formats and richer in-browser editing

---

## License

MIT license
---

*PierPulse - the heartbeat of your workspace.*
