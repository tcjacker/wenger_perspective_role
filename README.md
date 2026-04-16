# Wenger Perspective Role

`wenger-perspective` is a Codex skill that answers football questions in an Arsene Wenger-inspired interview voice.

The skill is tuned for football analysis first. It prioritizes match review, player and transfer judgment, club building, coaching, and refereeing or game-management questions. Recent revisions also push the voice away from polished essay writing and toward spoken interview cadence.

## Features

- Wenger-like interview voice with stronger football context
- Question routing for match analysis, player or transfer evaluation, and club building
- Research-first guidance for real teams, players, matches, coaches, and news cycles
- Example answers that calibrate tone, pacing, and recurring Wenger-style phrases
- Explicit guards against over-literary phrasing and legalistic refereeing language

## Repository Layout

```text
.
├── LICENSE
├── README.md
├── SKILL.md
└── references
    ├── examples
    │   └── interview-examples.md
    └── research
        ├── 01-writings.md
        ├── 02-conversations.md
        ├── 03-expression-dna.md
        ├── 04-external-views.md
        ├── 05-decisions.md
        └── 06-timeline.md
```

## Install

### Option 1: Copy into Codex skills

Clone this repository, then copy the folder into your local Codex skills directory:

```bash
git clone https://github.com/tcjacker/wenger_perspective_role.git
cp -R wenger_perspective_role ~/.codex/skills/wenger-perspective
```

Restart Codex after copying the files.

### Option 2: Replace an existing local version

If you already have a local `wenger-perspective` skill:

```bash
cp -R wenger_perspective_role/. ~/.codex/skills/wenger-perspective
```

Restart Codex after updating the files.

## Usage

Invoke the skill when you want football analysis in Wenger's voice. Useful prompts include:

- `用温格的方式分析这场比赛`
- `温格会怎么看这笔转会`
- `How would Wenger assess this young midfielder`
- `What would Wenger say about this referee decision`

The skill is designed to:

1. Route the question into the right football lane
2. Research current facts when the topic is real and time-sensitive
3. Apply Wenger-style judgment models
4. Answer in a spoken, interview-like voice

## What This Skill Optimizes For

- Football-first analysis rather than generic management commentary
- Spoken explanation over polished prose
- Repeated anchor phrases such as `you have to remember`, `the context is important`, and `we had quality, but...`
- Common-sense football language instead of legalistic or referee-manual language

## Development Notes

This repository contains both the main skill and the supporting calibration material.

- `SKILL.md` defines routing, research behavior, voice rules, and hard constraints.
- `references/examples/interview-examples.md` calibrates how the answers should sound.
- `references/research/` stores the supporting source notes used to shape the skill.

When editing the skill, keep the voice grounded in spoken football analysis. If a revision starts sounding like a polished column, a legal memo, or a generic motivational coach, it has drifted.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE).
