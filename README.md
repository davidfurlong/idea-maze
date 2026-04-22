# idea-maze

Ruthless idea triage for deciding what to try now, keep searching on, or discard.

This skill is for startup ideas, idea lists, and "which idea should I try?"
questions. It pushes hard on problem clarity, buyer pain, market reality,
bundling risk, and whether an idea is actually a company-sized opportunity or
just a feature.

## Install

Recommended:

```bash
npx skills add davidfurlong/idea-maze@idea-maze
```

Manual Codex install:

```bash
git clone https://github.com/davidfurlong/idea-maze.git ~/.codex/skills/idea-maze
```

Restart Codex after installing so the new skill is picked up.

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
