Before starting work on the new feature, create a separate branch to isolate your work from the main codebase. This will allow you to test, make mistakes, and iterate on the feature without worrying about breaking the live/stable version.

## Branch:

`git checkout -b feature/new-feature-name`

### Stage your changes:

`git add .`

### Commit your changes:

`git commit -m "Added initial implementation of new feature"`

### Switch to the main branch:

`git checkout main`

### Merge the feature branch:

`git merge feature/new-feature-name`

### Stage the resolved files:

`git add <file>`

### Commit the merge:

`git commit -m "Resolved conflicts and merged feature branch"`

### 7. Push Changes to Remote Repository

`git push origin main`

`git push -u origin main`

You should also push your feature branch (optional):

`git push origin feature/new-feature-name`

## 8. Delete the Feature Branch (Optional)
After the feature is merged into main and pushed, you can delete the local and remote branches to keep your project clean.

### Delete the local branch:

`git branch -d feature/new-feature-name`

### Delete the remote branch:

`git push origin --delete feature/new-feature-name`

## Others

`git commit --amend`

`git status`

`git pull`

`git push`

## Tags

### Lightweight Tag
`git tag v1.0.0`

### Annotated Tag
`git tag -a v1.0.0 -m "Release version 1.0.0"`

### Listing Tags
`git tag`

### Checkout a Tag

If you want to view the state of your project at the point in time when a tag was created, you can checkout the tag:

`git checkout <tag_name>`

### Push Tags to Remote
`git push origin <tag_name>`

or to push all tags

### Delete a Tag
`git tag -d <tag_name>`

To delete a remote tag: `git push origin --delete <tag_name>`