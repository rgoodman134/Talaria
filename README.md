# Talaria
A lightweight, portable application designed for system administrators and IT professionals that provides a central place to store, organise, and reliably execute existing scripts without replacing established scripting workflows. Its goal is to make commonly used administrative scripts easy to find and safe to run when required.


Overview
========
Talaria is a lightweight, portable application designed for system administrators and IT professionals who maintain collections of small, purpose‑built scripts that are executed manually as needed.
It provides a central place to store, organise, and reliably execute existing scripts without replacing established scripting workflows. Talaria does not generate scripts and does not enforce automation. Its goal is to make commonly used administrative scripts easy to find and safe to run when required.
Talaria is intentionally manual‑first, ensuring that execution always happens with clear human intent.


What Talaria Is
===============
Talaria is a script repository and execution utility.
Scripts are authored and maintained outside the application using your existing tools. Talaria focuses on organisation, discoverability, and execution.

If you've ever thought: “I know I wrote a script for this somewhere…” - Talaria is designed for you.


What Talaria Is Not
===================
Talaria does not:

- Create or edit scripts
- Replace orchestration or configuration management systems
- Automatically schedule or trigger scripts
- Enforce a scripting language or runtime
- Perform unattended or background execution


Key Features
============

- Centralised storage for administrative scripts
- Manual, user‑initiated execution only
- Script‑agnostic design
- Execution via the operating system shell
- Captured output displayed within the application
- Desktop‑focused user experience for day‑to‑day operations work


Setup And Usage Instructions
============================

REQUIREMENTS
  Windows: Windows 10 or later (x64)
  macOS:   macOS 12 or later (Intel or Apple Silicon)

FIRST TIME SETUP
  1. Copy the Talaria folder to your USB stick
     (or run directly from the USB)

  2. Launch Talaria.exe (Windows) or Talaria (macOS)

  3. Click the ⚙ Settings button in the top right

  4. Under Script Folder, click Browse and select
     the Scripts folder on your USB stick

  5. Enable Portable Mode so the drive letter updates
     automatically when the USB is used on different
     machines

  6. Click Save Settings

  7. Close Settings — your scripts will now appear
     in the sidebar

SCRIPT ORGANISATION
  Talaria organises scripts using your existing folder 
  structure rather than imposing a custom database or 
  tagging system. The sidebar mirrors your configured 
  scripts directory directly, allowing you to group 
  tools naturally by environment, platform, role, or 
  workflow. Talaria automatically discovers and 
  indexes scripts up to two subfolder levels deep, 
  helping keep repositories structured and easy to 
  navigate without requiring additional configuration.

PORTABLE MODE
  When enabled, Talaria automatically adjusts the
  scripts folder path to match whichever drive letter
  or volume name the USB stick is assigned on the
  current machine.

  Windows: drive letter is updated automatically
  macOS:   for best results, name your USB stick
           with a unique label (e.g. TALARIA)

RUNNING SCRIPTS
  • Click a script in the sidebar to select it
  • Press Run or use the dropdown for elevated modes
  • F5 to run, Escape to cancel

SHELL SCRIPTS (.sh .zsh .fish) ON WINDOWS
  These require an intermediary shell such as MSYS2
  or WSL. Install one and configure it under
  Settings → Shell Integration

KEYBOARD SHORTCUTS
  F5          Run / Cancel
  Ctrl+F      Focus search
  Ctrl+L      Clear console
  Ctrl+S      Save argument template
  Ctrl+P      Toggle properties panel
  Ctrl+1-4    Switch sidebar tabs
  Escape      Cancel run / clear search

LOGS
  Run logs are saved to a Logs folder inside your
  scripts directory. One log file per script,
  each run is appended.

SUPPORT
  Settings can be exported and imported via
  Settings → Configuration for easy backup
  and transfer between machines.


Execution Model
===============
Scripts are launched via the host operating system shell.
Standard output and execution feedback are captured by the application process and displayed to the user.
Talaria does not alter script contents and does not inject logic beyond execution control.


Supported Scripting Languages
=============================
Currently, Talaria supports 14 scripting languages, including:

.bat, .ps1, .cmd, .vbs, .py, .sh, .zsh, .wsf, .js, .rb, .pl, .php, .fish, .lua


Themes
======
Talaria includes Light, Dark, and System theme options, selectable
under Settings → Appearance. The System option follows your operating
system's current theme preference automatically. Your chosen theme
persists between sessions.


Distribution
============
Talaria is distributed as a prebuilt portable application.

Installation packages will be made available through official Bliitzscript
distribution channels. Detailed installation instructions will be provided
once public releases are announced.


Security and Safety
===================
All executions are explicitly triggered by the user
No automatic or background execution
No remote execution features by default
No modification of scripts at runtime

Talaria is designed to support responsible administrative workflows where control and visibility are essential.


Licensing
=========
Talaria is closed‑source software distributed under a dual‑license model:


Personal, Educational, and Non‑Commercial Use
=============================================

Talaria Personal Use License
Copyright (c) 2026 Bliitzscript
Permission is granted to any individual or organization to use, copy, and distribute this software for personal, educational, or non‑commercial purposes only.
Commercial use is strictly prohibited without prior written permission from Bliitzscript.
Commercial use includes, but is not limited to:

Selling the software, 
Bundling the software with paid products or services, 
Using the software within a commercial business environment, 
Enterprise or organizational deployment for financial benefit, 
Monetized redistribution

You may not:

Resell this software, 
Claim authorship of this software, 
Remove license or copyright notices

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND.

---------------------------------------------

Commercial Use
==============
Talaria Commercial License Agreement
Version 1.0
Copyright (c) 2026 Bliitzscript
Commercial use requires a separate license agreement.
The commercial license grants the right to:

Use Talaria in business or enterprise environments, 
Use Talaria in revenue‑generating activities, 
Deploy Talaria internally within an organization, 

Restrictions apply. Redistribution, resale, sublicensing, reverse engineering, and removal of branding or license notices are prohibited.
Support, updates, and maintenance are not guaranteed unless explicitly agreed in writing.
For commercial licensing inquiries, contact:
Bliitzscript.Commercial

Ownership
Talaria is licensed, not sold.
All intellectual property rights remain with Bliitzscript.

Status
Talaria is actively developed.
Features, platform support, and licensing terms may evolve over time.
