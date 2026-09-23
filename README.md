# Deepanshu Pal

GTM engineer working at the intersection of AEO, agentic commerce, and marketer-in-the-loop systems.

I build small, useful tools that turn a market insight into something testable: a benchmark, an audit, a data product, or an operating workflow.

- [marketerloop](https://github.com/DeepanshuPal/marketerloop) - human-approved agentic workflows for marketers
- [agent-ready](https://github.com/DeepanshuPal/agent-ready) - audit an ecommerce store for shopping-agent readiness
- [am-i-cited](https://github.com/DeepanshuPal/am-i-cited) - open-source AEO and LLM visibility tracking
- [compute.cafe](https://www.compute.cafe/) - a live GPU rental pricing index

Also contributing fixes to the agent, voice AI, and data tools I use.

## Receipts

- **agent-ready on 50 live DTC stores.** 50/50 audited. [First run](https://github.com/DeepanshuPal/agent-ready/tree/main/audits/2026-09-10-dtc-50): median 95, mean 92.1, one F (Vaaree, 18: product feed returns HTML, no schema.org). Two scores corrected by hand, both tool bugs, both fixed in code.
- **Re-audit with five new checks.** [2026-09-24](https://github.com/DeepanshuPal/agent-ready/tree/main/audits/2026-09-24-dtc-50): agent access vs a browser baseline, tiered robots.txt, soft-404 and bot-challenge detection, llms.txt linkage and shape, server-rendered product facts. Mean 91.2, median 93. 46 of 50 stores score 60/100 on llms.txt - the file exists but isn't linked or outlined.
- **Tests.** agent-ready: 22 passing. marketerloop: 7 passing.
- **Upstream merges.** 4 merged PRs in PostHog, LiveKit and notfair, listed below.

## OSS contributions

Merged:

- [PostHog/posthog-js#5051](https://github.com/PostHog/posthog-js/pull/5051) - skip cross-subdomain cookie removal when no cookie is visible to delete
- [livekit/agents#7300](https://github.com/livekit/agents/pull/7300) - shield voice transcript rotation from cancellation
- [nowork-studio/notfair-plugin#120](https://github.com/nowork-studio/notfair-plugin/pull/120) - resolve the gcloud ADC config dir per platform
- [nowork-studio/notfair-plugin#125](https://github.com/nowork-studio/notfair-plugin/pull/125) - fetch robots rules with the crawler user agent

Open:

- [mastra-ai/mastra#24619](https://github.com/mastra-ai/mastra/pull/24619) - preserve called concurrency on resume
- [BerriAI/litellm#41083](https://github.com/BerriAI/litellm/pull/41083) - forward custom_llm_provider in Responses WebSocket routing
- [BerriAI/litellm#41095](https://github.com/BerriAI/litellm/pull/41095) - reject Anthropic pass-through requests whose content blocks are all unrecognized
- [BerriAI/litellm#42194](https://github.com/BerriAI/litellm/pull/42194) - flatten empty text content lists for Moonshot
- [BerriAI/litellm#41004](https://github.com/BerriAI/litellm/pull/41004) - honor the caller's session id in spend logs
- [pandas-dev/pandas#68486](https://github.com/pandas-dev/pandas/pull/68486) - report dtype mismatch for NaT arrays with different units
- [browserbase/stagehand#2991](https://github.com/browserbase/stagehand/pull/2991) - hide the daemon console on Windows
- [qdrant/qdrant-client#1453](https://github.com/qdrant/qdrant-client/pull/1453) - keep cosine re-upserts idempotent in local mode
- [medusajs/medusa#16877](https://github.com/medusajs/medusa/pull/16877) - report unsupported TypeScript 7 in the CLI
- [METR/vivaria#1123](https://github.com/METR/vivaria/pull/1123) - fix PowerShell env file encoding on Windows
- [thinking-machines-lab/tinker-cookbook#952](https://github.com/thinking-machines-lab/tinker-cookbook/pull/952) - import the IFBench checker registry from the package
- [camel-ai/owl#625](https://github.com/camel-ai/owl/pull/625) - extract zip documents without an external command
- [mautic/mautic#17474](https://github.com/mautic/mautic/pull/17474) - fix MJML style serialization
- [storybookjs/storybook#36292](https://github.com/storybookjs/storybook/pull/36292) - document QueryClient isolation for docs pages and parallel story tests
- [nowork-studio/notfair-plugin#126](https://github.com/nowork-studio/notfair-plugin/pull/126) - keep skill descriptions under the 1024-character limit
- [nowork-studio/notfair-plugin#127](https://github.com/nowork-studio/notfair-plugin/pull/127) - ship playwright-core browsers.json in the standalone package
