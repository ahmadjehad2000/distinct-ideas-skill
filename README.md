# Distinct Ideas

Distinct Ideas is a brainstorming skill for Claude Code, Codex, and other AI agents. Use it when the agent keeps pitching variations of an idea you already rejected, or when you suspect it has misunderstood the problem.

The skill asks two questions before recommending an idea. **What did the user actually require, and what did the agent assume? Would the proposed alternatives lead anyone to run different experiments?** Bring it a failed attempt or an awkward detail from the real situation. That gives it something to build on in the next round.

[Download the skill](https://github.com/ahmadjehad2000/distinct-ideas/releases/latest/download/distinct-ideas.zip) · [Inspect the skill file](SKILL.md) · [Try the comparison exercise](examples/challenge-check.md)

## Install

Extract the `distinct-ideas` folder from the release ZIP into the personal skills directory for your agent. It contains one Markdown file.

| Agent | Installed file | Start your prompt with |
| --- | --- | --- |
| Claude Code | `~/.claude/skills/distinct-ideas/SKILL.md` | `/distinct-ideas` |
| Codex | `~/.agents/skills/distinct-ideas/SKILL.md` | `$distinct-ideas` |

On Windows, `~` is your user profile. Open a fresh session if the command does not appear. For another assistant, attach [SKILL.md](SKILL.md) and ask it to apply the skill to your brief.

## See a recommendation change

> “Our community radio show needs new voices. We shortened the voicemail prompt. The same three people still call.”

In this fictional brief, an agent could suggest a pop-up recording booth. That makes sense if the editor needs **new people speaking on air**. But the producer has noticed something odd. At the market, people who never call the show will argue for ten minutes about a sound they recognize.

One question changes the assignment: **Would a first-time contributor's words, read by the host with permission, count?**

| The editor's answer | What to try one market morning | What would make you reconsider |
| --- | --- | --- |
| “Yes. We need a local perspective we haven't aired.” | Play the sound at the stall. Put the producer's guess on a card and invite corrections. Let contributors choose whether the host may read their words anonymously. | People leave corrections, but nobody gives permission to air them. The format attracted interest and still left the editor without a usable contribution. |
| “We need listeners to hear the contributor's own voice.” | Let a volunteer record a short correction, hear it back, and decide whether the show may use it. | People are happy to discuss the sound but consistently decline recording. A more polished booth would still face the same obstacle. |

That last observation is worth bringing back to the agent. Ask which part of the idea survived, which premise failed, and what it would try differently.

## Use it on your own brief

> We want **[observable outcome]** for **[person]**. We've tried **[approach]**, and **[what happened]**. One detail that doesn't fit our explanation is **[observation]**. Challenge your first reading. Show me one idea that depends on this detail, what I could try this week, and what result would make you drop it.

A useful follow-up can be one sentence: *“People used it, but the outcome stayed the same. Which assumption should we revisit first?”*

## Judge it for yourself

Try the same brief in two fresh sessions of one model, then give both the same new evidence. Compare which answer preserves your requirements, changes its recommendation when warranted, and offers an experiment you would actually run. The repository includes a ready-to-use brief with three alternative follow-ups. [Two-round comparison exercise](examples/challenge-check.md)

The method draws on Innovation Training's work on challenge framing, human-first brainstorming, and blind selection. Distinct Ideas adds comparison with prior suggestions, a check on the agent's interpretation, and a way to revisit ideas after a trial. [AI for Ideation](https://www.innovationtraining.org/how-to-use-ai-to-generate-ideas/)
