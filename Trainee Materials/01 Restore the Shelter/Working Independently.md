# Working independently

## Tools and files

You need your existing personal Survival-Nexus project, a plain-text editor with AI disabled, Git, and a current browser. Git/GitHub basics have already been completed. Do not put these handouts or private solutions into the application repository.

In Pack01, open `web/index.html` directly in the browser. Open browser developer tools with F12 or Ctrl+Shift+I; choose Console to see JavaScript output and errors. For a blank page, check the actual file and extension, save, reload, and inspect the first error.

Activity06 introduces Node.js24 LTS, npm, modules, tests, and a local web server. Install the24.x LTS runtime from the [official Node download](https://nodejs.org/en/download) before that activity; reopen PowerShell and check `node --version` and `npm.cmd --version`. Use npm.cmd if PowerShell blocks npm.ps1; do not weaken machine execution policies. If installation is blocked by device policy, record that environment blocker and continue only the tasks whose tools are available; do not claim an unexecuted check passed.

Keep browser-only DOM code in main.js and pure domain logic in domain.js once those files are introduced. Node tests import domain logic without a browser. Use the exact filename, import path, and capitalization shown in each mission.

## Solve a blocker without another person

1. State the expected result and actual result in one sentence each.
2. Read the first error and its file/line. Fix that issue before chasing later errors.
3. Confirm input values and types. Predict a tiny example by hand.
4. Use a breakpoint or a few targeted logs to find where the result first differs.
5. Read the linked official reference for that concept. Use ordinary search results; avoid AI-generated answers.
6. Reduce the problem to a small disposable example, then apply the understood correction to your project.
7. Rerun the failing check and the related checks. Record what changed and why.

Do not hide an error by deleting its assertion, hard-coding the sample result, silently replacing data, or reporting a check you did not run. If a requirement is unclear, reread its stated rules and examples; record any remaining ambiguity and conservative assumption rather than changing an explicit rule.

## Evidence in Markdown

For each activity, create `docs/activity-NN.md` with: goal, inputs/cases, expected outcome, actual outcome, correction, and official documentation consulted. Describe files and technical behavior only. No name, participant code, contact detail, account screenshot, full device path, or browser-history export is required.

When a mission requests an explanation, write it in these notes. When it requests a demonstration, reproduce the behavior yourself and record the results. No other person needs to observe or approve it.

## Git as the project workflow

Use the workflow you already learned. Before committing, inspect status and diffs, stage named intended files, inspect the staged changes, commit, and push to your personal repository. New files must be read directly before staging because ordinary git diff does not show untracked contents.

From Activity04 use a new feature branch from clean, updated main. Push it, open a PR into your own main, self-review source/tests/notes, then merge using a merge commit. Switch back to local main and run `git pull --ff-only origin main`. No outside reviewer or approval is required. Keep branches if unsure; do not force-push or delete unrelated work.

If a branch name is taken, choose a fresh task-only suffix. If an ordinary pull refuses because histories diverged, inspect status and the branch graph before making further changes; preserve your work and follow the [official branching reference](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging). Never use destructive commands as a shortcut to a clean status.

## Self-check and progression

Complete every required acceptance case, including empty/invalid cases. For function/API/database work, run the automated tests and inspect the results. Compare your own explanations with actual behavior. Correct failures before the next mission. Answer keys are not needed to perform the published checks; they remain private for later evaluation.

There is no instructor sign-off, live review, or feedback dependency. Later packs are released separately; if the next pack is not published, practise variations of completed missions rather than guessing unreleased tasks.
