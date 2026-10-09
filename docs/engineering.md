# How it ships

- **Multi-target release.** Each country ships an app, a watch app and widgets, all from shared code with per-country bundle IDs.
- **Automated content.** Scheduled jobs generate and validate questions, and policy checks decide what's published.
- **Edge delivery.** The API and web version run on Cloudflare, with nothing to manage.

## Stack

Swift · SwiftUI · watchOS · WidgetKit · Cloudflare Workers & Pages · GitHub Actions · LLM content pipeline
