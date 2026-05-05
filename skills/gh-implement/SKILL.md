---
name: gh-implement
description: Fetch a GitHub issue and implement the required changes
license: MIT
---

## What I do
- Fetch GitHub issue details
- Analyze requirements and acceptance criteria
- Implement code changes to address the issue

## When to use me
Use this skill when you need to implement a specific GitHub issue. You should have the issue number available.

## Instructions

Fetch the issue to content using:

`gh api repos/[GITHUB_USER]/[GITHUB_REPO]/issues/$1 | jq -r '"### \(.title)\n\(.body)"'`

**Instructions:**

1. Analyze what needs to be implemented or fixed fetched issue
2. Follow the exact plan described in the issue
3. Implement the required changes following the project's coding
conventions
4. Follow the checklist in the issue and complete all tasks

**IMPORTANT**: Do NOT commit changes or call git. Only implement the code changes requested in the issue. The user will handle commits themselves.
