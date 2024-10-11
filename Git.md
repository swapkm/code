# 1. Create a New Feature Branch
Before starting work on the new feature, create a separate branch to isolate your work from the main codebase. This will allow you to test, make mistakes, and iterate on the feature without worrying about breaking the live/stable version.

## Create a feature branch:

`git checkout -b feature/new-feature-name`

In this case, replace new-feature-name with something descriptive, like user-auth or stock-updates, to reflect what you’re working on.

This command creates a new branch based on the current state of main and switches to it. All changes will now be applied to this new branch instead of the main branch.

# 2. Work on Your Feature
Now, work on your Next.js feature as usual. You can make changes, add files, and test everything locally. Git will track all of your changes in this new branch.

# 3. Stage and Commit Changes
Once you’ve made some progress and want to save your work:

## Stage your changes:

`git add .`

## Commit your changes:

`git commit -m "Added initial implementation of new feature"`

You can commit frequently to track different stages of development.

# 4. Test Your Feature
Before merging it into main, ensure the feature works as expected. Since you’re working in an isolated branch, you’re free to experiment, rollback, or make adjustments without affecting your live code.

# 5. Merge to main When Feature Is Ready
If everything works and you’re satisfied with the feature, you can merge it back into main. First, switch to the main branch:

## Switch to the main branch:

`git checkout main`

Then, merge the feature branch into main:

## Merge the feature branch:

`git merge feature/new-feature-name`

# 6. Handle Conflicts (if any)
If there are any conflicts between the main branch and your feature branch, Git will notify you. You will need to manually resolve the conflicts in the affected files. After resolving the conflicts:

## Stage the resolved files:

`git add <file>`

## Commit the merge:

`git commit -m "Resolved conflicts and merged feature branch"`

# 7. Push Changes to Remote Repository
Once the merge is done and your feature is successfully integrated into main, push the changes to the remote repository (e.g., GitHub):

`git push origin main`

`git push -u origin main`

You should also push your feature branch (optional):

`git push origin feature/new-feature-name`

# 8. Delete the Feature Branch (Optional)
After the feature is merged into main and pushed, you can delete the local and remote branches to keep your project clean.

## Delete the local branch:

`git branch -d feature/new-feature-name`

## Delete the remote branch:

`git push origin --delete feature/new-feature-name`

# 9. Use Pull Requests for Team Collaboration
If you’re working in a team or want to review your changes before merging, use a pull request. This allows you or your team to review the code before merging it into main.

## Push the feature branch to the remote repository:

`git push origin feature/new-feature-name`

Open a pull request in GitHub from the feature/new-feature-name branch to main. The pull request can be reviewed, discussed, and tested before merging.



`git status`

`git pull`

`git push`

`git tag v1.0.0`

`git push --tags`