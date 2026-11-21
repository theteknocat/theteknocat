# How I work with AI

TL;DR: I build software, websites and web apps using AI coding tools. I say so openly and I don't treat the results as trustworthy until I've thoroughly tested, reviewed and gone through every aspect I can think of that matters. This page explains how, so each project's README doesn't have to.
## What I use

- **[Claude Code](https://claude.com/claude-code)** (Anthropic's AI coding tool) writes most of the code in my recent projects.
- **The [ponytail](https://github.com/DietrichGebert/ponytail) plugin** pushes it toward the smallest change that works, so the code stays short and doesn't fill up with extras nobody asked for.
## How I work

I've been working with AI coding tools since Copilot was nothing more than better autocomplete and could attempt to write out whole functions as you typed. It took a long time before I trusted anything an AI wrote and started allowing it to do commits and PRs.

I still don't fully trust it, so my global CLAUDE.md includes rules to make it perform different roles in specific ways based on what I ask. It must declare the mode (research, implement, etc) as well as things like **CONFIRMED**, **INFERRED**, **UNKNOWN** next to information it provides.

1. **I decide exactly what the app or website should do and how it should look and feel.**
   I use Claude to work through that, help with the decisions and write the documentation. I never used to write down any plans or documentation, because that part's slow and boring, so this has been a huge improvement in the way I work. Sometimes I have Claude make me a tracking artifact so it's easier to review the backlog.
2. **I work through building it one piece at a time iteratively.**
   I describe a feature, look at the result, use it, provide feedback, and repeat. Details like layout, wording and behaviour are my calls, and I change a lot of them after seeing them. One thing I've learned is that the initial thing Claude builds can look very impressive, but things fall apart very quickly. That's the case with any very early version of something, but AI tools can fool you by making it look pretty from the get-go.
3. **I test each piece on real data and real devices, or as close to that as possible.**
   If it's an app, I'm testing it on my devices, using my actual system and any real devices it needs to connect to. For websites and web apps, I test against a copy of the real target environment and, where possible, using real content or data. The only catch, of course, is when it's not in production yet and there's no real content or data available.
4. **I do my best to keep decisions documented and in the repo.**
   I'm not always perfect with this; sometimes I turn a plan into a functionality reference that only covers what the app does in the end. However, in cases where it might look like a feature or function is missing that either a human or an AI agent might pick up on, that gets documented clearly as "do not build" and the reasons for it.

## What I can't judge

My background and expertise is all in web using a LAMP stack, but with AI tools I've been able to expand to other languages and build things like desktop apps for Linux without going through an extensive learning curve. As such, when working with Rust or Python, for example, I can't necessarily tell good code from merely working code. I'm up front about that and welcome feedback and criticism so I can learn and improve in those weaker areas.

To that end, here's what I do:

- keep the code small (see ponytail above) so there is less to go wrong
- have automated tests for the risky parts
- use linters set up with the standards for the language or framework (sometimes only in my IDE, not committed to the repo), and rely on them where I can't judge the code myself
- run a full code audit before publishing and fix what it finds (it's AI reviewing AI, so it helps but isn't a substitute for a human reviewer)
- apply my existing general knowledge of what's important in terms of security, application and code architecture, UI/UX and so on to mitigate risks
- follow smart people on YouTube, like other developers and engineers, as well as others in the field, to stay on top of best practices and learn how to be a better developer in general
- ask Claude lots of questions during the process about things to consider, have it search the web, do my own web searches, and make sure all aspects are covered
- question anything Claude code suggests or creates that I didn't ask for, to understand why it chose to do that and whether or not it should be kept
## What I don't do

- I don't pretend AI-written code is hand-written.
- I don't open AI-written pull requests or issues on other people's projects unless I know it's OK to do so and approved by them.
- I follow the AI rules of any platform I publish on. If that means I have to do some parts by hand, so be it, or I avoid publishing on it if I can't.
## On each project

Projects that are AI-written, in whole or in part, say so near the top of their README and link here. I'm still updating them, so if you find one that doesn't, please let me know. If something in a project looks wrong, or you'd like to know how a particular part was made, please open an issue and ask.
## Why I do it

I've been writing code since I was a teenager, making games in Basic on an Atari ST. I love learning new things and the challenges that go with them. Once I've got something mastered, though, writing the code by hand every time gets rather boring. What I like is figuring out how to solve the problem, getting to the end result, and seeing it work, whether I'm the one using it or other people are.

I also want to do more than I have the time or specific knowledge for, like working in a language I'm not familiar with yet. My day job doesn't give me many chances to try the things I'd love to do, and clients rarely have the budget for them. AI tools have let me seriously level up. I can do things I'm a lot slower at doing manually, and build things I otherwise wouldn't have, because I didn't know where to start or didn't have the time to learn it from scratch.

Being AUDHD means I get lots of ideas and want to do lots of things, but I either never get started or can't finish. It also means I'm not good at planning and organising myself, or at writing clearly and concisely. I get there eventually, but it takes time and I stumble along the way. AI helps me plan, write things down and keep track of what I've decided, and it does much of the typing, so more of my ideas actually get built.

It doesn't replace my judgement, though. It handles the parts that used to slow me down or stop me, and I still decide what gets built, how it should work and whether it's any good. Nothing goes public or gets a release if it looks or feels like slop to me. I hold the end result to a standard, even when I can't judge every line underneath it.