#tool 
### Commit
When adding new files, creating new features, or making any code changes in general, you should keep a log of your work by committing it. Make sure your worktree is a branch of the `develop` branch.

The workflow goes as follows:

1. use `git status` to review what files you have created, deleted, or modified.
2. use `git revert` to remove changes you did not intend.
3. use `git add` to select files you want to add to your commit. `git add .` will add everything that was modified.
4. use `git commit -m "Commit Message Here"` to commit your changes.

- Commit Guidelines:
    - Commit frequently with clear messages
    - Use prefixes like:
        - `feat:` for new features
        - `fix:` for bug fixes
        - `docs:` for documentation
        - `refactor:` for code refactoring

### Commit History
You can look at your previous commits easily using `git reflog`.  This will show you which commit your branch head is currently on. You can revert your changes using the following workflows:

1. Hard reset
	1. `git reset --hard <commit ref>`
	2. This discards all changes after the specified commit.
2. Soft reset
	1. `git reset --soft <commit ref>`
	2. This maintains all changes after the specified commit, which stages them. You may revert and add these files to your liking.

### Push
`git push` will push all of your commits to the remote branch `develop` for all of the team to see.

If you want to undo a push:
1. **Let us know.** It's possible that we've made conflicting pushes to `develop` that need to be considered, or there may be a safer way to back your changes out.
2. `git reset --hard <commit ref prior to push>`
3. `git push -f`