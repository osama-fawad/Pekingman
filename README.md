<h1 align="center">Pekingman v1.0.0: A Multimodal AGI-Oriented Agent System</h1>

<p align="center"><small>
TingYun Yin, Massachusetts Institute of Technology (MIT) &nbsp;&nbsp; Peixu Cai, University of Southern California (USC) &nbsp;&nbsp; Shahzaib Saqib Warraich, University of Southern California (USC) &nbsp;&nbsp; Osama Fawad, Université Bourgogne Europe (UBE)
</small>
</p>

<p align="center">
  <a href="https://osama-fawad.github.io/Pekingman/">Project Page</a> |
  <a href="https://osama-fawad.github.io/Pekingman/">Demo Video</a>
</p>

<p align="center">
  <video src="github-page/media/pekingman-demo.mp4" controls poster="github-page/media/poster.jpg"></video>
</p>

Pekingman v1.0.0 is a multimodal AGI-oriented agent system designed for environmental perception, long-term memory, human-like reasoning, emotional consistency, and real-time behavioral response. Equipped with a high-capacity persistent memory system, it can store, retrieve, and revisit historical events, giving NPCs authentic human-like behavioral logic.

## Abstract

Pekingman connects perception, memory, reasoning, emotion, and action into one continuous agent loop. The system is designed for virtual characters that need to observe changing environments, remember past interactions, make context-aware decisions, and respond with consistent behavior.

The current implementation focuses on:

- ingesting multi-source environmental signals;
- extracting emotional and semantic context;
- storing and revisiting historical interactions;
- selecting behavior from live context;
- producing responsive actions for interactive NPC scenarios.

## Human-Equivalent Capabilities

Pekingman is designed to replicate a broad set of core cognitive and behavioral capabilities associated with human-like agents. It continuously senses surrounding environmental changes, generates context-matched behavioral feedback to external stimuli, and maintains long-term memory of past experiences. It also supports humanized logical reasoning, sequential decision-making, and consistent emotional tendency expression, enabling NPCs to exhibit coherent, lifelike behaviors across long-running interactions.

The core capability set includes:

1. **Environmental sensing:** continuously observe multi-dimensional scene changes through multimodal input.
2. **Real-time response logic:** generate natural feedback and action plans matched to current external conditions.
3. **Long-term memory iteration:** persist, retrieve, and reference historical interactions to maintain sustained character consistency.
4. **Humanized decision and emotion output:** simulate human-style reasoning, preference shifts, task choices, and emotional expression.

This makes Pekingman useful for virtual NPCs, digital human projects, metaverse platforms, simulation games, and other commercial interactive content where characters need continuity, responsiveness, and believable behavior.

Lightweight games with low world complexity can often rely on basic trigger logic for NPC behavior. In contrast, large open-world titles and high-complexity simulation environments require agents with multimodal perception, real-time response, and long-term memory to produce natural and consistent virtual human behavior at scale.

## News
- **August 2026:** Release full code.
- **July 2026:** Added a GitHub Pages demo page with a compressed web copy of the project video.
- **June 2026:** Expanded interactive character control, environment awareness, and live visualization.
- **May 2026:** Added behavior selection, memory continuity, identity modeling, and end-to-end validation.

## Overview

The project has four main capability areas:

- **Perception:** understands environmental changes from multiple signal types.
- **Memory:** stores, retrieves, and references long-running interaction history.
- **Reasoning:** chooses context-aware behavior based on goals, state, and prior experience.
- **Action:** produces responses suitable for interactive virtual characters and NPCs.

## Hardware Requirements

Minimum requirements depend on which capabilities you run:

- CPU-only hardware is enough for lightweight demos and documentation preview.
- A modern GPU is recommended for advanced perception, generation, and large-scale interactive scenarios.
- Real-time 3D simulation experiments require a workstation capable of running the target simulation environment.

## Software Requirements

- Python 3.11
- Conda or another Python environment manager
- Optional GPU acceleration for advanced demos
- Optional 3D engine support for simulation experiments

## Cloning the Repository

```bash
git clone <your-pekingman-repository-url>
cd pekingman_project
```

This repository contains local data and experimental assets. Before publishing publicly, review ignored files and avoid committing secrets, generated caches, private documents, or local runtime data.

## Environment Setup

Create the Python environment with the provided environment file:

```bash
conda env create -f environment.yml
conda activate pekingman
```

Install lightweight web preview requirements when needed:

```bash
pip install -r requirements-web.txt
```

Copy and edit environment variables:

```bash
cp ../api-keys.env.example ../api-keys.env
```

`api-keys.env` is ignored by Git and should contain local database credentials and API keys.

## Optional Services

Advanced deployments can connect persistent storage, model services, speech processing, and simulation runtime components. These services are optional for reading the documentation or viewing the demo page.

## Running the Demo Page

The static project page lives in `github-page/`:

```bash
cd github-page
python3 -m http.server 8080
```

Open:

```text
http://127.0.0.1:8080/
```

The page uses `github-page/media/pekingman-demo.mp4`, a web-optimized copy of `demo_video/北京猿人.mp4`.

## Tests

Run local checks from the development environment:

```bash
python -m pytest
```

Some checks require optional services, local credentials, or simulation inputs. If a check fails because a service is missing, start the corresponding prerequisite or run a narrower smoke test.

## Functionalities

- **Observe:** collect multimodal environmental signals.
- **Remember:** preserve working memory, long-term memory, and entity-linked context.
- **Understand:** summarize current state from perception, memory, and emotional context.
- **Plan:** select tasks from goals, context, health, and environment conditions.
- **Act:** produce executable behavior plans for virtual characters.
- **Monitor:** inspect live agent activity through the local visualization page.

## Known Limitations

- Several advanced capabilities are experimental and may fall back when optional services are unavailable.
- Public release should exclude local credentials, generated outputs, private documents, and local runtime data.
- Optional perception and generation dependencies may require platform-specific installation steps.

## Citation

If you use this project as a research artifact, please cite the repository:

```bibtex
@software{pekingman2026,
  title  = {Pekingman v1.0.0: A Multimodal AGI-Oriented Agent System},
  year   = {2026}
}
```

Add the repository URL to the BibTeX entry after the project is published.

## Acknowledgments

This project integrates ideas and tools from embodied agents, memory systems, multimodal AI, interactive simulation, and open-source Python infrastructure.
