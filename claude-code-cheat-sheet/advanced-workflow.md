# Advanced workflow: a controlled first coding task

This is an original coaching guide, not a command catalog. Check the official Claude Code documentation for current installation, commands, supported systems, sign-in, and permissions. The user needs Claude Code installed and authenticated through a supported plan or provider; usage limits and billing depend on that setup.

1. Ask what outcome the user wants, which repository/files are in scope, what must remain untouched, what tools or integrations are needed, and any time or usage limit. Never ask for passwords, API keys, or recovery codes.
2. Inspect the smallest relevant area. Summarize the task and likely file changes before acting. For a plan-first session, consult the current CLI documentation for plan permission mode.
3. Review the proposed commands, file access, and tool permissions. Keep access narrow and use the normal permission prompts. Never recommend bypassing permission checks as a shortcut.
4. Work only in the approved scope. Preserve existing work; before an operation with broad or irreversible effects, explain its impact and follow the user's instruction and tool safeguards.
5. Run checks appropriate to the change, then report files changed, checks run, results, and anything unverified. Show a diff or clear review path.

Official sources are linked in `original-replacement-reference.md`. Commands and permission behavior can change; verify them against current documentation before use.
