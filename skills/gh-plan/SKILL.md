---
name: gh-issue-plan
description: Refine a GitHub issue with a detailed implementation plan and checklist
license: MIT
---

## What I do
- Analyze GitHub issues to understand requirements
- Explore the codebase to identify affected components
- Create a comprehensive implementation plan with checklist

## When to use me
Use this skill when you need to create a comprehensive implementation plan for a GitHub issue. You should have the issue number available.

## Instructions

1. Fetch the current issue content:
   `gh api repos/[GITHUG_USER]/[GITHUB_REPO]/issues/$1 | jq -r '"### \(.title)\n\(.body)"'`

2. Analyze the issue to understand:
   - What problem needs to be solved
   - What features or fixes are requested
   - Any constraints or requirements mentioned
   - Ask clarifying questions if needed

3. Explore the codebase thoroughly to:
   - Identify all files and components that will need changes
   - Understand the existing architecture and patterns
   - Find related code, tests, and dependencies
   - Note any potential challenges or edge cases

4. Create a comprehensive implementation plan that includes:
   - A clear summary of the approach
   - Step-by-step breakdown of changes needed
   - Files to be created or modified
   - Any database migrations required
   - Test coverage requirements
   - Always create a decisive plan without any options or alternatives; ask the user questions if needed

5. Format the refined issue with:
   - Original issue description preserved at the top
   - A "## Implementation Plan" section with the approach
   - A "## Checklist" section with actionable task items using `- [ ]` format

6. Update the issue on GitHub:
   `gh issue edit $1 --repo [GITHUG_USER]/[GITHUB_REPO] --body "REFINED_BODY"`

7. Report success and show a summary of the plan added to the issue.

**Important:**
- Preserve the original issue content; append the plan below it
- Keep checklist items specific and actionable
- Reference specific files and line numbers where helpful
- Always follow the project conventions
