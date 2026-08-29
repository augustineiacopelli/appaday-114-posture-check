# AppADay #114: Posture Check

A background reminder app that nudges you to check your posture and stretch at a set interval, tracks a daily streak, and shows a rotating tip each time it fires.

Part of [AppADay](https://augustineiacopelli.github.io/appaday/), a project to design, build, and publish one complete web app every day.

## What it does

Pick a reminder interval (20, 30, 45, 60, 90 minutes, or a custom value), and Posture Check will nudge you on that schedule with a short posture or stretch tip. Acknowledge a reminder to log it toward your daily streak and total check count, or snooze it five minutes if the timing is bad. If the tab is in the background and notification permission is granted, you also get a system notification alongside the in-tab card.

## Features

- Interval presets from 20 to 90 minutes, plus a custom minute input
- Optional sound (Web Audio tone) and vibration alerts
- System notifications when the tab is unfocused and permission is granted
- Streak tracking with same-day, consecutive-day, and broken-streak logic
- Catch-up check on page load if a reminder was due while the tab was closed
- Ten rotating posture and stretch tips with no immediate repeats
- All state saved locally, nothing leaves your browser

## Tech

Single HTML file. No frameworks, no build step, no external dependencies beyond Google Fonts. State persists in localStorage. Built to work down to a 375px mobile viewport with 44px minimum tap targets and no horizontal scroll.

## Live app

https://augustineiacopelli.github.io/appaday-114-posture-check/
