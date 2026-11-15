# Your Own Skill

Project 16 from the BSERC Week 2 brief. This project builds one local `/resume-roast` agent skill.

## Use the skill

The skill is at `.agents/skills/resume-roast/SKILL.md`. Open this project folder as the working folder in a new Codex session; the project-local `.agents/skills` directory keeps the skill with the project. Invoke it with `$resume-roast`, then provide both a resume and the job post to compare. The sample reviews in `examples.md` show its intended use.

This is an agent instruction skill, not a standalone phone app. On Android, you can read and copy the skill and prompt files from the project folder, but automatic skill discovery depends on an agent app that supports project-local skills. That was not verified on Android.

## Done when

- [x] The skill instructions and discovery metadata are included.
- [x] The skill is rehearsed on three different fictional inputs in `examples.md`.
- [x] `comparison.md` shows the same task before and after applying the skill.
- [x] Skill frontmatter, metadata, and three-example coverage were manually checked.

The bundled skill validator could not run here because its PyYAML dependency is not installed. A fresh Codex session smoke test also could not run: the local CLI reported that it could not find the Codex home directory. No dependencies were installed to work around those environment limits.
