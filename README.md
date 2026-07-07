# AgoraSim

**A hybrid agent-based modeling framework

[Try the web demo](https://haalab.github.io/AgoraSim/) ·
[Download local package](https://haalab.github.io/AgoraSim/downloads/agorasim-local-demo-package.zip) ·
[Repository](https://github.com/haalab/AgoraSim)

AgoraSim resolves natural-language or multimodal artifacts into editable ABM
configurations, runs ratio-controlled populations of LLM, vision-language,
custom-endpoint, random, and classical agents, and compares the same scenario
against matched classical reference dynamics.

![AgoraSim results dashboard](docs/assets/ui_results_dashboard.png)

## What AgoraSim Is For

AgoraSim is designed for exploratory scenario analysis rather than point
prediction. A user can start from a policy announcement, product launch,
advertisement, public statement, social-media post, market event, image, or
video, then inspect how different modeling assumptions change the resulting
scenario trajectory.

The central idea is comparison: if an LLM-agent run resembles a simple
threshold, contagion, herding, learning, or utility reference dynamic, the
pattern may be explainable by explicit ABM assumptions. If it diverges, that
divergence becomes a scenario hypothesis to inspect.

## Highlights

| Area | What AgoraSim Supports |
| --- | --- |
| Scenario workbench | Artifact-to-configuration workflow for events, target populations, action spaces, survey questions, networks, prompts, model mixes, and comparison plans |
| Hybrid agents | Ratio-controlled LLM, VLM, custom-endpoint, random, and classical agents using one structured decision schema |
| Interaction protocols | Independent survey, social diffusion, broadcast comment stream, sequential exposure, focus group, and A/B treatment |
| Classical references | Threshold/Bass, Deffuant, SIR, herding, DeGroot/voter, and discrete-choice reference dynamics |
| Audit records | Resolved configurations, prompts, structured decisions, public statements, heard statements, costs, model metadata, and rule diagnostics |

## Try It

The public GitHub Pages demo is static and safe to open in a browser:

```text
https://haalab.github.io/AgoraSim/
```

It includes a browser-only illustrative preview. It does not store API keys,
upload files, call LLM providers, or require a backend server.

For the full system, download the local package:

```text
https://haalab.github.io/AgoraSim/downloads/agorasim-local-demo-package.zip
```

After unzipping:

- macOS: run `run_macos.command`
- Windows: run `run_windows.bat` or `run_windows.ps1`
- Linux: run `run_linux.sh`

The local package starts AgoraSim on `127.0.0.1:8000` or the next available
local port. Users paste their own Anthropic, OpenAI, or Gemini keys only if they
want live LLM/VLM calls. No API keys are bundled.

## Demo Workflow

1. Enter a brief, draft, or media artifact.
2. Inspect and edit the generated ABM configuration.
3. Choose LLM/VLM/classic/random model slots and budget settings.
4. Select interaction protocols and classical reference dynamics.
5. Run the scenario locally.
6. Compare trajectories, survey aggregates, action distributions, and audit
   records.

## Repository Contents

```text
docs/
  index.html                         Static GitHub Pages project page
  assets/                            UI screenshots
  downloads/
    agorasim-local-demo-package.zip  Full local runnable package
    PACKAGE_MANIFEST.txt             Package contents and safety notes
```


## Responsible-Use Note

AgoraSim outputs are synthetic trajectories generated under explicit modeling
assumptions. They are useful for hypothesis generation, teaching, method
comparison, and baseline construction, but they are not measurements or
predictions of real populations. Claims about precise proportions, subgroup
reactions, tipping points, or individual trajectories require empirical
validation beyond the demo.

