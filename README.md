# sequentialist-markets

Planned application software for sequential analysis of markets, risk and
strategy deterioration in the Sequentialist ecosystem.

This repository currently contains planning and discovery documentation only.
There is no implementation, installable package, public API, benchmark or
validated trading strategy here. The proposed Python import name
`sequentialist.markets` describes intended placement, not an available module.

The target architecture separates mathematical methods (`sequential-analysis`,
`sequential-search`, `sequential-games`) from software engineering
(`sequentialist-core`, `sequentialist-visuals`) and subject applications such as
this one. Future market-specific states, constraints, costs and workflows
belong here; common algorithms belong in their methodological libraries.

Start with the [plain-language overview and planning FAQ](docs/overview.md).
The same overview is available [in Russian](docs/overview.ru.md).
[llms.txt](llms.txt) indexes the available sources. [AGENTS.md](AGENTS.md)
describes the current repository state and contribution boundaries.
