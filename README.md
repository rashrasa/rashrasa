# Ahmed Rashrash

*Check pinned projects for images/gifs*

### Hello there!

I'm a Software Engineering student at McMaster University with a wide breadth of interests, including:

- ️🎨 3D Graphics
- 🖥️ Backend Development
- ⏳ Realtime Systems
- 🛜 Networking Protocols
- 🏙️ Distributed Systems
- 🎛️ Signals and Control Systems

## Personal Projects

### [Rover](https://github.com/rashrasa/rover)

A WebGPU + Rust native application meant for exploring graphics rendering and physics.

### [Mini-Redis](https://github.com/rashrasa/mini-redis-rs)

A server hosted over TCP which has in-memory JSON storage + persistence.

### [Blind-Maze](https://github.com/rashrasa/blind-maze)

Game allowing multiple connections to a dedicated, authoritative server written in Go, serving clients using Next.js. Implemented state synchronization, simple particles, and collisions.

## Current Position

I currently work at Quasar Consulting Group as part of the Automation Team. I've been working part-time during Fall/Winter terms and full-time in the Summer term since July 2024.

### Highlights

### Offline-First Flutter App ![Static Badge](https://img.shields.io/badge/Flutter-blue) ![Static Badge](https://img.shields.io/badge/Supabase-darkgreen) ![Static Badge](https://img.shields.io/badge/RxDart-blue) ![Static Badge](https://img.shields.io/badge/Riverpod-blue) ![Static Badge](https://img.shields.io/badge/Brick-red)

- Designed and developed an offline image processing pipeline that enables users to work in areas with low connectivity. Uses **RxDart** to merge remote and local data.
- Implemented **Riverpod** state management to reduce frequent and unnecessary UI re-builds
- Designed an async request queue (rate-limiter) for image uploads/downloads

### C# Desktop Application for Word Processing ![Static Badge](https://img.shields.io/badge/C%23-purple) ![Static Badge](https://img.shields.io/badge/.NET%209.0-purple) ![Static Badge](https://img.shields.io/badge/WinUI%203-blue) ![Static Badge](https://img.shields.io/badge/OpenXML-orange)

- Multi-threading to speed up slow tasks like using Word interop to process documents. Thread safety by using semaphores, locks, concurrency-safe collections.
- Caching results of heavy calculations _(such as calculating page numbers which requires rendering the word document in the background)_ on Word documents that don't tend to change frequently to avoid doing unnecessary work
- Project-scoping, inspired by VS Code, where any user can open a project and be back where they (or someone else) left off

### AI Experience

I've used multiple coding agents and understand when they go from being a useful tool to a potential problem to a codebase. I've been able to prevent bugs that agents attempted to introduce, such as:

- Inconsistent widget states (flutter) resulting from improper use of Riverpod providers
- Duplicated sources of truth (and redundancy in general), and many more, before they were introduced to a codebase.
- Race conditions, deadlocks (C#)

I've had the best results come from Claude Opus and Sonnet inside of Claude Code.

## Github Analytics

![](https://github-readme-stats.vercel.app/api/top-langs/?username=rashrasa&theme=dark&hide_border=true&include_all_commits=true&count_private=false&exclude_repo=rustlings&langs_count=6)

## AI Notice

All commits on public, personal repositories are posted without the use of integrated AI coding agents, unless explicitly mentioned in the root README.md of the repository. No code is ever copy pasted from AI.

I've used ChatGPT infrequently while working on multiple projects to identify sources of bugs and errors. This is after spending much time throwing around print/log statements everywhere and pinpointing the lines of code where the issue is occurring (which is often enough on its own).
