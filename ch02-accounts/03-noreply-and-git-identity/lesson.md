# Your commit address and Git name

Every commit you make records a name and an email address. Git stores them in the commit itself, and they are published with it when you push. You do not want your real email address there, so GitHub gives you a private address to use instead. Visual Studio's Git Changes window uses the same name and address when you commit, so set them here, before Chapter 13.

## Use GitHub's noreply address

In your GitHub settings, open Emails. Turn on the option to keep your email address private, and note the noreply address it shows. It looks like this:

`12345678+yourname@users.noreply.github.com`

The number and name are yours, and the address works for commits without showing your real address.

Figure 2.5 shows the setting.

![Figure 2.5 - Noreply email setting](images/ch02-noreply-email-setting.png "width=75%")

*Figure 2.5 - Noreply email setting*

## Set your name and email in Git

Git needs to know who you are. You set it once for your computer, and every repository you make on it uses the same details. Open PowerShell from the Start menu and type the commands below, using your own name and the noreply address from the last step.

```
git config --global user.name "Your Name"
git config --global user.email "12345678+yourname@users.noreply.github.com"
```

Git has to be installed before this step. The setup script installs it. If you installed Visual Studio by hand, check now with this command:

```
git --version
```

If PowerShell says that git is not recognized, install it with this command, then open a new PowerShell window and try again:

```
winget install Git.Git
```

If winget is not available, download Git for Windows from git-scm.com and use the default options.

Once the Git identity is set, check the result with this command:

```
git config --global --list
```

The output should include the two lines you just set, with your name and the noreply address. Tick the step in the checklist once they match.

> **Why the name matters:** the name is what other people see on your commits. Use the name you want on your work, and keep it the same across the commits you make in this course.
