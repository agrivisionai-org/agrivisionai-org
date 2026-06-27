# Contributing to AGRIVISION AI

Hey -- thanks for stopping by. AGRIVISION AI builds AI products for farmers and agricultural extension workers across India, Africa, Latin America, and Southeast Asia. Our flagship, **YieldAI Global**, ships in 70+ languages across 40+ countries. Every contribution here lands in front of real growers, so we care a lot about getting it right -- and we want it to be a good experience for you, too.

We build in public. Pull up a chair.

## Ways to contribute

- **Code** -- features, bug fixes, performance, accessibility, i18n
- **Agronomy & domain input** -- crop calendars, pest signatures, mandi pricing nuance, regional advisory conventions
- **Translations** -- we ship in 70+ languages; native-speaker review is gold
- **Docs** -- READMEs, runbooks, model cards, eval reports
- **Issues** -- reproducible bugs and well-scoped feature requests

If you're not sure where to fit, open a Discussion or email **hello@agrivisionai.org**.

## Dev environment setup

1. Fork the repo and clone your fork.
2. Install the toolchain pinned in each repo's README (Node, Python, and `uv` are the common ones).
3. Copy `.env.example` to `.env.local` and fill in keys. Never commit real keys.
4. Run `make setup` (or the repo-specific equivalent) -- this installs deps, pulls model weights where needed, and runs a smoke test.
5. Run the test suite before you start: `make test`. A green baseline saves debugging later.

For the AI components (RAG, agent workflows, voice pipelines), the README will point you at sample fixtures so you don't need production API keys to develop locally.

## Filing issues

Before opening one, please search existing issues. When filing:

- **Bugs** -- what you expected, what happened, repro steps, environment, logs. Screenshots help.
- **Feature requests** -- describe the farmer or extension-worker problem first, then the proposed solution. Domain context matters more than implementation details.
- **Security** -- do **not** open a public issue. Email **security@agrivisionai.org**.

## Proposing changes

1. Open an issue or Discussion first for anything non-trivial -- saves rework.
2. Branch from `main`: `feat/short-description` or `fix/short-description`.
3. Keep PRs focused. One change, one PR.
4. Add or update tests. For model changes, include eval numbers (before vs after).
5. Update docs in the same PR.

## Commit messages

We use [Conventional Commits](https://www.conventionalcommits.org/):

```
feat(advisory): add Telugu voice prompts for kharif sowing
fix(prices): handle missing MSP rows for minor millets
docs(rag): clarify retrieval index rebuild steps
chore(deps): bump langchain to 0.3.x
```

Types we use: `feat`, `fix`, `docs`, `chore`, `refactor`, `test`, `perf`, `i18n`, `eval`.

## PR review process

- A maintainer will review within ~3 business days.
- CI must be green. Reviewers may request changes -- please don't take it personally; we're optimizing for farmers downstream.
- Two approvals required for changes to advisory logic, pricing signals, or anything user-facing in production.
- Squash-merge is the default.

## Tone

Be direct, be kind, assume good faith. Critique the code or the idea, not the person. If you disagree, say so plainly and explain why -- that's how we get to good answers.

## Discussing agriculture-domain questions

Crop science is regional and seasonal. When proposing changes that touch advisory content, pest models, or mandi data:

- Cite the source (ICAR, FAO, state extension departments, peer-reviewed papers, vetted field data).
- Name the region, crop, and season the claim applies to -- "wheat" in Punjab is not "wheat" in Bihar.
- Loop in a domain reviewer via the `domain-review` label.

## Getting help

- **Discussions** -- design questions, ideas, "is this the right approach?"
- **hello@agrivisionai.org** -- anything else
- **LinkedIn** -- [linkedin.com/company/113249948](https://linkedin.com/company/113249948)
- **Website** -- [agrivisionai.org](https://agrivisionai.org)

Founded by Vijesh Reddy Golamari (ex-Google, ex-Meta, ex-Citi, ex-Flipkart). We're a small team building for a very large problem -- your help genuinely moves the needle. Welcome aboard.
