# PR Description

Generate a clear, structured pull request description based on the current branch's changes.

## Steps

1. Run `git diff main...HEAD` to get all changes since branching from main.
2. Run `git log main...HEAD --oneline` to see the commit history.
3. Analyze the changes and write a PR description with:
   - **Title**: concise (under 70 chars), imperative mood
   - **Summary**: 2–4 bullet points covering what changed and why
   - **Test plan**: checklist of how to verify the changes
4. Output the final description in a markdown code block, ready to paste into GitHub.
