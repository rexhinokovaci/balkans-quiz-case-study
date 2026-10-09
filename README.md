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

## Lessons learned

- **Local beats generic in the stores.** Separate per-country apps give each market its own listing, branding and App Store search presence.
- **Many apps, one codebase.** Per-country configuration keeps a whole family of apps down to one thing to maintain.
- **Design for daily, glanceable use.** Watch apps and widgets in every build give people a reason to come back each day.
- **Automated content needs policy checks.** Questions are generated on a schedule, but checks decide what actually gets published.

## FAQ

### Which countries are covered?

Albania, Kosovo, Greece, Serbia, Croatia, Bosnia, Montenegro, North Macedonia, Bulgaria, Romania, Moldova, Slovenia and Turkey, each as its own branded app.

### Why separate apps instead of one app with a country picker?

Each market gets its own store listing, local branding and search presence, while all apps share one codebase.

### How are new questions created?

A scheduled pipeline generates questions, validates them and publishes accepted ones to the Cloudflare Workers API. Apps and the web version pick them up without an app release.

### Does it work on Apple Watch?

Yes. Every country build includes a watchOS app and home-screen widgets for quick daily questions.

### Can you build a family of localized apps for my business?

Yes. I'm a mobile app developer and DevOps engineer based in Tirana, Albania, building iOS, watchOS and web apps with automated content pipelines for clients across the Balkans and Europe. [Email me about your project](mailto:kovacirexhino@gmail.com?subject=Project%20inquiry).

## Read more

- [Architecture and key decisions](docs/architecture.md)
- [Delivery pipeline and stack](docs/engineering.md)

---

**Want something like this built for your business?** I build mobile apps, web apps and AI products end to end. [Email me about your project](mailto:kovacirexhino@gmail.com?subject=Project%20inquiry) · [Full profile](https://github.com/rexhinokovaci)
