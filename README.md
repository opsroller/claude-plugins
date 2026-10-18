# opsroller Claude plugins

A catalog of job-function plugins for Claude Code. Each plugin is a role a
person could hold on any team, with the agent, skills and workflows that
job needs. Every plugin lives in its own repository and is versioned on
its own; this repository only lists them, as the `opsroller` marketplace.

Roles never name a project or a technology they depend on. A project
tells a role what to work with in its own `CLAUDE.md` and project profile.

## Install and update (how-to)

Add the marketplace once, then install the shared practices and the roles
you need:

```
/plugin marketplace add opsroller/claude-plugins
/plugin install engineering-practices@opsroller
/plugin install gameplay-programmer@opsroller
```

When a plugin publishes a new version, refresh the catalog and update:

```
/plugin marketplace update opsroller
```

To add a role, create its own repository with `.claude-plugin/plugin.json`,
`agents/`, `skills/`, `workflows/` and Diataxis docs, keep it free of
project and stack specifics, then add its entry here in a `feat: add <role>`
pull request.

## Catalog (reference)

| Plugin | Job |
|---|---|
| [`engineering-practices`](https://github.com/opsroller/engineering-practices) | Shared working practices for every role: project onboarding, git with Conventional Commits, work packages, talking to other agents, and asset and code provenance. |
| [`project-manager`](https://github.com/opsroller/project-manager) | Project manager role: turns an owner's requests into work packages, staffs each role-first, records and holds the owner's standing rules, routes and unblocks agents, and reports status in the owner's terms. |
| [`game-designer`](https://github.com/opsroller/game-designer) | Game designer: documents how a game plays, designs levels and progression, balances difficulty with simulation, and sets feel targets. |
| [`gameplay-programmer`](https://github.com/opsroller/gameplay-programmer) | Gameplay programmer: implements game rules and systems as deterministic, tested code with a clean boundary to the engine. |
| [`graphics-programmer`](https://github.com/opsroller/graphics-programmer) | Graphics programmer: builds what the player sees in real time: scenes, camera, lighting, animation driven by game events, input, and rendering performance: frame time and counts such as draw calls, triangles and memory. |
| [`technical-artist`](https://github.com/opsroller/technical-artist) | Technical artist: creates original 3D models, materials, textures and shaders, preferably by script, and runs the asset pipeline into the engine. |
| [`sound-designer`](https://github.com/opsroller/sound-designer) | Sound designer: creates original sound effects, music and ambience, and integrates them through a cue system with clean mixing. |
| [`ui-developer`](https://github.com/opsroller/ui-developer) | UI developer: builds menus, HUDs and screens that bind to game state, with clean navigation, localisation and accessibility. |
| [`devops-engineer`](https://github.com/opsroller/devops-engineer) | DevOps engineer: CI pipelines, cross-platform builds, releases from Conventional Commits, store submissions, and open-source license compliance and credits. |
| [`frontend-web-developer`](https://github.com/opsroller/frontend-web-developer) | Front-end web developer: builds fast, accessible static websites, such as a product's landing and download site, with platform detection, store links and credits. |
| [`graphic-designer`](https://github.com/opsroller/graphic-designer) | Graphic designer: owns visual identity and 2D design: logo, colour and type, app icons, store and marketing art, UI visual design and website visuals. |
| [`code-reviewer`](https://github.com/opsroller/code-reviewer) | Code reviewer: reviews pull requests for design, correctness, tests, security, performance and readability, with labelled comments and a clear verdict. |
| [`technical-writer`](https://github.com/opsroller/technical-writer) | Technical writer: plans, writes, reviews and maintains documentation using the Diataxis framework (tutorials, how-to guides, reference, explanation) and docs-as-code practice. |
| [`engineering-operations`](https://github.com/opsroller/engineering-operations) | Engineering operations: owns the team's cost, delivery health and reporting; reads every role's records, finds workflow problems and waste with a few read-only investigators, and checks that each improvement worked. |

## License

Copyright (C) 2026 the contributors. Licensed under the
GNU General Public License v2.0 or later (`GPL-2.0-or-later`); see `LICENSE`.
