# todoist-cli — OpenClaw Skill

An [OpenClaw](https://openclaw.ai) agent skill for managing Todoist using the **official Doist CLI** (`@doist/todoist-cli`).

## Requirements

- Node.js + npm
- A [Todoist API token](https://todoist.com/app/settings/integrations/developer)

## Installation

Install the CLI:

```bash
npm install -g @doist/todoist-cli
```

Set up your API token:

```bash
export TODOIST_API_TOKEN="your-token"
# or
td auth token "your-token"
```

## What This Skill Does

Gives your OpenClaw agent full access to Todoist via the `td` CLI. Covers:

- **Tasks** — view today, add, complete, update, delete, reschedule, move
- **Projects** — list, create, archive, delete
- **Labels & Sections** — full management
- **Reminders** — add and manage task reminders
- **Comments** — add and view comments on tasks
- **Activity & Stats** — view logs, karma, and productivity stats
- **Upcoming** — see tasks for the next N days
- **Completed** — review what you've done

## Quick Examples

```bash
td today                                        # What's due today
td task add "Review PR" --due "today" --priority p1 --project "Work"
td task complete <ref>                          # Mark as done
td upcoming 7                                   # Next 7 days
td task list --filter "p1 & overdue"           # Overdue priority 1 tasks
td stats                                        # Karma + productivity
```

## Skill File

The `SKILL.md` contains full command reference and usage examples for the AI agent.

## License

MIT
