# Why pull requests

Chapter 15 pushed commits straight to main. That works for a practice repository, where you are the only person working. On a team, pushing straight to main has two problems. Nobody else sees a change before it becomes the shared version, and a mistake is already in the history by the time anyone notices.

A pull request fixes both. You push a branch, and open a pull request asking for it to be merged into main. Other people can read every changed line, comment on it, and approve it. The merge happens only after the review. Until then, main stays as it was.

The rules for custom code at DataBank describe the same process. Code is reviewed before it is delivered, and the review has to confirm that the code works, is maintainable, and that the developer understands it. A pull request is where that review takes place, and its history records who checked what, and when.

A pull request also collects the automatic checks that run on the code, such as a build or a test run. Those checks appear on the pull request page, so a reviewer can see whether the code passed before reading it.

## Try it

Open the pull requests page of your practice repository on github.com. If there are none, the page says so. Read the tabs at the top: Code, Issues, and Pull requests. The next lesson creates one.
