# seamwatch

> **Status: starter. Nothing is built yet.** This repo is the home for our entry to the
> [Nebius x NVIDIA Global AI Hackathon](https://nebiusglobalaihackathon.devpost.com/).
> The concept below is a proposal, not a final team decision.

## The idea (proposed)

Git catches "we edited the same lines." It misses "you changed what `calc_total` returns while a
teammate writes code that depends on the old behavior." That change merges cleanly, then breaks.

seamwatch is a Git-native collaboration layer for teams and their coding agents. It warns people
before their in-progress work semantically collides:

1. **Fast layer:** a symbol-level dependency graph (static analysis, not an LLM) intersects
   "everything that depends on the symbol I changed" with "the code my teammate is editing now."
2. **Confirm layer:** a speculative merge of both in-progress states, with tests run in a Nebius
   sandbox, turns "possible conflict" into "confirmed: this test fails when combined."
3. **NVIDIA model:** Nemotron summarizes each person's in-progress intent, explains the impact in
   plain English, and proposes a small reconciling patch.

Only confirmed conflicts should interrupt someone.

## Hackathon requirements this repo must meet

- [ ] Runs on **Nebius Token Factory** or **Nebius AI Cloud** (a runtime call to Token Factory, or compute on Serverless Jobs / Endpoints / DevPods)
- [ ] Uses at least one **NVIDIA open-source model** (Nemotron)
- [ ] One track chosen (Coding and Agentic Engineering is the closest fit)
- [x] Public repository
- [x] Open-source license file (MIT, see [LICENSE](LICENSE))
- [ ] README that shows how Nemotron and Token Factory are used (section below)
- [ ] Hosted demo URL
- [ ] Demo video under 3 minutes
- [ ] Feedback on Nebius and NVIDIA tools (required by the rules)

**Submission closes Fri Oct 30, 2026, 10:00 am PT.** The Devpost page is the authority on the rules.

## How we use Nemotron and Nebius

_To be filled in as we build. State exactly which model, which endpoint, and what each call does._

## Run it

_Setup and run instructions go here once there is code._

## Team

Shamit and teammate. Roles to be added.

## License

[MIT](LICENSE)
