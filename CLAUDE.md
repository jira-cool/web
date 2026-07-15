# Project workflow instructions

## Always push and merge after a code fix

After any code change is implemented and verified (whether done directly or via a
delegated agent like JJ, html-ui-builder, js-developer, python-developer, data-handler,
etc.), always finish the workflow by:

1. Committing the change with a clear message
2. Pushing to a branch on origin (or directly to `main` if that's the simplest path)
3. Merging it into `main` and pushing `main`

Do this every time a fix is confirmed working — don't leave finished work sitting only
in the local working tree, and don't wait for the user to separately ask for push/merge
each time. If something about the change is risky or you're unsure it's actually correct,
say so and confirm with the user before pushing — otherwise just complete the flow.
