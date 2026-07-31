# Ahmed Rashrash

*Check pinned projects for images/gifs*

### Hello there!

I'm a Software Engineering student at McMaster University with a wide breadth of interests, including:

- ️🎨 3D Graphics
- 🖥️ Backend Development
- ⏳ Realtime Systems
- 🏙️ Distributed Systems
- 🎛️ Signals and Control Systems

## Personal Projects

### [Agate Engine](https://github.com/rashrasa/agate_engine)

Game engine implemented in Rust using WebGPU. Includes model and texture loading, a gravity system, world boundary, and a free camera. 

https://github.com/user-attachments/assets/645711d6-bb88-4bcd-bb98-247cc32211e9

### [Gradient](https://github.com/rashrasa/gradient)

A NextJS-based learning platform for STEM topics. Created a simulation for decomposing audio signals into their frequency components using the Fast Fourier Transform (and its inverse). Created a WASM module in Rust for heavy computations. Implemented a Docker-based development environment with hot-rebuilds for the WASM module to complement NextJS's hot-reloads.

https://github.com/user-attachments/assets/3fc98ed4-b295-4f85-bc88-089534c0a463

### [Concurrent Queue](https://github.com/rashrasa/mpmc_rs)

An unbounded Multi-Producer, Multi-Consumer channel, a benchmarking engine, and a highly optimized aggregator. Implemented in Rust using different techniques. Benchmarked against `crossbeam`. 

![](https://github.com/rashrasa/mpmc_rs/blob/main/bench/docs/assets/summary_scalability.jpg)

## Current Position

I currently work at Quasar Consulting Group as part of the Automation Team. I've been working part-time during Fall/Winter terms and full-time in the Summer term since July 2024.

### Highlights

### Offline-First Flutter App ![Static Badge](https://img.shields.io/badge/Flutter-blue) ![Static Badge](https://img.shields.io/badge/Supabase-darkgreen) ![Static Badge](https://img.shields.io/badge/RxDart-blue) ![Static Badge](https://img.shields.io/badge/Riverpod-blue) ![Static Badge](https://img.shields.io/badge/Brick-red)

- Designed and developed an offline image processing pipeline that enables users to work in areas with low connectivity. Uses **RxDart** to merge remote and local data.
- Implemented **Riverpod** state management to reduce frequent and unnecessary UI re-builds
- Designed an async request queue (rate-limiter) for image uploads/downloads

### C# Desktop Application for Word Processing ![Static Badge](https://img.shields.io/badge/C%23-purple) ![Static Badge](https://img.shields.io/badge/.NET%209.0-purple) ![Static Badge](https://img.shields.io/badge/WinUI%203-blue) ![Static Badge](https://img.shields.io/badge/OpenXML-orange)

- Multi-threading to speed up slow tasks like using Word interop to process documents
- Caching results of heavy calculations _(such as calculating page numbers which requires rendering the word document in the background)_ on Word documents, for which the results don't tend to change frequently, to avoid doing unnecessary work
- Project-scoping, inspired by VS Code, where any user can open a project and be back where they (or someone else) left off

### AI Experience

I acknowledge the benefit that AI agents can bring when used appropriately and have personally boosted my productivity at my current role significantly by using them. Specifically:

- I've minimized code turnover rate by steering clear of short-term band-aid solutions and implementing durable code which rarely needs patching (implemented a Data and Business Logic Layer for the Flutter app). This was done by using my knowledge of common pitfalls during early stages of the app to bias the agent towards a more durable solution.
- I've cut my average bug fixing time to mere minutes for small-medium bugs
- I've discovered root causes of large bugs by prefacing prompts with only the most relevant context up-front and making educated guesses on the root causes to reduce the search space

I also understand when agents can go from being a useful tool to a potential problem to a codebase. I've been able to prevent bugs that agents attempted to introduce, such as:

- Inconsistent widget states (Flutter) resulting from improper use of Riverpod providers
- Duplicated sources of truth (and redundancy in general), before they were introduced to a codebase.
- Race conditions, deadlocks (C#)

Agents commonly implemented flawed or incorrect code when the problem required knowledge on the architecture of the project.

For example, implementing concurrency for the C# app required understanding where synchronization needed to occur in the app, what possible states and transitions existed, and what other tasks the app needed to perform. The agent produced an output which did the job of concurrently calculating page counts of Word documents, saving the result to a cache file, and allowed for cancelling the operation. However, it also blocked the UI thread, failed entirely when an error occurred with any single file, spawned a Word process for every file instead of leveraging Word COM Interop's Document API that allows for multiple open documents, and also closed any pre-opened Word applications.

In that scenario, there was too much context needed to perform the task and the agent didn't have enough examples to draw from (this was a new internal tool). The solution would be to implement a narrow slice of core functionality that the agent can digest, validate it from all angles (correctness, performance, user experience), then use that foundation to expand it with more features. Specifically, it would involve moving the same functionality from a function call into a separate thread, but validating a single-threaded version to isolate any threading issues before expanding to more threads.

AI agents perform well when they have a strong foundation of well-written code, tests, and guidelines to draw knowledge from.

I've had the best results come from Claude Opus and Sonnet inside of Claude Code.

## Github Analytics

![](https://github-readme-stats.vercel.app/api/top-langs/?username=rashrasa&theme=dark&hide_border=true&include_all_commits=true&count_private=false&exclude_repo=rustlings&langs_count=6)

## AI Notice

All commits on public, personal repositories are posted without the use of integrated AI coding agents, unless explicitly mentioned in the root README.md of the repository. No code is ever copy pasted from AI.

I've used ChatGPT and Claude Web infrequently while working on multiple projects to identify sources of bugs and errors. This is after spending much time throwing around print/log statements everywhere and pinpointing the lines of code where the issue is occurring (which is often enough on its own).
