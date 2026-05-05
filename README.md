# Context Stash

This repo contains various markdown files for use with Agentic
Development and with LLMs.

## Resources

To see how my `gh-plan`, `gh-implement`, and `reflect` commands are used
in practice, refer to my blog post on my ["Plan, Implement, Reflect
Workflow"](https://michaeljcoyne.me/posts/2026-05-04-plan-implement-reflect-workflow.html?utm_source=github&utm_medium=context_stash&utm_campaign=readme#content)
for agentic software development.

- `commands/`: Various slash commands that are primarily used with
  OpenCode. It's pretty straightforward on how to repurpose these
  commands for agentic tooling.
  - `code-coverage.md`: Achieve 100% test code coverage by analyzing
    missing coverage and adding test cases
  - `commit.md`: Stage changes, write a semantic commit message, and
    push to main
  - `gh-implement.md`: Fetch a GitHub issue and implement the requested
    changes
  - `gh-plan.md`: Refine a GitHub issue with a detailed implementation
    plan and checklist
  - `reflect.md`: Reflect on the session and update documentation with
    new context
  - Both the `gh-plan` and `gh-implement` commands will require
    customizations, and you will need to update the `[GITHUB_USER]` and
    `[GITHUB_REPO]` placeholders. These commands can also be reworked
    for other issue trackers, like Shortcut.
- `skills/`: "Skill" versions of the various slash commands.
- `RAILS.md`: Template text for a `AGENTS.md` file for Rails
  development.
- `RAILS-TURBO.md`: Reference notes for using Turbo with Rails
  controllers and views
- `RUBY-MINITEST.md`: Reference notes for testing with Minitest
