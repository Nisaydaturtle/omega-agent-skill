# Ω OMÉGA

[![Install via skills.sh](https://skills.sh/b/Nisaydaturtle/omega-agent-skill)](https://skills.sh/Nisaydaturtle/omega-agent-skill)

### Your idea shouldn't need an expert vocabulary.

**An Agent Skill that helps your AI ask the questions you didn't know to ask.**

[Français](README.fr.md) · [The skill](skills/omega/SKILL.md) · [Example conversations](examples.md) · [V1 checks](evaluation.md) · [Launch copy](launch-copy.md)

You know what you want to achieve. You may not know the language of lighting, software architecture, typography, or access control. OMÉGA helps an assistant bridge that gap through a guided conversation.

It starts with your intention, explains the choices that matter, uncovers overlooked requirements, and turns the answers into an actionable brief.

## What changes

| You say | OMÉGA helps clarify |
| --- | --- |
| “I want a woman in the rain.” | The purpose, emotion, visual treatment, weather, framing, and light—through examples you can recognize. |
| “I want an app for my clients.” | The real workflow, who can see what, what “payments” means, recovery needs, and a useful first version. |
| “Make this video dynamic.” | Whether you mean faster cuts, moving text, camera motion, subject movement, or sound. |
| “What is drizzle?” | A direct answer. No unnecessary interview. |

## How it works

1. **Understand the territory.** Identify the main domain and relevant adjacent disciplines.
2. **Make choices understandable.** Explain effects before technical terms.
3. **Ask progressively.** Usually one to three focused questions at a time, with deeper rounds when wanted.
4. **Expose blind spots.** Surface relevant requirements the user would not know to mention.
5. **Produce a usable brief.** Separate confirmed intent, recommendations, assumptions, and success checks.
6. **Know when to stop asking.** Move to the requested deliverable when enough is clear.

The user owns the intention. The assistant proposes the technical translation and explains consequential tradeoffs.

## Try it

**Quick install** with the skills CLI:

```bash
npx skills add Nisaydaturtle/omega-agent-skill --skill omega
```

Or install the complete [`skills/omega`](skills/omega) folder using your Agent Skills-compatible client's supported method. Keep `SKILL.md`, `references/`, and `agents/` together. The CLI can report anonymous installation counts to skills.sh; set `DISABLE_TELEMETRY=1` to opt out.

Then invoke OMÉGA through your client's skill selector, with a request like:

> Use OMÉGA. I want to design an app for my small business, but I don't know what to specify. Help me discover the important choices before writing the brief.

Or:

> Use OMÉGA to help me prepare an image brief. I have an atmosphere in mind but don't know the vocabulary. Explain options with concrete examples.

For a client without skill support, paste the contents of `SKILL.md` and the relevant reference material into the conversation. This provides the guidance manually; it does not add automatic skill loading or tool access.

## What's included

- `SKILL.md`: the adaptive discovery workflow and stopping rules.
- `references/domain-lenses.md`: examples for images, applications, video, writing, learning, and business decisions.
- `references/brief-template.md`: a flexible handoff structure.
- `agents/openai.yaml`: display metadata for clients that support it.

The instructions are written in English for portability and direct the assistant to respond in the user's language. No API key, executable script, external service, or paid dependency is bundled with this skill. A host model and any tools needed for the actual task remain necessary.

## What V1 does—and what remains to prove

OMÉGA structures a conversation. It does not retrain the model, supply universal domain expertise, guarantee correct answers, or override the host's instructions. Some hosts require immediate execution; their rules take precedence over interviewing.

V1 has undergone a small qualitative check covering image discovery, application discovery, brief handoff, and a direct factual follow-up. See [evaluation.md](evaluation.md). Cross-model performance and improved final outcomes have **not** been established by a benchmark.

If you try it, share an anonymized example of where the questions helped—or got in the way. Useful feedback includes the initial request, client/model, relevant exchange, and what should have happened. Never post credentials or private customer data.

## Version and license

**V1 · 0.1.0** · Created by [Nisaydaturtle](https://github.com/Nisaydaturtle).

Released under the [MIT License](LICENSE).
