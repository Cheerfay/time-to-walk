# Time to Walk

[English](README.md) | [简体中文](README.zh-CN.md)

**Focus, stand, repeat. Even one second counts.**

[View in the Chrome Web Store](https://chromewebstore.google.com/detail/jcbldmgghanpecpbcmjdhbijjffoackf)  
<sub>The latest release is under review. Chrome Web Store availability varies
by region and may require access to Google services.</sub>

Time to Walk is a lightweight Chrome extension for people who spend long hours
working or studying at a desk. Pomodoro-style focus intervals and fullscreen
reminders build movement into your work rhythm. When a session ends, a
fullscreen page asks you to stand—without streaks to protect or exercise goals
to complete.

站起来，哪怕只有一秒，也算一次胜利。

## Why I built it

Most break reminders are easy to dismiss without noticing. Others turn basic
movement into another system to manage. I wanted a gentler middle ground: a
clear interruption at the right moment, with just enough friction to make the
choice conscious.

## What it does

- 15, 25, 30, 45, or 60-minute focus intervals
- Fullscreen stand-up reminders
- Three-click early dismissal to reduce reflexive skipping
- Automatic close after five minutes, followed by the next focus session
- Optional prompts to get water, stretch, look into the distance, or walk
- Two switchable visual themes
- Friendly English and Chinese copy
- Automatic pause while the device is locked
- Timer recovery after browser interruptions

## Product decisions

- **Movement without performance.** No check-ins, targets, streaks, or exercise
  tracking.
- **Friction with an escape hatch.** Three clicks make early dismissal
  deliberate; the reminder still closes automatically.
- **Local by default.** No account, analytics, or personal data collection.
  Timer state and preferences remain in the browser.
- **Resilient timing.** Persistent deadlines and Chrome alarms keep sessions
  reliable when the extension background process is suspended.

## Technical outline

- Chrome Extension Manifest V3
- Native HTML, CSS, and JavaScript
- `chrome.alarms`, `chrome.storage`, `chrome.windows`, and `chrome.idle`
- Node.js built-in test runner

## Status

The latest bilingual store release is currently under review.

The source code is private. This repository is a public product overview.
