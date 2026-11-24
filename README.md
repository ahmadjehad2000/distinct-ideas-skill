# Distinct Ideas

A brainstorming skill for Claude Code, Codex, and other AI agents. Give it your problem, what you have already tried, and one detail about how the work actually happens. It returns a shortlist of ideas you could test differently, with a reason to try the first one and a reason to drop it.

**Would two suggestions lead you to run the same experiment?** An email reminder, a push notification, and an AI-written nudge can all depend on the same person remembering to act. Distinct Ideas groups those suggestions together and looks for another way the outcome could change.

[Download the skill](https://github.com/ahmadjehad2000/distinct-ideas/releases/latest/download/distinct-ideas.zip) · [Read the instructions](SKILL.md)

## See it on one problem

A tool library keeps missing Saturday drill reservations. Its team has already proposed a reminder app and a dashboard. Change one fact about the library and a different experiment makes sense.

| What happens on Friday | Idea to test | What to watch on Saturday |
|---|---|---|
| Borrowers arrive after the tool counter closes. The book desk stays open and already stores locked cases overnight. | With the desk's agreement, accept one evening of drill returns in numbered cases. Keep the usual inspection before checkout. | How many booked drills are ready on time? How many minutes of work moved to the book desk? |
| Borrowers return drills on time. Missing chargers turn up at pickup, after the parts counter has closed. | Check the drill and charger together with the borrower at handback, while a missing item can still be recovered. | How many incomplete kits were fixed on Friday? Did that save any Saturday reservations? |

These are fictional briefs. Both ideas have a cheap test, and either can fail for a reason the library can observe.

## Try it

> We need Saturday drill reservations to start on time. We already tried text reminders. Borrowers often arrive after our counter closes, but the book desk stays open two hours later. We have one volunteer shift and no budget for more drills. Give me three ideas that work in different ways. Which one would you test on Friday, and what would persuade you to drop it?

For your own brief, replace the drill story with a real workaround, exception, or constraint. Include rejected ideas and why they fell short. On a second round, tell the agent which mechanisms to set aside and what you learned since the first round.

## Install

Download the [release ZIP](https://github.com/ahmadjehad2000/distinct-ideas/releases/latest/download/distinct-ideas.zip) and extract its `distinct-ideas` folder into the location for your agent. The installed file should end in `distinct-ideas/SKILL.md`.

| Agent | Personal skill directory | Invoke |
|---|---|---|
| Claude Code | `~/.claude/skills/` | `/distinct-ideas` followed by your brief |
| Codex | `~/.agents/skills/` | `$distinct-ideas` followed by your brief |
| Another agent | Its supported skills directory, or attach [SKILL.md](SKILL.md) to the conversation | Ask it to apply Distinct Ideas to your brief |

On Windows, `~` means your user profile. Start a fresh agent session if the skill does not appear. The skill itself is one Markdown file and requires no API keys, scripts, or external services.

## Where the method comes from

Challenge framing, human-first brainstorming, and blind selection draw on Innovation Training's guide. This skill adds a record of prior ideas, a comparison of how each proposal would work, and a check for whether the idea still makes sense when the most distinctive local fact is removed. These checks help assess originality relative to the alternatives you supplied. Market novelty needs its own research. [AI for Ideation](https://www.innovationtraining.org/how-to-use-ai-to-generate-ideas/)
