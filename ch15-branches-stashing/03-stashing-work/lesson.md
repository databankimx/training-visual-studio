# Stashing unfinished work

Sometimes you are halfway through a change when something urgent comes up. You need to switch branches, but your edits are not ready to commit. A stash solves this. It takes your uncommitted changes off the files, saves them in a list, and leaves the files matching the last commit. You can switch branches, do the other work, and bring the stash back later.

Figure 15.2 shows the stash entry on the Git menu.

![Figure 15.2 - The stash entry on the Git menu](images/ch15-git-menu-stash.png "width=50%")

*Figure 15.2 - The stash entry on the Git menu*

Choose Git, then Stash, then the option to stash your changes. Give the stash a short description if Visual Studio asks for one, so you can tell it apart from others. The Changes list is empty afterward.

To bring the changes back, open the stash list from the same menu, and apply the stash you want. Applying a stash puts the changes back on the files. Once you are sure they are back, you can drop the stash from the list.

A stash is a safety net, not a place to keep work for weeks. A stash that you cannot describe is easy to forget, so commit the work when it is ready.

## Try it

1. Make a change to a file on the feature branch, but do not commit it.
2. Stash the change from the Git menu.
3. Check that the Changes list is empty, and that the file matches the last commit.
4. Open the stash list, and apply the stash to bring the change back.
