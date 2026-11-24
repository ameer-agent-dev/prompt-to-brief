# prompt-to-brief

Turn any rough prompt, messy idea, or vague request to an AI into a clear Four-Part Brief (Outcome, Context, Format, Constraints).
Works as an open Agent Skill in coding agents, as an uploaded skill in Claude.ai and ChatGPT, or by copy-pasting into any AI chat.

## 1. Install for Coding Agents

Install with one command in Claude Code, Codex, Cursor, OpenCode, Gemini CLI, or VS Code:

```bash
npx skills add ameer-agent-dev/prompt-to-brief
```

Once installed, ask your agent to improve, tighten, or write a prompt for a specific AI task.

## 2. Download ZIP for Claude.ai and ChatGPT

Download the ready-to-upload skill archive from the `v1.0.0` release:

- [Download prompt-to-brief.zip (v1.0.0)](https://github.com/ameer-agent-dev/prompt-to-brief/releases/download/v1.0.0/prompt-to-brief.zip)

### Upload to Claude.ai

1. Download `prompt-to-brief.zip` from the link above.
2. Open Claude.ai and go to **Settings > Capabilities > Skills**.
3. Click **Upload skill** and select `prompt-to-brief.zip`.
4. Turn the skill on, then paste any rough prompt and ask Claude to turn it into a brief.

### Upload to ChatGPT

1. Download `prompt-to-brief.zip` from the link above.
2. Open ChatGPT and go to **Settings > Skills** (or your workspace Skills page).
3. Click **Upload skill** (or **Add skill**) and select `prompt-to-brief.zip`.
4. Enable the skill and ask ChatGPT to rewrite or structure your prompt.

*Note: If your plan does not include skill uploads, use the copy-paste setup below.*

## 3. Copy-Paste Setup for Any Free AI Chat

You can use `prompt-to-brief` in Gemini, Claude.ai, ChatGPT, or any other free AI chat without installing anything:

1. Open [skills/prompt-to-brief/SKILL.md](skills/prompt-to-brief/SKILL.md) (or view the [raw file](https://raw.githubusercontent.com/ameer-agent-dev/prompt-to-brief/main/skills/prompt-to-brief/SKILL.md)) and copy everything below the top `---` header block.
2. Choose where to put it:
   - **Project Instructions or Custom Instructions:** Paste it once so the chat automatically rewrites prompts whenever you ask for prompt help, while answering normal questions as usual. (If your tool has a shorter character limit, use the chat-start option below.)
   - **Start of a chat:** Paste the instructions as your first message, followed by your rough prompt.

## 4. Before and After Example

*Illustrative sample (you can replace or expand this section with your own examples later).*

### Before (rough prompt)

```text
Act as a world-class email copywriter. Write a cold email to SaaS founders about my analytics tool and make it punchy and persuasive. Think step by step.
```

### After (Four-Part Brief)

```text
OUTCOME
Draft one cold outreach email introducing my analytics tool to SaaS founders and asking for a brief intro call. Done when the email is under 120 words, includes one specific value point and one clear call to action, and uses no unverified product claims.

CONTEXT
- Audience: SaaS founders.
- Product: [PLACEHOLDER: product name and 1-sentence description of what the analytics tool measures or fixes]
- Proof point: [PLACEHOLDER: one real metric, customer result, or concrete feature]
- Call to action: [PLACEHOLDER: desired next step, such as a 15-minute call or reply with a question]

FORMAT
Inline chat text: one subject line followed by the email body. Include a short "Unverified / Assumptions" section below the email if any detail could not be confirmed from the context above.

CONSTRAINTS
- Keep the tone direct, plain, and respectful of a busy founder's time.
- Keep the email body under 120 words.
- Do not invent customer names, metrics, pricing, or product features.
```

**What Changed & Fill In Before Running**
- Removed the empty expert title ("Act as a world-class email copywriter") and the manual "Think step by step" instruction.
- Added a testable "Done when" line, word limit, and output format.
- Replaced missing product details with explicit placeholders so the model does not invent claims.
- Fill in before running:
  - `[PLACEHOLDER: product name and 1-sentence description of what the analytics tool measures or fixes]`
  - `[PLACEHOLDER: one real metric, customer result, or concrete feature]`
  - `[PLACEHOLDER: desired next step, such as a 15-minute call or reply with a question]`

## License

MIT License. Copyright (c) 2026 ameer_dev. See [LICENSE](LICENSE).
