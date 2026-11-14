# skillhub-mock-test-repository-good

A known-good SkillCentral skill in a public repository. The SkillCentral live
tests register it with no username and no personal access token, and expect it
to be adopted. It uses the plugin layout (ADR-074): the manifest is the root
`plugin.json`. Do not change the files without updating
`metadata.skillcentral.hash` in `plugin.json` (it covers every file except
`plugin.json` and `.git/`; `skillcentral hash --write` sets it) and raising
`version`.
