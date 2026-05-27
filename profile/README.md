# BioSymphony

**AI agent tools for biological research.**

BioSymphony builds open toolkits that help scientists use coding agents on
real biological research tasks. The repos here give agents enough structure to
search, plan, run small checks, organize results, and hand work back in a form
that a human can read and improve.

The common pattern is simple: describe the goal, point the agent at the
repo-local instructions, run the first demo locally, then grow into a larger
workflow when the direction is useful.

## Start Here

- [BioProspector](https://github.com/BioSymphony/biosymphony-bioprospector)
  explores biosynthetic routes to target molecules, finds enzyme and gene
  candidates, and turns pathway ideas into concrete follow-up work.
- [GeneCluster](https://github.com/BioSymphony/biosymphony-genecluster) runs
  natural-product genome-mining campaigns across public plant, fungal, and
  microbial data sources.
- [Ferm DoE](https://github.com/BioSymphony/biosymphony-ferm-doe) helps plan
  fermentation and biomanufacturing experiments, choose useful design
  families, check scale context, and prepare run packets.
- [CryoCore](https://github.com/BioSymphony/biosymphony-cryocore-public) works
  through cryo-EM map and model questions, figure planning, state comparison,
  and local or cloud compute preparation.

## What The Repos Share

- Agent instructions in `AGENTS.md` and repo-local skill packs.
- Local demos that use synthetic fixtures or explicitly public inputs.
- Small command-line checks that help an agent catch simple mistakes early.
- Examples and templates that turn broad scientific questions into bounded
  pieces of work.
- Paths from local runs to operator-owned cloud, HPC, or GPU resources when a
  task needs more compute.

## Using Them With An Agent

1. Pick the toolkit that matches your research workflow.
2. Read the repository `README.md` and `AGENTS.md`.
3. Run the local smoke test or demo before giving an agent a larger task.
4. Point your coding agent at the repo-local skill pack.
5. Keep private data in your own storage and out of public issues, examples,
   and pull requests.

## Working Style

These projects assume a scientist stays close to the work: setting goals,
choosing data sources, approving compute, interpreting results, and deciding
what is worth doing next. Agents help with search, setup, organization,
repetition, and first-pass synthesis.

Use the public repos with appropriate scientific, biosafety, regulatory, and
operational review for your setting.

## Contributing

Issues and pull requests are welcome in the relevant repository. The most
useful contributions are examples with public inputs, clearer documentation,
small reproducibility fixes, and adapters that make agent work easier to run
and review.

Please keep private data, credentials, and unpublished biological details out
of issues, pull requests, and examples.
