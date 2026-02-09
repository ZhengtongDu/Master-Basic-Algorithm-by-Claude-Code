# Summarize Session Command

Review the entire conversation history and update CLAUDE.md with relevant information.

## Steps

1. **Check compact status:**
   - Ask the user: "Have you already run the `/compact` command?"
   - If YES: proceed to step 2 and use the compacted conversation context for analysis
   - If NO: suggest the user to interrupt this `/summarize` command, run `/compact` first, then run `/summarize` again. Stop here and do not proceed with the remaining steps.

2. **Read current CLAUDE.md** to understand existing structure and content

3. **Analyze what should be added:**
   - New tasks discovered → add to "Todolist"
   - Completed work → add to "Done Tasks" with date
   - Important findings or patterns → add to relevant sections
   - Temporary notes or context → add to "Temporary Interaction Area"

4. **Present summary to user:**
   - Show a brief summary of the conversation
   - List proposed changes to CLAUDE.md
   - Ask for user confirmation before making changes

5. **After user approval**, update CLAUDE.md with the confirmed changes

## Guidelines

- Do NOT duplicate existing information
- Keep entries concise and actionable
- Use consistent formatting with existing content
- Preserve all existing content unless explicitly told to remove
- Add date stamps to completed tasks (format: YYYY-MM-DD)
