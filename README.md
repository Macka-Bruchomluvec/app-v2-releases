# Vellumancy — downloads

This repository holds the **downloads only**. The source is developed privately.

This is an early build shared with a handful of friends. Expect rough edges.

## Before you install

- **Windows 10 or 11, 64-bit.**
- **Your own Claude account.** The app does not come with AI access: it drives
  [Claude Code](https://claude.ai/code) signed in as *you*, so you need a Claude
  Pro or Max subscription. The installer sets Claude Code up if you do not have
  it, and the app walks you through signing in on first launch.
- **About 1 GB of disk** for the app. The optional Office document editor is a
  separate ~930 MB download you can start later from inside the app.

## Install

Open **PowerShell** and paste one line:

```powershell
irm https://github.com/Macka-Bruchomluvec/app-v2-releases/releases/latest/download/install.ps1 | iex
```

That installs Claude Code if it is missing, then installs Vellumancy and puts it
in your Start menu.

Prefer to do it by hand? Download `Vellumancy-Setup-<version>.exe` from
[the latest release](../../releases/latest) and run it.

**Windows will warn you.** The installer is not code-signed, so SmartScreen says
*"Windows protected your PC"*. Click **More info → Run anyway**. It installs for
your user only, no admin rights needed.

## First launch

1. Pick a **home folder** (suggested: `Documents\Vellumancy`). Your notes, to-do
   list and vault live there — an existing folder is fine, nothing is overwritten.
2. **Sign in to Claude** when the app asks. It opens a terminal, you log in in
   your browser, and the app confirms.
3. A short setup interview follows — answer it or skip it.

## What it does on your machine

The app runs AI agents locally. By default a run is **read-only**; runs you
explicitly give write permission to can create and edit files inside the home
folder you chose, and use a shell fenced to that folder. Nothing is sent
anywhere except to Anthropic, through your own Claude account. There is no
telemetry and nothing reports back to me.

## Updates

The app checks this repository for new versions and updates itself (⚙ Settings →
**App updates** to change that). Your notes, vault and settings are kept.

## Known limitations

- Windows only, x64 only.
- The installer is unsigned (see the SmartScreen note above).
- The Office document editor is an optional extra download and is the newest,
  least-tested part.
- Early build: bugs, half-finished corners and changing UI are expected.

## Feedback

Open an issue here, or just tell me directly. Crashes, confusing moments and
"why does it do that" are all useful — say what you clicked and what happened.

Please don't redistribute the installer; this build is shared privately.
