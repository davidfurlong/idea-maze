# idea-maze

Ruthless idea triage for deciding what to try now, keep searching on, or discard.

This skill is for startup ideas, idea lists, and "which idea should I try?"
questions. It pushes hard on problem clarity, buyer pain, market reality,
bundling risk, and whether an idea is actually a company-sized opportunity or
just a feature.

This repo ships the raw skill source as `SKILL.md`, so you can install it in
agent tools that support the Agent Skills format or upload it into products that
support skill import.

## Install

### skills.sh / npx skills

```bash
npx skills add https://github.com/davidfurlong/idea-maze.git --skill idea-maze -g
```

This is the most portable option if you use the open agent-skills ecosystem.
Discoverable packages and install flows live at [skills.sh](https://skills.sh/).

### Claude Code

Using `npx skills`:

```bash
npx skills add https://github.com/davidfurlong/idea-maze.git --skill idea-maze -g
```

Manual install:

```bash
git clone https://github.com/davidfurlong/idea-maze.git ~/.claude/skills/idea-maze
```

Restart Claude Code after installing.

### Codex

Using `npx skills`:

```bash
npx skills add https://github.com/davidfurlong/idea-maze.git --skill idea-maze -g
```

Manual install:

```bash
git clone https://github.com/davidfurlong/idea-maze.git ~/.codex/skills/idea-maze
```

Restart Codex after installing.

### OpenClaw

Manual global install:

```bash
git clone https://github.com/davidfurlong/idea-maze.git ~/.openclaw/skills/idea-maze
```

Manual workspace install:

```bash
git clone https://github.com/davidfurlong/idea-maze.git ./skills/idea-maze
```

Start a new OpenClaw session after installing. This repo is not on ClawHub yet,
so there is not an `openclaw skills install ...` command for it yet.

### ChatGPT

ChatGPT has a native skills flow, but it is not a direct GitHub install.

1. Open ChatGPT.
2. Open your profile menu and go to `Skills`.
3. Click `New skill`.
4. Choose `Upload from your computer`.
5. Upload `SKILL.md` from this repo and install it.

ChatGPT Skills are currently available in beta on ChatGPT Business, Enterprise,
Edu, Teachers, and Healthcare plans.

### Claude

Claude web/Desktop does not have the same native `SKILL.md` install flow as
ChatGPT. The closest setup is to use a Claude Project:

1. Create a new Project.
2. Upload `SKILL.md` to the project's knowledge.
3. Paste the workflow into Project instructions, or ask Claude to adapt the
   uploaded file into project instructions.
4. Use that project whenever you want idea triage.

If you want a true installable skill workflow, use Claude Code or `npx skills`.

## Use

Invoke the skill with `$idea-maze`.

If you trigger it without idea content, it will ask:

```text
Paste one idea or a bullet list of ideas.
```

Example prompts:

```text
$idea-maze

$idea-maze
- AI tool for SDR onboarding
- software for restaurant shift handoffs
- compliance workflow for small clinics
```

## Output

The skill produces a decision memo, not an implementation plan. Its default
posture is to kill weak ideas fast and keep only the ones with real pain and a
credible path to value.
