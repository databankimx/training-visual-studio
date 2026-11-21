# Homework: review a pull request

This exercise has you open a pull request and review it as if someone else wrote it. You are the author and the reviewer, so you will read it with a fresh view.

## Work through these steps in order

1. **Open a pull request.** Create a branch from main called feature/review-practice, add a comment above the Average method in PriceCalculator.cs, commit it, and push. On github.com, open a pull request from the branch into main, with a title and a short description.
2. **Read the description.** Check that it says what the change does and why, without reading the code.
3. **Review the Files changed tab.** Read the one changed line, and check that the comment is accurate.
4. **Leave a comment.** Hover over the line, click the plus sign, and write a question about the wording, such as whether the comment should say what the method returns.
5. **Choose Review changes.** Select Comment, and submit the review.
6. **Close the pull request.** Choose Close pull request, without merging, so main stays as it was.

## Check your work

The pull request is closed, its history shows your comment and review, and main has no new commit.

~~~spoiler
A good description says what changed, why, and what to look at. Here, the change is a comment, so the description can be one sentence.

The comment you left should be a question or a suggestion about wording, not a complaint. Reviews work best when a comment names one line and one concern.

Closing the pull request without merging keeps main unchanged, and the pull request stays in the list of closed requests, with its comments.
~~~
