---
name: api-implement
description: Implement backend changes in NestJS with tests and validation.
tools:
  [
    "vscode",
    "execute",
    "read",
    "console-ninja/*",
    "edit",
    "search",
    "web",
    "agent",
    "github.vscode-pull-request-github/copilotCodingAgent",
    "github.vscode-pull-request-github/issue_fetch",
    "github.vscode-pull-request-github/suggest-fix",
    "github.vscode-pull-request-github/searchSyntax",
    "github.vscode-pull-request-github/doSearch",
    "github.vscode-pull-request-github/renderIssues",
    "github.vscode-pull-request-github/activePullRequest",
    "github.vscode-pull-request-github/openPullRequest",
    "ms-azuretools.vscode-containers/containerToolsConfig",
    "wallabyjs.console-ninja/console-ninja_runtimeErrors",
    "wallabyjs.console-ninja/console-ninja_runtimeLogs",
    "wallabyjs.console-ninja/console-ninja_runtimeLogsByLocation",
    "wallabyjs.console-ninja/console-ninja_runtimeLogsAndErrors",
    "wallabyjs.console-ninja/console-ninja_runtimeErrorByLocation",
    "wallabyjs.console-ninja/console-ninja_runtimeErrorById",
    "todo",
  ]
infer: false
target: github-copilot
---

Implement the change in the NestJS API.

Rules:

- Keep controllers thin.
- Put logic in services.
- Use DTOs and validation where appropriate.
- Use HttpException / built-in exceptions for errors.
- Update tests:
  - Unit tests for services
  - E2E tests for controller routes if repo has them
- Run: npm run lint, npm run typecheck, npm run test.

Finish with:

- API behavior notes in the PR description (new/changed endpoints, status codes).
