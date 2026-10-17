# Project T900 privacy policy

**Effective:** 16 October 2026 · **Applies to:** Project T900 0.16.0 and later: the web app, the
browser extension and the desktop app; and its website, t900.si · **Published by:** WildOwlLab ·
**Contact:** contact@t900.si

## In short

- **We receive nothing.** Project T900 has no accounts, no analytics, no crash reporting, no tracking and
  no backend. WildOwlLab never receives your text, files, images, audio or library, or even a count
  of how often you use Project T900.
- **Everything stays on your device,** in Project T900's own storage there.
- **Nothing is sent for you.** Project T900 never sends anything to ChatGPT, Claude, Gemini or any other
  AI provider. You copy or insert a context pack yourself, and you press Send yourself. On first
  use you choose whether one click is enough (it then asks only when a pack holds a secret you
  added back) or whether each pack also needs a tick. In the extension, once you have agreed, a
  pack with something of yours in it goes into the AI site's prompt box as soon as it is ready,
  after you click **Prepare current prompt**; you can turn that off.

## What Project T900 stores, and where

Project T900 stores your library on your device only:

- **What:** your chats (each one's name, and the project it is in, if any), workspaces, projects
  and memories, including what you saved about yourself ("About you"); the context packs you save; your settings; and your optimization history, which
  holds each chat's turns. Your settings include the choice you made about copying, and when you
  made it, and, in the web and desktop app, whether the extension allows this copy to share (so
  that **Delete all local data** reaches the other copy whenever sharing is allowed). History keeps details about each run and the pack you copied, not
  the source text you pasted in, unless you turn on the setting that saves it (it is off by default,
  and another control removes saved source text from history). A chat's turns are your side of the
  conversation only: Project T900 never sees what an AI answers.
- **Where:** in the web app, in your browser's storage for that site; in the extension, in its own
  storage inside your browser; in the desktop app, in its data folder:
  `~/Library/Application Support/com.wildowllab.library` on a Mac,
  `%APPDATA%\com.wildowllab.library` on Windows, `~/.config/com.wildowllab.library` on Linux.
- **Selected text you save:** when you save text you selected on a web page as a memory, the page's
  title and address are saved with it, as where it came from.
- **The desktop app also keeps** its Context Lens settings (whether it is on, and its shortcut).
  Once you set up sharing with the extension, it also keeps a random key that lets only your own
  browser connect, tells each installed browser where to find it (a small file in the browser's
  settings folder, or a registry entry on Windows), and logs connection events, such as when the
  browser connected and why it stopped. The log never contains your library, and it is kept to
  about 64 KB. **Stop sharing** removes the key and the browser entries.

Project T900 does **not** keep:

- **Images** you read text from. An image is held in memory while you review its text, then
  dropped; only the text you choose to add is kept.
- **What you type in a chat before you prepare it.** Go to another page and back, and your task
  and notes are still there: they are held in memory for this visit, never written to storage,
  and gone when you reload, close the app, or start the next message.
- **Audio** you dictate in the desktop app. It is held in memory until it has been turned into
  text, then dropped; only the text you keep stays.
- **Text Context Lens reads** from the clipboard. It stays in memory while the lens is open and
  until you choose what to do with it. It is dropped when you cancel or close the lens, or two
  minutes after you choose if the app has not taken it by then. It is never written to disk.
- **Files** you import (PDF, Word, Markdown, text). Project T900 converts them on your device and keeps
  only the text you add to your source context. A PDF whose scanned pages you read is held in
  memory while you review them, each page drawn as a picture only while it is read; the PDF and
  the pictures are then dropped.

Project T900 does not add encryption of its own to what it stores: the data is protected by your device,
your browser and your operating-system account. Anyone who can use your account can open it, so
use a login and, where you can, disk encryption.

## What Project T900 reads, and when

Project T900 works only on what you give it, when you give it:

- **Text, files and images** you paste, choose or drop in.
- **On ChatGPT, Claude and Gemini,** the extension runs a small script on those sites that does
  nothing until you open the Project T900 popup there. To decide what to offer you, the popup asks the
  page only whether any text is selected, yes or no, never what it is. It reads your prompt only
  when you click **Prepare current prompt**, and selected text only when you choose **Use selected
  text as source** or **Save as memory**. It inserts a context pack above your prompt only after you
  click **Prepare current prompt** (as soon as the pack is ready, unless you turned that off, the
  pack holds a secret you added back, which asks first, or it holds nothing of yours) or
  **Insert**. **Take it out** removes
  that pack again, and only that pack, and preparing again replaces it the same way; a pack
  changed in the box is left alone. It never presses Send. Once text is in a site's prompt box,
  that site's own page can read it, even before you send it: that is the site's doing, under its
  own policies.
- **Memory from another AI assistant** reaches Project T900 only when you paste it in. Project
  T900 gives you a prompt to copy into a chat with that assistant, and never contacts the
  assistant itself. What you paste back is read on your device, and only the facts you choose to
  keep are saved, like any other memory.
- **Context Lens** (desktop app) is off until you turn it on. It then reads the clipboard, as plain
  text, only when you press its shortcut or **Try it now**, and shows you exactly what it read.
- **Dictate locally** (desktop app) is off until you turn it on. The microphone is on only while
  the dictation button says it is listening, for at most 30 seconds at a time. The app refuses the
  microphone to anything but that button.

Project T900 never captures your screen, never reads your browsing history, other tabs, your
conversations on AI sites or your keystrokes, never watches the clipboard and never listens in the
background. Its own chats hold only what you prepare in them.

## What leaves your device

**Nothing, by Project T900's doing.** Project T900 makes no network requests except to load its own files:

- The extension enforces this with a Content Security Policy: its pages load nothing from, and
  send nothing to, anywhere but the extension itself, so the browser would refuse anything else.
  The web app sets the same policy in its page, which covers the page but not the background
  workers it starts; the README explains how to send it as a header too.
- The desktop app cancels every web request its window makes, on top of that policy.
- The models Project T900 uses on your device (meaning-based matching, the contradiction check, reading
  text in images and, in the desktop app, speech to text) are files that come with Project T900:
  the extension and the desktop app carry them, and the web app loads them from its own address
  the first time it needs them, never from anyone else.

Your text leaves your device only when **you** send it:

- **When you copy or insert a context pack** into ChatGPT, Claude, Gemini or another AI tool and
  send it, that provider handles it under its own policies. Project T900 cannot see or control what
  happens after that.
- **When you export** your library, the file is saved where you choose, and what happens to it is
  up to you.

Other companies are involved only in getting Project T900 to you:

- **Downloads** come from GitHub, which serves them under its own policies. GitHub shows
  WildOwlLab totals, such as how many times each file was downloaded and how many people viewed
  the download page, and nothing about who they are.
- **The website,** t900.si, is static pages served by Cloudflare. The pages set no cookies, run no
  scripts or analytics, and load nothing from other sites. Like any web host, Cloudflare receives
  each visitor's IP address and browser details to serve the pages and protect them from attacks,
  under its own policies. Cloudflare shows WildOwlLab totals, such as how many pages it served and
  to which countries, and the IP address of any request its security features block or challenge.
  WildOwlLab turns on none of Cloudflare's optional analytics and keeps no record of who visits.
- **If you install from a browser's add-on store,** that store handles installation and updates
  under its own policies.
- **If you use the web app from a hosted address,** the host that serves its files sees ordinary
  requests for them (such as your IP address and browser), as with any website. It never receives
  your library, which stays in your browser.

## Sharing between the web app, the extension and the desktop app

Each part of Project T900 keeps its own library. You can let them share one, on the same computer, with
no network involved. Sharing is off until you turn it on:

- **The extension and the web app** share through the extension. Only the extension's own settings
  page can approve sharing, and only with the addresses it was built for (a released extension:
  the web app served on your own computer at `localhost:7900` or `127.0.0.1:7900`). While sharing
  is on, anything running at an allowed address can read and change your library, also when the
  web app is not what runs there: another program on your computer, or another person's account
  on a computer you share, could serve a page at that address. On such a computer, or when you are
  not using the web app, turn sharing off with **Stop sharing**.
- **The extension and the desktop app** share through native messaging, the browser's own channel
  to a program on the same computer. You set it up in both: **Set up sharing** in the desktop app,
  then **Share with the desktop app** in the extension, which asks for the extra permission to do
  so. The browser starts the desktop app's link only for the Project T900 extension, and the desktop app
  answers only on a local connection that your account alone can open, never on a network port.
- **What is shared:** chats, workspaces, projects, memories, saved packs and history, and
  deletions of them. Settings are not shared, and source text saved in history never leaves the part it was
  saved in.

## Browser extension permissions

The extension asks for as little as it can, and for no access to websites beyond those below:

| Permission | Why |
| --- | --- |
| `activeTab` | To see the address and title of the tab you opened the Project T900 popup on, so it knows whether it can help on that site, and to talk to that tab. Only that tab, only when you open the popup. |
| `storage` | Only its in-memory session area, never written to disk: to hand your prompt or selected text from the popup to the full review page when you choose **Open full review** (cleared as soon as that page reads it), and to remember when to try reconnecting to the desktop app. |
| `alarms` | Only to reconnect to the desktop app while sharing with it is on. |
| `nativeMessaging` (optional) | To share your library with the Project T900 desktop app. The browser asks you for it when you turn on **Share with the desktop app**, and not before. |

Its script on web pages runs only on `chatgpt.com`, `chat.openai.com`, `claude.ai` and
`gemini.google.com`, to read your prompt or selected text when you ask and to insert a context pack
when you ask; and on `localhost` and `127.0.0.1`, to connect to a copy of the web app on your own
computer when you turn on sharing. It asks for no other site access and no permission to read your
tabs, history, bookmarks, cookies, downloads or clipboard.

## Sensitive content

Project T900 looks, on your device, for a few unmistakable kinds of secret: private keys, API keys and
other labelled secrets, passwords, payment card numbers and identity numbers. It flags what it
finds, leaves flagged source text out of packs by default, and keeps memories marked sensitive out
unless you include them. It is not a complete check for secrets or personal information and can
miss things: review what you share.

## Your control

- **Export** everything as a JSON file with **Export all data as JSON**, under **Settings →
  Export and import**, and a chat's memory as a PDF with **Memory → Export PDF** in that chat. The PDF is
  made on your device: the desktop app saves it where you choose, and a browser hands it to its
  own print window, where **Save as PDF** saves it. Nothing is uploaded.
- **Delete** a memory, a chat (with its memory and turns), a project's memories, a project or a
  workspace; use **Delete all optimization history**; or use **Delete all local data** to remove
  everything in that part of Project T900. A turn keeps the pack you copied as it was: deleting a
  memory does not take it out of turns that already carried it. Remove those turns, or delete the
  history, to remove it there too.
- **Uninstalling the extension** deletes its storage with it. **Uninstalling the desktop app**
  leaves its data folder (listed above) in place, so that a reinstall keeps your library; delete
  that folder to remove the library too. If you shared it with the extension, click **Stop
  sharing** in the desktop app before uninstalling it, to remove its entries from your browsers.

WildOwlLab holds no data about you, apart from any email you send us, so there is nothing else for
us to access, correct, export or delete on your behalf. All of it is on your device, under your
control. To have your emails deleted, ask.

## Children

Project T900 is not directed at children and collects no data from anyone, including children.

## Changes to this policy

If what Project T900 stores, reads or sends ever changes, this policy will change first, with a new
effective date, and the release notes for that version will say so.

## Contact

Email contact@t900.si with questions about this policy or about how Project T900
handles your data. Cloudflare, which forwards the domain's mail, passes your message to
WildOwlLab's mailbox, and WildOwlLab uses your address and what you write only to answer you.
