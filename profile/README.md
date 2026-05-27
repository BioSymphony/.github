# BioSymphony

**AI agent tools for biological research.**

[Website](https://biosymphony.github.io/)

BioSymphony builds public toolkits for using coding agents in biological
research. Current toolkits cover biosynthetic route exploration, structural
biology campaigns, natural-product genome mining, fermentation experiment
design, and cryo-EM review.

Each toolkit ships local demos, agent skill packs, and templates for concrete
outputs.

## Start Here

- [BioProspector](https://github.com/BioSymphony/biosymphony-bioprospector)
  maps biosynthetic routes for target molecules: enzyme and gene candidates,
  pathway ideas turned into follow-up searches and experiment plans.
- [Structure Factory](https://github.com/BioSymphony/biosymphony-structure-factory-public)
  runs structural biology campaigns: binder design, structure mapping,
  candidate screening, ranking, and local or cloud run plans.
- [GeneCluster](https://github.com/BioSymphony/biosymphony-genecluster)
  searches public plant, fungal, and microbial data sources for
  natural-product gene clusters, with candidate comparison and follow-up
  planning.
- [Ferm DoE](https://github.com/BioSymphony/biosymphony-ferm-doe)
  plans fermentation and biomanufacturing experiments: design options,
  scale-context comparison, and run plans.
- [CryoCore](https://github.com/BioSymphony/biosymphony-cryocore-public)
  drives cryo-EM review: maps and models, figure planning, state comparison,
  and local or cloud compute setup.

## Shared across the toolkits

- Repo-local agent instructions and skill packs.
- Local demos that use synthetic fixtures or explicitly public inputs.
- Setup and formatting checks for local runs.
- Templates for search plans, experiment plans, review notes, and compute
  setup.
- Paths from local demos to operator-owned cloud, HPC, or GPU resources.

## Using Them with an Agent

1. Choose the toolkit that matches your research workflow.
2. Read the repository `README.md` and `AGENTS.md`.
3. Run the local demo or smoke test.
4. Give your coding agent the repo-local instructions or skill pack.

## Working Style

Scientific judgment belongs with the researcher. The agent can collect
context, prepare files, run routine checks, and summarize early findings. The
researcher sets the question, chooses inputs, interprets outputs, and decides
what belongs in the next analysis or experiment.

Begin with one research question and one local demo. Inspect the output before
expanding the analysis. Apply your lab's standard review practices.

## Contributing

Issues and pull requests are welcome in the relevant repository. Helpful
contributions include public examples, clearer documentation, reproducibility
fixes, and adapters for local agent workflows.

Please keep private data, credentials, and unpublished biological details out
of issues, pull requests, and examples.
