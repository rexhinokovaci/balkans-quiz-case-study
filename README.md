# Balkans Quiz: case study

**Trivia about the countries of the Balkans and the wider region**, shipped as a family of per-country apps with Apple Watch and home-screen widgets.

[Website](https://balkansquiz.pages.dev) · Platforms: iOS · watchOS · widgets · web · Cloudflare Workers

> Source code is private. This repo documents what was built and how. Ask for a live walkthrough of the real codebase.

## What I built

- **One codebase, many apps.** Each country (Albania, Kosovo, Greece, Serbia, Croatia, Bosnia, Montenegro, North Macedonia, Bulgaria, Romania, Moldova, Slovenia, Turkey) ships as its own branded app.
- **Apple Watch app and widgets** for each country, for quick daily questions.
- **Automated question pipeline.** New questions are generated on a schedule, checked for quality, and published to the edge.
- **A web version** on Cloudflare Pages.

## Results

- Launching a new country means configuration and a store listing, not a new app.
- The question bank grows automatically without manual work.

## Read more

- [Architecture and key decisions](docs/architecture.md)
- [Delivery pipeline and stack](docs/engineering.md)

---

**Want something like this built for your business?** I build mobile apps, web apps and AI products end to end. [Email me about your project](mailto:kovacirexhino@gmail.com?subject=Project%20inquiry) · [Full profile](https://github.com/rexhinokovaci)
