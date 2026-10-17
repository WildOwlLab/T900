# Project T900

**Give AI the right context, not all your context.**

Project T900 prepares what you give ChatGPT, Claude or Gemini. Its T900 Engine keeps what is
relevant to your task, leaves out repetition and noise, flags statements that contradict each other,
and shows you everything before you send it. It runs on your device and never sends
anything for you. The engine selects and orders your own text: it is not an AI model, and it never
writes anything.

This repository holds the downloads. The website is [t900.si](https://t900.si); the source code is
not public.

## Download

The latest version is v0.20.3: get it from
[Releases](https://github.com/WildOwlLab/t900/releases/latest).

| For | File |
| --- | --- |
| Chrome, Edge, Brave or Arc (extension) | `project-t900-extension-v0.20.3.zip` |
| Firefox 140 or newer (extension) | `project-t900-extension-firefox-v0.20.3.zip` |
| Mac with Apple silicon (M1 or later) | `Project-T900-0.20.3-mac-arm64.dmg` |
| Mac with an Intel processor | `Project-T900-0.20.3-mac-x64.dmg` |
| Windows 10 or 11 | `Project-T900-0.20.3-windows-x64-setup.exe` |
| Debian or Ubuntu | `Project-T900-0.20.3-linux-amd64.deb` |

## Install

**Extension in Chrome, Edge, Brave or Arc:** unzip `project-t900-extension-v0.20.3.zip` into a folder you
will keep, open `chrome://extensions`, turn on **Developer mode**, click **Load unpacked** and pick
that folder.

**Extension in Firefox:** open `about:debugging#/runtime/this-firefox`, click **Load Temporary
Add-on** and pick `project-t900-extension-firefox-v0.20.3.zip`. Firefox removes it when it restarts, so export
your library first (Settings, Export all data as JSON) and load it again after a restart.

**Desktop app:** the installers are not signed with a developer certificate, so the first launch
takes one extra step. Mac: drag Project T900 into Applications, open it once, then click **Open
Anyway** under System Settings → Privacy & Security. Windows: if SmartScreen stops the setup, click
**More info**, then **Run anyway**. Debian or Ubuntu:
`sudo apt install ./Project-T900-0.20.3-linux-amd64.deb`. Installing over an older version keeps
your library.

## Simple, or Nerd mode

Project T900 starts simple: say what the AI should do, add your notes if you have any, and copy the
pack, or let the extension put it in the AI's prompt box. Turn on **Nerd mode** in Settings for the
advanced options and details, such as optimization modes, word budgets, scores and token estimates.

## Privacy

No account, no servers, no analytics. Your library stays on your device and Project T900 makes no
network requests of its own. Nothing goes into an AI site's prompt box until you click Prepare
current prompt, nothing is copied until you click Copy, and it never presses Send. The full privacy
policy is in [PRIVACY.md](PRIVACY.md), and at [t900.si/privacy](https://t900.si/privacy/).

## License

Project T900 is free to use, and it is not open source: you may not copy, change, resell or unpack it.
The terms are in [LICENSE.md](LICENSE.md). The open-source software and models it includes keep
their own licences, listed in Project T900 under Settings → Open-source notices.

## Contact

Questions, problems or ideas: contact@t900.si
