# Architecture

```mermaid
flowchart LR
  subgraph Apps[Per-country builds from one codebase]
    I[iOS app] --- WA[Watch app] --- WG[Widgets]
  end
  Apps -->|questions| API[Cloudflare Workers API]
  WEB[Web · Cloudflare Pages] --> API
  PIPE[Scheduled question pipeline<br/>generate → validate → publish] --> API
```

## Key decisions

| Decision | Why |
|---|---|
| Per-country apps instead of one big app | Stronger local branding and App Store search, and each market gets its own listing |
| One codebase with per-country config | Many apps, but only one thing to maintain |
| Watch and widgets in every build | Daily, glanceable engagement brings people back |
| Questions served from the edge | Content updates without app releases |
