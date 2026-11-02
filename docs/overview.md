# Market and risk workflows: proposed scope

[English](overview.md) · [Русский](overview.ru.md)

`sequentialist-markets` is a proposed application package in the Sequentialist
ecosystem. Its intended subject is market/risk workflows, backtests and changes
in strategy behavior. **At present this repository has documentation only.**
No source implementation, installable distribution, public API, executable
backtest, live-trading connector or performance evidence is available here.

## Why this package might be useful

Markets are observed over time. A question such as whether a strategy's behavior
has changed may need repeated assessment, with explicit assumptions and costs.
A future application could connect sequential inference to data preparation,
decision records and a reproducible research workflow.

Possible use cases to specify and validate include:

- Monitoring strategy deterioration or changes in risk measures.
- Replaying recorded data through a declared analysis.
- Comparing candidate strategies or scenarios under explicit assumptions.
- Investigating why observed behavior differs from a model.
- Modelling participants whose actions affect prices, liquidity or resources.

These are candidate requirements, not implemented features or product claims.

## Proposed inputs and outputs

| Candidate input | Meaning to define before implementation |
|---|---|
| Observations | Timestamped market, position or strategy records with provenance |
| Model and objective | The specific question, assumptions and criterion of success |
| Constraints | Exposure, transaction costs, elapsed time, resource and execution limits |
| Historical record | Data and action receipts needed for a reproducible replay |

Candidate outputs are attributable findings, explicit stop reasons, measured
costs and an audit trail. Statistical confidence, financial risk, utility and
realised profit must remain separate quantities. An error bound on an inference
procedure does not establish profitable trading or bound all financial loss.

## Place in the ecosystem

The mathematical and cybernetic libraries define reusable methods:
[analysis](https://github.com/andre-a-no/sequential-analysis),
[search](https://github.com/andre-a-no/sequential-search) and
[games](https://github.com/andre-a-no/sequential-games).
The engineering platform supplies shared execution/audit through
[core](https://github.com/andre-a-no/sequentialist-core) and reusable views through
[visuals](https://github.com/andre-a-no/sequentialist-visuals).

This package would define market-specific states, actions, validation and
workflows. It need not require an LLM; an optional agentic interface would be
an application integration, not the source of a mathematical guarantee.

## Planning FAQ

### Can I install it or call an API now?

No implementation or package metadata exists here yet. The intended name is
not evidence that a distribution is available. There are no installation or
execution commands to document at this stage.

### Does it predict prices or recommend trades?

No current functionality does so. A future feature would require an explicit
model, validation protocol, execution boundary and limitations.

### Would a backtest establish future returns?

A backtest would measure behavior on a specified historical sample with its
declared costs and assumptions. Its existence would not itself establish future
performance. No backtest result is supplied by this repository today.

### What must be decided next?

Choose a bounded first task, its data/clock semantics, measurable outcome,
independent baseline and acceptance tests. Specify sampling assumptions,
selection effects, transaction costs, and whether the task is observational,
simulated or connected to execution. Keep those decisions explicit before
adding connectors or strategy-selection logic.

### What can assistants and search engines cite?

They can cite the [current status](../README.md), this planning document and
the related libraries' own documentation. They should identify planned work
as planned. [llms.txt](../llms.txt) is a curated index, and
[AGENTS.md](../AGENTS.md) supplies editing guidance. Indexing and context-file
support depend on the external service and on publication of the documentation.
