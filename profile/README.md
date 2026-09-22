![BioSymphony: a retro-game research lab with plants, protein structures, and fermentation vessels](https://raw.githubusercontent.com/BioSymphony/.github/main/profile/assets/biosymphony-banner.png)

# BioSymphony

Use biological research tools with your AI agent. BioSymphony combines tool
knowledge, scripts, and reusable workflows for sequence search, protein
modeling, molecular design, cryo-EM, and experiment design.

The skills explain which tools fit a question, what inputs they need, how to
call them, and how to connect their outputs. You and your agent can use that
knowledge to run analyses and decide what to investigate next.

[Choose a toolkit](#choose-a-toolkit) · [Example toolchains](#connect-tools-into-analyses) · [Get started](#use-your-agent-harness) · [Website](https://biosymphony.github.io/)

## Choose A Toolkit

### [BioProspector](https://github.com/BioSymphony/bioprospector) · Compare Pathways And Find Enzyme Candidates

Explore alternative biosynthetic routes and investigate missing steps. Combine
sequence searches, domain annotations, structural neighbors, and reaction
references to compare candidate enzymes and route feasibility.

[Tool knowledge](https://github.com/BioSymphony/bioprospector/blob/main/docs/tool-stack.md):
DIAMOND, MMseqs2, BLAST+, HMMER, Foldseek, and Rhea.

### [GeneCluster](https://github.com/BioSymphony/genecluster) · Search Genes And Compare Genome Context

Connect sequence search, function annotation, and gene-cluster comparison.
Extract matched sequences, join gene identifiers across tools, and compare
candidate genes across species. Compare genomic neighborhoods where coordinates
are available.

[Calling and chaining guide](https://github.com/BioSymphony/genecluster/blob/main/skills/genecluster-superpowers/SKILL.md):
MMseqs2, HMMER, InterProScan, antiSMASH, plantiSMASH, cblaster, and clinker.

### [Structure Factory](https://github.com/BioSymphony/structure-factory) · Compose Protein Design And Prediction Workflows

Choose tools for backbone design, sequence design, complex prediction,
scoring, and visualization. Compare methods with consistent inputs and metrics,
and connect configured tools through local commands, APIs, or compute providers.

[Tool cards](https://github.com/BioSymphony/structure-factory/blob/main/tools/README.md):
RFdiffusion3, ProteinMPNN, Boltz, Chai-1, and ChimeraX, among other methods.

### [CryoCore](https://github.com/BioSymphony/cryocore) · Work With Cryo-EM Maps And Models

Choose processing and validation methods, assess how models fit experimental
maps, compare conformational states, and prepare structural figures. Try the
CPU-only review demo before configuring a larger workflow.

[Software guide](https://github.com/BioSymphony/cryocore/blob/main/docs/tooling-and-licensing.md):
RELION, CryoSPARC, Phenix, Coot, and ChimeraX workflows and setup requirements.

### [Small Molecules](https://github.com/BioSymphony/small-molecules) · Choose Chemistry Tools For Your Task

Match molecular generation, synthesis planning, docking, affinity estimation,
and property prediction methods to your inputs. Give your agent the method
comparisons, calling references, and setup knowledge it needs to write and run
an analysis with the selected tools.

[Tool matrix](https://github.com/BioSymphony/small-molecules/blob/main/references/tool-matrix.md):
AiZynthFinder, RDKit, AutoDock Vina, GNINA, and other chemistry tools.

### [Ferm DoE](https://github.com/BioSymphony/ferm-doe) · Generate Designs And Choose The Next Experiment Batch

Generate fermentation experiment designs, analyze supplied results, and select
follow-up batches under factor, cost, and run-count constraints. Compare
scale-transfer assumptions and use optional optimization backends when needed.

[Commands](https://github.com/BioSymphony/ferm-doe/blob/main/docs/CLI_REFERENCE.md)
and [backends](https://github.com/BioSymphony/ferm-doe/blob/main/docs/TOOL_REGISTRY.md):
`ferm-doe`, SciPy, BoFire, ENTMOOT, and BoTorch.

## Connect Tools Into Analyses

A useful toolchain passes the right data to the next method. Your agent extracts
sequences, converts file formats, matches identifiers, and checks outputs
between calls. These examples show tool combinations and command sequences
documented by the toolkits.

<a href="https://raw.githubusercontent.com/BioSymphony/.github/main/profile/assets/toolchains.svg">
  <picture>
    <source media="(max-width: 600px)" srcset="https://raw.githubusercontent.com/BioSymphony/.github/main/profile/assets/toolchains-mobile.svg">
    <img src="https://raw.githubusercontent.com/BioSymphony/.github/main/profile/assets/toolchains.svg" alt="Three examples. GeneCluster: MMseqs2 search, matched protein sequences, HMMER or InterProScan annotation, and Quarto reporting. Structure Factory: RFdiffusion3 backbone design, ProteinMPNN sequence design, Boltz or Chai-1 complex prediction, and ChimeraX figures. Ferm DoE: validate inputs, generate a design, analyze supplied results, and plan a follow-up batch. Experiments occur separately; analysis uses supplied data.">
  </picture>
</a>

The toolkits include runnable helpers and reference workflows. Scientific tools,
models, and databases have their own installation requirements; the linked
guides distinguish available integrations from methods that need adaptation.

## Use Your Agent Harness

Open a toolkit in Codex, Claude Code, or another agent that can read files and
call tools. The agent uses your existing shell, Python environment, APIs, or
configured compute. You can also run the supplied command-line tools directly.

<a href="https://raw.githubusercontent.com/BioSymphony/.github/main/profile/assets/agent-workflow.svg">
  <picture>
    <source media="(max-width: 600px)" srcset="https://raw.githubusercontent.com/BioSymphony/.github/main/profile/assets/agent-workflow-mobile.svg">
    <img src="https://raw.githubusercontent.com/BioSymphony/.github/main/profile/assets/agent-workflow.svg" alt="You provide the question, data, and compute limits. BioSymphony supplies tool knowledge and workflows to your AI agent. The agent selects and calls configured scientific tools, inspects the results, and chooses the next analysis with you.">
  </picture>
</a>

Start with a small analysis:

> Read this toolkit's skill and tool guides. My goal is [question], using [inputs].
> Choose a toolchain and check its dependencies. Run a small local example,
> inspect the outputs, and use those results to suggest the next analysis.
> Explain which commands ran and which tools still need setup.

## Related Tools

- [Proteus](https://github.com/jvogan/proteus) automates structure lookup, PyMOL and ChimeraX analysis, and molecular figures.
- [BioVoice](https://github.com/jvogan/biovoice) lets you control PyMOL and ChimeraX by voice.
- [NeoCloud Bridge](https://github.com/jvogan/symphony-neocloud-bridge) runs approved workloads on cloud providers and returns outputs to your workspace.

## Contribute

Useful contributions include tool integrations, calling examples, analysis
recipes, and fixes to the tool guides. Open an issue or pull request in the
relevant repository, using public or synthetic data for shared examples.
