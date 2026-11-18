# Maximilian Schottke

Entrepreneur in Berlin. Close to seven years as managing director of an omnichannel brand for sleep systems, plus my own consultancy for e-commerce and digital projects in mid-sized companies.

Since 2026 I have been running a business with AI agents: Claude Code and MCP across shop, marketplaces and ERP. Processes, rules, approvals and sign-off are mine; the agents write the code.

Deutsche Fassung: [README.de.md](README.de.md)

## Open-source projects

Three small tools that came out of that work. Each one runs without an account or an API key, and each README says what was tested and what was not.

| Project | Use it when | First step |
|---|---|---|
| [safe-write-mode](https://github.com/maxschottke-spec/safe-write-mode) | an agent or script holds an API token and must not change live data by accident. Reads always work, writes need an explicit mode and a confirmation, every attempt is logged. Node.js, no dependencies. | [Quickstart](https://github.com/maxschottke-spec/safe-write-mode#quickstart) |
| [schadenfall-demo](https://github.com/maxschottke-spec/schadenfall-demo) | you want a runnable template for "the model reads and quotes its evidence, fixed code decides, a human approves". 16 invented insurance claims with expected results, replayable offline. Python, standard library only. | [README](https://github.com/maxschottke-spec/schadenfall-demo#readme) |
| [seo-survival-kit](https://github.com/maxschottke-spec/seo-survival-kit) | a shop lost visibility after a Google core update and you work with Claude Code. Skills for diagnosis, a recovery plan and a weekly check. No skill changes anything on the live system by itself. | [README](https://github.com/maxschottke-spec/seo-survival-kit#readme) |

**State, honestly:** all three are automatically tested and run in CI. safe-write-mode was also checked in a real Claude Code session. No outside user has confirmed any of them yet. If you try one, an issue saying where you got stuck is the most useful thing you can send.

Most of my work is in private repositories, because customer and business data live there.

## How my AI team works

- **Agents may read everything and change things only with my approval.** Before any change to a production system the agent shows what is affected. The approval covers that one change.
- **A mistake may happen once.** Every mistake is written down with its cause. The second time it gets a rule and, where possible, an automated test; the third time it is made technically impossible.
- **Whoever builds does not review.** What one model built is checked by an independent reviewer without prior knowledge: a model from another vendor where the data allows it, otherwise a separate agent.
- **Green tests are not enough.** I look at what actually arrives, in the browser and on the phone.
- **Every claim needs a source.** Numbers come fresh from the system. Without a source we ask or leave it out.
- **Some things stay with me.** Prices, legal wording, negotiations and sending e-mail do not run automatically. One exception was a deliberate decision: a weekly report that is sent behind two checks and can be switched off.
- **Automation comes slowly.** Only after a process has run cleanly by hand three times.

## Contact

[linkedin.com/in/max-schottke](https://www.linkedin.com/in/max-schottke)
