# skillhub-mock-test-repository-good

A known-good SkillCentral skill in a public repository. The SkillCentral live
tests register it with no username and no personal access token, and expect it
to be adopted. It is an Agent Plugins 1.0.0 plugin (SkillCentral ADR-081, ADR-106): the
manifest is the root `plugin.json`, and the skill is
`skills/skillhub-mock-test-repository-good/SKILL.md`. Do not change the files
without updating `extensions["io.skillcentral"].hash` in `plugin.json` (it
covers every file except `plugin.json` and `.git/`; `skillcentral hash --write`
sets it) and raising `version`.
