---
name: create-skill
description: Create a reusable skill from a conversation workflow, including frontmatter, stepwise logic, and validation.
---

Use when: a user asks to package a multi-step workflow or methodology into a new `SKILL.md` file.

1. Review the conversation history for a clear workflow:
   - Identify the step-by-step process being followed.
   - Locate decision points or branching logic.
   - Note quality criteria, completion checks, and any validation requirements.

2. If the workflow is not clear, ask the user:
   - What outcome should this skill produce?
   - Should it be workspace-scoped or personal?
   - Should it be a quick checklist or a full multi-step workflow?

3. Draft the new skill:
   - Choose a descriptive skill name and folder under `.agents/skills/`.
   - Create `SKILL.md` with YAML frontmatter containing `name` and `description`.
   - Write body content as a numbered workflow, including guidance for tool use, conditionals, and exit criteria.

4. Validate the skill file:
   - Confirm the file path is `.agents/skills/<skill-name>/SKILL.md`.
   - Verify the frontmatter is valid YAML with `---` delimiters.
   - Ensure `description` clearly states when the skill should be used.

5. Summarize the result:
   - State what the skill produces.
   - Suggest example prompts to invoke it.
   - Offer related customizations, such as companion prompts or file instructions.
