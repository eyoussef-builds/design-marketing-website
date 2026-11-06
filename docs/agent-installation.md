# Step-by-step installation for 15 agents

[العربية](agent-installation.ar.md) · [Main explanation](../README.md)

Think of the skill as a small instruction book. We download it, put it on the shelf your assistant knows about, then ask the assistant to read it. You do not need to edit code.

## 1. Download the folder once

1. Open [this repository](https://github.com/eyoussef-builds/design-marketing-website).
2. Click the green **Code** button, then **Download ZIP**.
3. Extract the ZIP. Open the extracted folder containing `README.md` and `skills`.
4. Check that `skills/design-marketing-website/SKILL.md` exists. Install the complete `design-marketing-website` folder with its references, templates and scripts, not just `SKILL.md`.
5. Choose your agent below. Install one copy in one location; you do not need every directory.

Or, if Git is installed, open Terminal or PowerShell in a suitable download folder and run:

```sh
git clone https://github.com/eyoussef-builds/design-marketing-website.git
cd design-marketing-website
```

This is a local skill-folder package, not a registered marketplace plugin. You need one installed, signed-in agent, not all 15.

## 2. How to copy it

**Without commands:** each agent's destination is below. `~` means your own home folder, not a particular person's username. On macOS, use Finder → **Go → Go to Folder**. On Linux, use your file manager and reveal hidden folders if needed. On Windows, open your user folder and create the directories shown by the PowerShell path. If the destination does not exist, create its parent directories inside your own home folder first. Copy the complete skill folder there. If a copy exists, compare it before replacing it.

**With commands:** open a terminal in the extracted repository folder. In your agent's section, choose the macOS/Linux or PowerShell destination line. Run it, then run the matching copy block below in **the same terminal window**.

macOS / Linux, after setting `dest_parent` from your agent's section:

```sh
if [ -e "$dest_parent/design-marketing-website" ] || [ -L "$dest_parent/design-marketing-website" ]; then
  echo "Already installed. Compare your existing copy before updating."
else
  mkdir -p "$dest_parent" && cp -R "skills/design-marketing-website" "$dest_parent/"
fi
```

Windows PowerShell, after setting `$destParent` from your agent's section:

```powershell
$skillDest = Join-Path $destParent 'design-marketing-website'
if (Test-Path -LiteralPath $skillDest) { throw 'Already installed. Compare before updating.' }
New-Item -ItemType Directory -Force -Path $destParent | Out-Null
Copy-Item -LiteralPath 'skills/design-marketing-website' -Destination $destParent -Recurse
```

“Already installed” means the old copy was not updated. Save your modifications and compare the two versions first. The final folder must contain `design-marketing-website/SKILL.md` directly, not another nested folder with the same name.

The available linked official documentation was reviewed on 2026-11-06, with the Windsurf exception explained below. That is documentation verification, not a claim of end-to-end testing in all 15 agents. Versions and organization policies may differ. Reopen the session or reload skills if needed.

**Compatibility boundary:** this is an instruction-and-template skill. Planning needs readable product context; implementation needs repository/file tools and the project's actual runtime; visual QA needs a browser. Optional external builders/design skills have separate requirements and costs. Installing this folder adds no tools, accounts or hosting. The instructions and package were reviewed here; full website execution has not been tested across all 15 agents. The Windsurf documentation could not be retrieved during this review, so that entry uses explicit reading rather than asserting a current native path.

## 1. OpenAI Codex

1. Use the personal destination: `~/.agents/skills/design-marketing-website/`.
2. Run your system's line, then the copy block in step 2 above:

```sh
dest_parent="$HOME/.agents/skills"
```

```powershell
$destParent = Join-Path $HOME '.agents/skills'
```

3. In Codex CLI/IDE, type `$design-marketing-website` or select it with `/skills`. In the desktop picker, select the installed skill. Project alternative: `.agents/skills/design-marketing-website/`.

[Official documentation](https://developers.openai.com/codex/skills/).

## 2. Claude Code

1. Use the personal destination: `~/.claude/skills/design-marketing-website/`.
2. Run your system's line, then the copy block in step 2 above:

```sh
dest_parent="$HOME/.claude/skills"
```

```powershell
$destParent = Join-Path $HOME '.claude/skills'
```

3. Type `/design-marketing-website` followed by your request. Project alternative: `.claude/skills/design-marketing-website/`. This local installation does not automatically install the skill into Cowork or cloud sessions.

[Official documentation](https://code.claude.com/docs/en/skills).

## 3. OpenClaw

1. From the downloaded repository, run:

```sh
openclaw skills install ./skills/design-marketing-website --as design-marketing-website
openclaw skills list
openclaw skills check
```

2. Review trust warnings rather than bypassing them. Confirm installation targets the intended configured agent workspace; use the official CLI agent-selection options when you have several.
3. Ask to use `design-marketing-website` and verify discovery. A remote Gateway needs the files and tools in its own execution environment.

[Official documentation](https://docs.openclaw.ai/cli/skills).

## 4. Hermes Agent

1. In your terminal, run:

```sh
hermes skills install eyoussef-builds/design-marketing-website/skills/design-marketing-website
```

2. Review the community-skill scan and keep normal security checks enabled.
3. Ask Hermes to list skills, then use `design-marketing-website`. Default manual destination: `~/.hermes/skills/design-marketing-website/`; custom profiles may differ.

[Official documentation](https://hermes-agent.nousresearch.com/docs/user-guide/features/skills/).

## 5. Cursor

1. Use the personal destination: `~/.cursor/skills/design-marketing-website/`.
2. Run your system's line, then the copy block in step 2 above:

```sh
dest_parent="$HOME/.cursor/skills"
```

```powershell
$destParent = Join-Path $HOME '.cursor/skills'
```

3. In Agent chat type `/` and choose `design-marketing-website`. Project alternative: `.cursor/skills/design-marketing-website/`. Local personal skills need separate supported sync/configuration to reach a cloud worker.

[Official documentation](https://cursor.com/docs/skills).

## 6. Grok Bot

1. This is an **instruction adaptation**, not verified native `SKILL.md` import. Open the Bot and provide this repository link.
2. Ask it to read `skills/design-marketing-website/SKILL.md` and relevant references, then save the method as a private skill called `design-marketing-website`. Retain supporting files if the host supports them.
3. Verify the saved skill in private-skill/plugin management, enable it for the current Bot if required, and select it with `/` where available. If it cannot read the folder, use the explicit-read fallback below.

[Official documentation](https://docs.x.ai/grok-bot/skills-routines-and-automations).

## 7. OpenCode

1. Use the personal destination: `~/.config/opencode/skills/design-marketing-website/`.
2. Run your system's line, then the copy block in step 2 above:

```sh
dest_parent="$HOME/.config/opencode/skills"
```

```powershell
$destParent = Join-Path $HOME '.config/opencode/skills'
```

3. Ask it to load `design-marketing-website` through its skill tool. Project alternative: `.opencode/skills/design-marketing-website/`. Check the skill name is listed and its references are readable.

[Official documentation](https://opencode.ai/docs/skills/).

## 8. GitHub Copilot

1. Use the personal destination: `~/.copilot/skills/design-marketing-website/`.
2. Run your system's line, then the copy block in step 2 above:

```sh
dest_parent="$HOME/.copilot/skills"
```

```powershell
$destParent = Join-Path $HOME '.copilot/skills'
```

3. Use a supported local IDE Agent or Copilot CLI and ask for `design-marketing-website`. Project alternative: `.github/skills/design-marketing-website/`. Product/version and organization policies affect discovery; a cloud agent cannot read your local files automatically.

[Official documentation](https://docs.github.com/en/copilot/concepts/customizations/agent-skills).

## 9. Gemini CLI

1. Use the personal destination: `~/.gemini/skills/design-marketing-website/`.
2. Run your system's line, then the copy block in step 2 above:

```sh
dest_parent="$HOME/.gemini/skills"
```

```powershell
$destParent = Join-Path $HOME '.gemini/skills'
```

3. Run `/skills list` in the agent, then ask it to use `design-marketing-website`. Reload with `/skills reload` if needed. Project alternative: `.gemini/skills/design-marketing-website/`. Keep normal skill activation consent enabled.

[Official documentation](https://geminicli.com/docs/cli/skills/).

## 10. Windsurf / Cascade / Devin Desktop

1. Open the downloaded repository in your workspace.
2. Use the explicit-read prompt below, naming `skills/design-marketing-website/SKILL.md` and keeping its references/assets accessible.
3. Ask the agent to summarize the brief/build distinction before starting. This is an instruction-reading adaptation for this release; check the [current official setup](https://docs.windsurf.com/windsurf/cascade/skills) for native installation in your installed version. The documentation could not be retrieved during this review.

## 11. Cline

1. Use the personal destination: `~/.cline/skills/design-marketing-website/`.
2. Run your system's line, then the copy block in step 2 above:

```sh
dest_parent="$HOME/.cline/skills"
```

```powershell
$destParent = Join-Path $HOME '.cline/skills'
```

3. Open Cline, confirm skills are enabled in your version, and ask it to use `design-marketing-website`. Project alternative: `.cline/skills/design-marketing-website/`. Use a mode with the tools needed for the actual task.

[Official documentation](https://docs.cline.bot/customization/skills).

## 12. Roo Code

1. Use the personal destination: `~/.roo/skills/design-marketing-website/`.
2. Run your system's line, then the copy block in step 2 above:

```sh
dest_parent="$HOME/.roo/skills"
```

```powershell
$destParent = Join-Path $HOME '.roo/skills'
```

3. Ask Roo to load `design-marketing-website` using its skill tool. Project alternative: `.roo/skills/design-marketing-website/`. Use the generic skill root unless you intentionally want mode-specific scoping.

[Official documentation](https://roocodeinc.github.io/Roo-Code/advanced-usage/available-tools/skill/).

## 13. Aider

1. Use **read-only context**, not an assumed native skill installer. From the repository, run:

```sh
aider --read skills/design-marketing-website/SKILL.md
```

2. Add relevant reference files with `/read` and their paths under `skills/design-marketing-website/references/`; add helpers when needed.
3. Ask it to follow the skill with only authorized inputs. Reading text does not add missing chat tools, browser/build tools or execution permissions.

[Official documentation](https://aider.chat/docs/usage/tips.html).

## 14. Amp

1. Use the personal destination: `~/.agents/skills/design-marketing-website/`.
2. Run your system's line, then the copy block in step 2 above:

```sh
dest_parent="$HOME/.agents/skills"
```

```powershell
$destParent = Join-Path $HOME '.agents/skills'
```

3. Ask Amp to list/load `design-marketing-website`. Project alternative: `.agents/skills/design-marketing-website/`. Check your configuration has not disabled global agent-skills discovery.

[Official documentation](https://ampcode.com/docs/customize/skills).

## 15. Goose

1. Use the personal destination: `~/.agents/skills/design-marketing-website/`.
2. Run your system's line, then the copy block in step 2 above:

```sh
dest_parent="$HOME/.agents/skills"
```

```powershell
$destParent = Join-Path $HOME '.agents/skills'
```

3. Keep the Skills extension enabled. Check `goose skills list`, then use `/skills design-marketing-website` in chat. Project alternative: `.agents/skills/design-marketing-website/`. File/terminal work needs suitable tool extensions.

[Official documentation](https://github.com/aaif-goose/goose/blob/main/documentation/docs/guides/context-engineering/using-skills.md).

## 3. Check that it works

1. Start a new session or reload skills if it is missing.
2. Ask: “Can you see `design-marketing-website`? Read its instructions and tell me what you need before starting.”
3. Check it reads the complete skill folder rather than another similarly named file.
4. Use the first-task prompt in [the main explanation](../README.md). If a required tool is missing, the agent must say so rather than invent a successful result.

## Any other agent: explicit reading

Download/open the repository in a workspace the agent can read, then say:

```text
Read skills/design-marketing-website/SKILL.md and follow it for this task.
Read linked references when needed and inspect helpers before running them.
Respect my current permissions and explain unavailable tools or evidence.
```

For a chat-only agent, attach the entrypoint and necessary references if attachments are supported. That enables advice or planning, not access to your local computer. Share only the product facts needed for this site; keep credentials and unrelated business data private.

## Troubleshooting

| Problem | What to do |
| --- | --- |
| Skill does not appear | Check the supported directory, uppercase `SKILL.md`, and no extra nesting. Reload skills. |
| It does not trigger automatically | Name it explicitly or use the agent's own invocation control. |
| The installed copy is old | Compare versions and preserve modifications and your local profile before updating. |
| Two copies share a name | Keep the intended location and remove the duplicate after preserving changes. |
| A cloud session cannot see local files | Use a local environment or actually accessible authorized source; do not assume automatic sync. |
| Organization policy blocks skills | Use the supported setup with your administrator; do not bypass the restriction. |
| You want to uninstall | Remove only the installed `design-marketing-website` folder or use the agent's uninstall control; leave your project files alone. |

---

Created by [eyoussef-builds](https://github.com/eyoussef-builds) · [hello@eyoussef.me](mailto:hello@eyoussef.me) · [eyoussef.me](https://eyoussef.me)
