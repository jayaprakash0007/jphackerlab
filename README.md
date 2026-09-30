# CyberOps — Terminal Escape

A browser-based cybersecurity terminal game. The current MVP includes:

- 8 sequential Linux and Docker objectives
- a safe simulated terminal (no system commands are executed)
- 10-minute countdown, 3 lives, score, XP, streak bonuses, and hints
- mission success/failure states
- a responsive hacker-style interface
- a device-local leaderboard using browser storage

## Run locally

Open `dist/index.html` in a modern browser. No installation or build step is required.

For a local web server, run this command from the project directory:

```powershell
python -m http.server 8080 --directory dist
```

Then visit `http://localhost:8080`.

## Important architecture note

This first version simulates terminal commands in the browser. It does not execute commands on the player's machine or connect to Docker. A later production version can run isolated, disposable containers behind a server API.

