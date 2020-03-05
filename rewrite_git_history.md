# Rewriting origin history with upstream history

*These are instructions written by an amateur. They have worked for my use, but there is a high risk if you follow these instructions and they are not what you needed. Use at your own risk.*

1. Make sure you are in the branch that you want to update:

`git checkout <branch-name>`

2. Reset your local git to a commit-hash where origin and upstream have an identical commit history:

`git reset <commit-hash>`

3. Pull the upstream changes since that commit:

`git pull upstream <branch-name>`

4. Force push your local git repo to origin (**BE SURE YOU WANT TO DO THIS AS ALL OVERWRITTEN HISTORY WILL BE LOST**):

`git push --force origin <branch-name>`
