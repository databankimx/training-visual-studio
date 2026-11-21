# Creating a pull request on GitHub.com

First, push a branch to GitHub. Create a branch called feature/pricing-notes from main in Visual Studio, as in Chapter 15. Add a comment above the Total method in PriceCalculator.cs, commit it, and push the branch. Chapter 16 covers pushing. Publishing a new branch the first time is the same as pushing one.

Open your practice repository on github.com. After a push, GitHub usually shows a banner near the top of the page, offering to compare and create a pull request for the new branch. Figure 18.1 shows the banner with its button. Choose Compare & pull request.

![Figure 18.1 - The Compare and pull request banner on GitHub](images/ch18-compare-and-pull-request.png "width=75%")

*Figure 18.1 - The Compare and pull request banner on GitHub*

The form has a few parts. The base branch is main, the branch you want to merge into. The compare branch is feature/pricing-notes, the branch with your change. Give the pull request a title that says what it does, such as Add a note above Total. In the description, say what you changed and why, in a few sentences, so a reviewer knows where to look.

Choose Create pull request. The page now lists the commits, the changed files, and the checks, and it is open for review.

## Try it

1. Push feature/pricing-notes with the comment change, then open your repository on github.com.
2. Choose Compare & pull request, and check that the base is main and the compare branch is feature/pricing-notes.
3. Write a title and a short description, and choose Create pull request.
