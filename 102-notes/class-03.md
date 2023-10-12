## Class 03 Notes

### What is Version control?

- Allows you to see many different iterations of files during the change process.  This makes it so you are able to revert back to an older save, track modifications over time and compare changes.  Mistakes that could happen can be reverted back to an older more stable file.

### Cloning in Git

- Cloning is the act of taking a repo from GitHub and saving it to your local directory, essentially cloning your online repo for offline use.  Typically don't have to clone multiple times, one time is good as after that you're allowed to push or pull any changes you made both on Github or locally.

### Common Git Commands

1. **git add** is the command to track and stage files, this allows you to specify what files you wish to stage for the next commit process.

2. **git commit** is the command that takes a snapshot of your staged changes with your message of choice to give more details as to why you're doing the changes.

3. **git push origin main** is the command to push all the changes you made.  Origin is the remote repository and main is the branch that you're pushing to.  This finallizes all changes and updates the repo on GitHub with your changes.