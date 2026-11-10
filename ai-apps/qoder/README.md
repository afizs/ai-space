# Keyform — Mechanical Keyboard Playground

A single-file interactive mechanical keyboard for the browser. Type on your real keyboard or click the keys; every press animates and plays a switch sound synthesized live with the Web Audio API.

<img width="1299" height="981" alt="image" src="https://github.com/user-attachments/assets/1409d595-759f-4fe7-b2b8-1b74c493b53a" />


## Run

Open `index.html` in a modern browser. No install, build step, server, or network access required.

Audio starts on your first keypress or click because of browser autoplay policy. Use the **Sound** button in the header to mute or unmute everything.

## What’s inside

- 87-key ANSI QWERTY layout: function row, number row, modifiers, navigation cluster, and arrows
- Smooth physical key travel on real keystrokes, mouse clicks, and touch taps
- Three synthesized switch voices: **Blue** (clicky), **Red** (linear), **Brown** (tactile)
- Live keycap and case color pickers, volume, key travel, ambient glow, and reset
- Typing area with copy, clear, undo, character count, key-press counter, and rolling 15-second WPM
- Dark responsive UI; small screens scroll or swipe the keyboard horizontally

## Typing notes

- Just start typing; the typing space is focused on load.
- `Tab` inserts a tab. `Esc` moves focus out of the typing space.
- Click `Shift` to latch it for the next character; click `Caps Lock` to toggle caps for virtual typing.
- `Insert` toggles overwrite mode; the navigation keys move the caret.
- Browser shortcuts such as Ctrl/Cmd+C, V, A, and Z are left to the browser and native editor.

## Tech

One HTML file with inline CSS and vanilla JavaScript. No libraries, external fonts, images, or audio files. Key sounds are generated from filtered noise bursts and decaying resonances; wide keys get extra stabilizer rattle. Settings live in memory for the current tab.
