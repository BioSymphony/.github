# BioSymphony

**AI agent tools for biological research.**

[Website](https://biosymphony.github.io/)

BioSymphony develops public toolkits for agent-assisted biological research.
The repos cover biosynthetic route exploration, structural biology campaign
design, natural-product genome mining, fermentation experiment design, and
cryo-EM analysis support.

Each toolkit includes local instructions, public or synthetic examples, local
checks, and templates for concrete outputs: search plans, candidate lists,
experiment designs, review notes, and compute setup.

Start with one research question and one local demo. Inspect the output before
expanding the analysis.

## Start Here

- [BioProspector](https://github.com/BioSymphony/biosymphony-bioprospector)
  explores biosynthetic routes for target molecules. It identifies enzyme and
  gene candidates and turns pathway ideas into follow-up searches and
  experiment plans.
- [Structure Factory](https://github.com/BioSymphony/biosymphony-structure-factory-public)
  supports structural biology campaigns: binder design, structure mapping,
  candidate screening, ranking, and local or cloud run plans.
- [GeneCluster](https://github.com/BioSymphony/biosymphony-genecluster) runs
  natural-product genome-mining campaigns across public plant, fungal, and
  microbial data sources.
- [Ferm DoE](https://github.com/BioSymphony/biosymphony-ferm-doe) helps plan
  fermentation and biomanufacturing experiments. It prepares design options,
  compares scale context, and builds run plans.
- [CryoCore](https://github.com/BioSymphony/biosymphony-cryocore-public)
  supports cryo-EM map and model review, figure planning, state comparison,
  and local or cloud compute setup.

## What the Repos Share

- Agent instructions in `AGENTS.md` and repo-local skill packs.
- Local demos that use synthetic fixtures or explicitly public inputs.
- Setup and formatting checks for local runs.
- Templates for search plans, experiment plans, review notes, and compute
  setup.
- Paths for moving from local demos to operator-owned cloud, HPC, or GPU
  resources.

## Using Them with an Agent

1. Choose the toolkit that matches your research workflow.
2. Read the repository `README.md` and `AGENTS.md`.
3. Run the local demo or smoke test.
4. Give your coding agent the repo-local instructions or skill pack.
5. Keep private data in your own storage and out of public issues, examples,
   and pull requests.

## Working Style

Scientific judgment belongs with the researcher. The agent can collect
context, prepare files, run routine checks, and summarize early findings. The
researcher sets the question, chooses inputs, interprets outputs, and decides
what belongs in the next analysis or experiment.

Use these tools under the review practices required for your lab, institution,
or project.

## Contributing

Issues and pull requests are welcome in the relevant repository. Helpful
contributions include public examples, clearer documentation, reproducibility
fixes, and adapters for local agent workflows.

Please keep private data, credentials, and unpublished biological details out
of issues, pull requests, and examples.
