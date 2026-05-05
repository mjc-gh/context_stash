---
name: code-coverage
description: Achieve 100% test code coverage for CI
license: MIT
---

## What I do
- Identify files with inadequate test code coverage
- Guide you through adding tests to reach 100% coverage
- Help with coverage pragmas for impractical code paths

## When to use me
Use this skill when you need to reach 100% code coverage for your project's CI pipeline.

## Instructions

1. Run `COVERAGE=1 be rails t` to generate a table of files with under 100% code coverage. The `missing` column shows app code line numbers and ranges with inadequate coverage
2. For each file with inadequate coverage, analyze the application code and its existing test code
3. Identify and implement additional code coverage in order to achieve 100% coverage
  - Never modify application code, only test code
  - Prioritize adding to existing test cases to increase coverage
  - Add new test cases to increase coverage
  - When coverage is impractical, code requirements can be skipped using `# :nocov:` code comments

**Example COVERAGE Output**

Given an example COVERAGE result table:

+----------+-------------------------------------+-------+--------+---------+
| coverage | file                                | lines | missed | missing |
+----------+-------------------------------------+-------+--------+---------+
|  93.75%  | app/services/referrer_parser.rb     | 16    | 1      | 28      |
|  94.12%  | app/controllers/sites_controller.rb | 17    | 4      | 8,10-12 |
+----------+-------------------------------------+-------+--------+---------+

- `app/services/referrer_parser.rb` is missing 1 line of coverage on line 28
- `app/controllers/sites_controller.rb` is missing 4 lines of coverage on line 8 and lines 10 through 12
