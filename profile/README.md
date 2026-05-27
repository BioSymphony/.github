# BioSymphony

**Agentic AI infrastructure for biological research.**

BioSymphony builds public, agent-readable toolkits for turning biological
research goals into reviewable workflows: durable manifests, schema-checked
artifacts, provenance records, claim boundaries, and local-to-cloud execution
plans.

Our public repositories are built for scientific operators who want AI agents
to do useful work without losing traceability, scientific caution, or control
over private data.

## What We Build

- **Agent-ready workflows** with skill packs, prompts, schemas, validators,
  examples, and compact handoff artifacts.
- **Reviewable scientific outputs** that separate planning, evidence,
  execution, and validation claims.
- **Public-safe demos** using synthetic fixtures or explicitly public data.
- **Compute-portable run shapes** that can start locally and escalate to
  operator-owned cloud, HPC, or GPU resources when a reviewed lane earns it.

## Public Toolkits

| Repository | Use it for |
| --- | --- |
| [biosymphony-bioprospector](https://github.com/BioSymphony/biosymphony-bioprospector) | Agentic biosynthetic pathway discovery: route expansion, enzyme and gene candidate mining, pathway stitching, and construct-hypothesis review packages. |
| [biosymphony-ferm-doe](https://github.com/BioSymphony/biosymphony-ferm-doe) | Constraint-aware experimental design for fermentation and biomanufacturing: DoE planning, scale bridge checks, adaptive backend routing, and run packets. |
| [biosymphony-cryocore-public](https://github.com/BioSymphony/biosymphony-cryocore-public) | Agent-ready cryo-EM workflows for map/model review, density support, structural figures, state comparison, and cloud run preparation. |

## How To Use The Repos

1. Pick the toolkit that matches your research workflow.
2. Read the repository `README.md` and `AGENTS.md`.
3. Run the local smoke test or demo before giving an agent a larger task.
4. Point your coding agent at the repo-local skill pack and keep private data
   in operator-owned storage outside the public checkout.

## Safety And Release Boundaries

BioSymphony public repos are research infrastructure, not substitutes for
scientific review, wet-lab validation, biosafety review, regulatory review,
clinical guidance, LIMS, ELN, or GxP batch-record systems.

We do not publish secrets, private datasets, unpublished biological data,
private run logs, customer records, raw provider artifacts, or internal
planning notes. Reusable mechanics are generalized before release.

## Contributing

Issues and pull requests are welcome in the relevant repository. The most
useful contributions are public-safe examples, documentation improvements,
schema and validator fixes, reproducibility checks, and small adapters that
make agent work easier to review.

Please keep private data, credentials, and unpublished biological details out
of issues, pull requests, and examples.

