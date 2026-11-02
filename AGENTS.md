# Repository guidance

## Current state

This repository contains planning documentation only. There is no package
manifest, source implementation, executable example or test suite. Do not
invent installation commands, API signatures, published versions, backtest
results, trading performance or statistical guarantees.

## Intended role

`sequentialist-markets` is a proposed application package for market/risk
workflows and strategy deterioration. Mathematical procedures belong in
`sequential-analysis`; generic search and interaction algorithms belong in
`sequential-search` and `sequential-games`. Common execution/audit and rendering
infrastructure belong to `sequentialist-core` and `sequentialist-visuals`.

The [README](README.md) and [overview](docs/overview.md) describe target scope.
Clearly mark proposals and unresolved choices. Realised gains, prediction
accuracy and control of trading losses must not be inferred from a sequential
test's error bound.

## Editing and checks

For documentation changes, validate local Markdown links, factual status,
source attribution and `git diff --check`. There are no test or build commands
yet. Report that distinction rather than reporting a zero-test run as success.
Do not create package scaffolding or select trading/execution behavior as a
side effect of documentation work.

## Assistant entry points

AGENTS.md is shared development context. CLAUDE.md, QWEN.md and GEMINI.md point
here; actual automatic loading depends on the client. [llms.txt](llms.txt)
and the overview are retrieval-oriented documentation for Grok, Perplexity and
other systems, with no indexing or ranking promise.
