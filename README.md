# opsroller Claude plugins

A catalog of job-function plugins. Each one is a role a person could hold on any team, with the skills that job needs. Every plugin lives in its own repository and is versioned on its own; this repo only lists them.

| Plugin | Job |
|---|---|
| [`engineering-practices`](https://github.com/opsroller/engineering-practices) | Shared working practices for every role: project onboarding, git with Conventional Commits, work packages, talking to other agents, and asset and code provenance. |
| [`game-designer`](https://github.com/opsroller/game-designer) | Game designer: documents how a game plays, designs levels and progression, balances difficulty with simulation, and sets feel targets. |
| [`gameplay-programmer`](https://github.com/opsroller/gameplay-programmer) | Gameplay programmer: implements game rules and systems as deterministic, tested code with a clean boundary to the engine. |
| [`graphics-programmer`](https://github.com/opsroller/graphics-programmer) | Graphics programmer: builds what the player sees in real time: scenes, camera, lighting, animation driven by game events, input, and rendering performance. |
| [`technical-artist`](https://github.com/opsroller/technical-artist) | Technical artist: creates original 3D models, materials, textures and shaders, preferably by script, and runs the asset pipeline into the engine. |
| [`sound-designer`](https://github.com/opsroller/sound-designer) | Sound designer: creates original sound effects, music and ambience, and integrates them through a cue system with clean mixing. |
| [`ui-developer`](https://github.com/opsroller/ui-developer) | UI developer: builds menus, HUDs and screens that bind to game state, with clean navigation, localisation and accessibility. |
| [`devops-engineer`](https://github.com/opsroller/devops-engineer) | DevOps engineer: CI pipelines, cross-platform builds, releases from Conventional Commits, store submissions, and open-source license compliance and credits. |
| [`frontend-web-developer`](https://github.com/opsroller/frontend-web-developer) | Front-end web developer: builds fast, accessible static websites, such as a product's landing and download site, with platform detection, store links and credits. |
| [`graphic-designer`](https://github.com/opsroller/graphic-designer) | Graphic designer: owns visual identity and 2D design: logo, colour and type, app icons, store and marketing art, UI visual design and website visuals. |
| [`code-reviewer`](https://github.com/opsroller/code-reviewer) | Code reviewer: reviews pull requests for design, correctness, tests, security, performance and readability, with labelled comments and a clear verdict. |

## Use

```
/plugin marketplace add opsroller/claude-plugins
/plugin install engineering-practices@opsroller
/plugin install gameplay-programmer@opsroller
```

A project tells a role *what* to work with in its own `CLAUDE.md` and project profile: stack, commands, paths, contracts. Roles never name a project or a technology they depend on.

## Adding a role

Add one only when work needs a job function no role covers. Create its own repo with `.claude-plugin/plugin.json`, `agents/<role>.md` and `skills/`, keep it free of project and stack specifics, then add a line here as `feat: add <role>`.
