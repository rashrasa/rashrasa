# Ahmed Rashrash

### Hello there! 👋

I'm a Software Engineering student at McMaster University 🏫 with a wide breadth of interests (that I can't keep up with), including:

️🎨 3D Graphics

🖥️ Backend Development

⏳ Realtime Systems

🛜 Networking Protocols

🏙️ Distributed Systems

🎛️ Signals and Control Systems

## Currently Developing

### Blind Maze

[![Blind Maze](https://github-readme-stats.vercel.app/api/pin/?username=rashrasa&repo=blind-maze)](https://github.com/rashrasa/blind-maze)

A full stack multiplayer web game that consists of:

### Server ![Static Badge](https://img.shields.io/badge/Go-cyan)

A basic websocket server written in Go which facilitates communications between clients.

### Client ![Static Badge](https://img.shields.io/badge/Typescript-blue)

A canvas-based component which renders the game, connects to the server, handles inputs and also handles game logic elements such as collisions. Written in typescript.

### Frontend ![Static Badge](https://img.shields.io/badge/HTML-orange) ![Static Badge](https://img.shields.io/badge/Tailwind%20CSS-blue) ![Static Badge](https://img.shields.io/badge/Typescript-blue) ![Static Badge](https://img.shields.io/badge/React-blue) ![Static Badge](https://img.shields.io/badge/Next.js-black)

A Next.js project which features simple anonymous logins and is the main entry point of the app.

## Current Position

I currently work at Quasar Consulting Group as part of the Automation Team. I've been working part-time during Fall/Winter terms and full-time in the Summer term since July 2024.

### What I've Helped Build

### An offline-first, full-stack (CRUD) app ![Static Badge](https://img.shields.io/badge/Flutter-blue) ![Static Badge](https://img.shields.io/badge/Supabase-darkgreen) ![Static Badge](https://img.shields.io/badge/RxDart-blue) ![Static Badge](https://img.shields.io/badge/Riverpod-blue) ![Static Badge](https://img.shields.io/badge/Brick-red)

- Designed and developed an offline image processing pipeline that enables users to work in areas with low connectivity. Uses **RxDart** to merge remote and local data.

- Implemented **Riverpod** state management to reduce frequent and unnecessary UI re-builds

### A desktop app for Microsoft Word processing ![Static Badge](https://img.shields.io/badge/C%23-purple) ![Static Badge](https://img.shields.io/badge/.NET%209.0-purple) ![Static Badge](https://img.shields.io/badge/WinUI%203-blue) ![Static Badge](https://img.shields.io/badge/OpenXML-orange)

- Multi-threading to speed up slow tasks like using Word interop to process documents.

- Caching results of heavy calculations _(such as calculating page numbers which requires rendering the word document in the background)_ on Word documents that don't tend to change frequently to avoid doing unnecessary work

- Thread safety by using semaphores, locks, concurrency-safe collections

- Project-scoping, inspired by VS Code, where any user can open a project and be back where they (or someone else) left off

- User-friendly UI using the Model-View-ViewModel framework and libararies such as CommunityToolkit.MVVM

### AI Experience

I've used multiple coding agents at my current position and understand when they go from being a useful tool to a potential problem to a codebase. I've been able to catch multiple bugs, such as:

- Inconsistent widget states (flutter) resulting from improper use of Riverpod providers
- Duplicated sources of truth (and redundancy in general), and many more, before they were introduced to a codebase.

I've had the best results come from Claude Opus and Sonnet inside of Claude Code.

## Github Analytics

![](https://github-readme-stats.vercel.app/api/top-langs/?username=rashrasa&theme=dark&hide_border=true&include_all_commits=true&count_private=false&exclude_repo=rustlings&langs_count=6)

## AI Notice

All commits on public, personal repositories are posted without the use of integrated AI coding agents, unless explicitly mentioned in the root README.md of the repository. No code is ever copy pasted from AI.

I've used ChatGPT infrequently while working on my blind-maze project to figure out sources of bugs and errors. This is after spending much time throwing around print/log statements everywhere and pinpointing the lines of code where the issue is occurring (which is often enough on its own, without ChatGPT).
