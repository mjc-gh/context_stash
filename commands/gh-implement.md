---
description: Fetch a GitHub issue and implement it
model: openrouter/anthropic/claude-haiku-4.5
---

Fetch the issue to content using:

`gh api repos/[GITHUB_USER]/[GITHUB_REPO]/issues/$1 | jq -r '"### \(.title)\n\(.body)"'`

**Instructions:**

1. Analyze what needs to be implemented or fixed fetched issue
2. Follow the exact plan described in the issue
3. Implement the required changes following the project's coding
conventions
4. Follow the checklist in the issue and complete all tasks

**IMPORTANT**: Do NOT commit changes or call git. Only implement the code changes requested in the issue. The user will handle commits themselves.
