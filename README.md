# Multi Social - AI Content Skills

A collection of 10 skills for planning, producing and distributing social content.

## Skills

| Skill | Purpose | Location |
| --- | --- | --- |
| multi-social | Bilingual multi-platform distribution | [SKILL.md](SKILL.md) |
| ai-content-pipeline | End-to-end production workflow | [Skill](skills/ai-content-pipeline/SKILL.md) |
| ai-topic-plan | Topic selection grounded in real experience | [Skill](skills/ai-topic-plan/SKILL.md) |
| ai-video-script | Spoken scripts and shooting plans | [Skill](skills/ai-video-script/SKILL.md) |
| ai-talking-edit | Talking-head editing and subtitles | [Skill](skills/ai-talking-edit/SKILL.md) |
| ai-point-motion | Motion graphics for spoken points | [Skill](skills/ai-point-motion/SKILL.md) |
| cover-generate | Bilingual multi-format covers | [Skill](skills/cover-generate/SKILL.md) |
| baoyu-xhs-images | Xiaohongshu image cards | [Skill](skills/baoyu-xhs-images/SKILL.md) |
| baoyu-infographic | Infographics | [Skill](skills/baoyu-infographic/SKILL.md) |
| hypit | AI video production | [Skill](skills/hypit/SKILL.md) |

## Installation

Clone this repository, then copy the skills you need into your user skills folder.
Review existing installations before replacing files. The original root-level
multi-social entry remains compatible with existing users.

```bash
git clone https://github.com/chenkan0617chris/multi-social.git
mkdir -p ~/.codex/skills/multi-social
cp multi-social/SKILL.md ~/.codex/skills/multi-social/
cp -R multi-social/agents ~/.codex/skills/multi-social/
# Example: install the complete workflow and topic planner.
cp -R multi-social/skills/ai-content-pipeline ~/.codex/skills/
cp -R multi-social/skills/ai-topic-plan ~/.codex/skills/
# Repeat for other desired directories under skills/.
```

## Usage and dependencies

Ask the agent to use a skill by name. Start with ai-topic-plan for ideas,
ai-video-script for scripts, or ai-content-pipeline for the full workflow.
The full workflow calls the individual skills; install those you intend to use.

Several production skills require the ChatCut plugin, an available image-generation
backend, or the Hypit runtime. Installing these files does not install external
services or grant accounts, API access, credits or publishing permission.

Default content location: ~/Documents/Social Media. Personal style preferences
and Sydney timezone defaults remain documented in the skills and can be overridden.
Distribution always follows the user's authorization for the specific content.

## Source and licenses

Local skill snapshot: 2026-10-12. Personal workflow skills and the root distribution
skill use the repository [MIT license](LICENSE).

Third-party skills retain their own licenses, which override the root license
for those directories:

- baoyu-xhs-images and baoyu-infographic: [JimLiu/baoyu-skills](https://github.com/JimLiu/baoyu-skills), MIT. See each directory's LICENSE and UPSTREAM.md.
- hypit: [hypit-ai/hypit](https://github.com/hypit-ai/hypit), modified Apache 2.0 with additional conditions. See [its license](skills/hypit/LICENSE).

Other installed marketing, programming, system and plugin skills are not bundled
here. The separate private local-skills repository remains the full local backup.
