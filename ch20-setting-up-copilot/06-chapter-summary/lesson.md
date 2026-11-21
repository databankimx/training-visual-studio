# Chapter summary

Remember these as you set up Copilot:

- Add your GitHub account from the account icon at the top right, with Add another account. The Copilot menu lists the Copilot options, and Copilot Usage shows your plan's limits.
- Copilot sends part of the code around your cursor to GitHub's service. Keep secrets and customer data out of your code and comments.
- The Copilot page under GitHub, in the Options dialog, controls suggestions. Changes take effect straight away.
- Follow the use rule at the start of this chapter, and treat every suggestion as untrusted until you have read, built, and tested it.

```quiz
Where do you add your GitHub account to Visual Studio?
○ The Solution Explorer
→ The Solution Explorer shows projects and files, not accounts.
○ The Output window
→ The Output window shows messages, not accounts.
◉ The account icon at the top right of the window
→ Yes. Choose Add another account, then GitHub.
```

```quiz
Which of these should stay out of code and comments you give to Copilot?
◉ Passwords and secrets
→ Yes. Copilot sends nearby code to GitHub's service, so secrets must not appear in it.
○ Method names
→ Method names are ordinary code, and they are not secrets.
○ Comments that describe a method
→ A plain comment about a method is fine, as long as it has no secrets or customer data.
```

```quiz
You turn off automatic suggestions. How do you get a suggestion now?
○ Restart Visual Studio
→ A restart does not change how suggestions are requested.
◉ Press Ctrl+Space to ask for one
→ Yes. With automatic suggestions off, you ask for one when you want it.
○ Remove the GitHub account
→ Removing the account stops Copilot from working. It does not request a suggestion.
```
