# Reviewing and checks

A review is the reading of the changes, and the reviewer's response to them. On the pull request page, the Files changed tab shows every changed line, with removed lines in red and added lines in green. Hover over a line to see a plus sign in the gutter. Click it to start a comment on that line, and the comment appears in the thread, where the author can answer it.

When you have read the changes, choose Review changes. You can leave a comment, approve the changes, or request changes. Approving says the change is ready to merge. Requesting changes says the author must address something first. The review then appears in the pull request's history.

The Checks area shows the automatic checks for the latest commit. Each one shows a green check mark when it passed, a red X when it failed, and a yellow dot while it is still running. Open a failed check to read its log. A check that failed is a reason to read the code more carefully, even if the diff looks correct.

If your repository has no checks set up, the Checks area is empty. That is expected for the practice repository, and the review still works without them.

## Try it

1. Open the pull request, and choose Files changed.
2. Find your comment line in PriceCalculator.cs, and hover over the line to see the plus sign.
3. Read the Checks area, and note whether it lists any checks.
