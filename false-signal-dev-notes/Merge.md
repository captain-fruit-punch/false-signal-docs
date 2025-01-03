#tool 
This is how we will reconcile the remote branch with the `develop` branch and the `develop` branch with the `main` branch.

The two following workflows should only be used when you are **not working with prefabs or scenes**.
##### Integrating `develop` with remote
Verify your remote branch is up to date with `origin\develop`:
	1. `git fetch origin develop`
	2. `git status`
	3. If it isn't up to date, use `git merge origin\develop`
	4. `git push origin develop`

##### Integrating `main` with `develop`
1. `git fetch origin main`
2. `git checkout main`
3. `git status`
4. If it isn't up to date, use `git merge origin\main`
5. `git merge develop`
6. `git push origin main` 

### Scenes and Prefabs
**Merging scenes and prefabs is not advised.** Only **one** person should be working on and pushing changes to a scene or a prefab at a time. You need to revert your changes if you are making commits to the same scene/prefab at the same time as someone else.

If you are working on a scene/prefab, use the following workflows instead to merge:

##### Integrating remote with `develop`
Verify your remote branch is up to date with `origin\develop`:
	1. `git fetch origin develop`
	2. `git status`
	3. If it isn't up to date, use `git merge --ff-only develop`
	4. If this fails, verify which files have changed between the two branches.
	   `git diff @{upstream} --name-only`
	5. If no scene or prefab files have been modified, you can proceed with the merge using
	   `git merge origin\develop`.
	6. `git push origin develop`

##### Integrating `develop` with `main`
1. `git fetch origin main`
2. `git checkout main`
3. `git status`
4. if it isn't up to date, use `git merge --ff-only origin\main`
5. If this fails, verify which files have changed between the two branches.
	`git diff @{upstream} --name-only`
1. If no scene or prefab files have been modified, you can proceed with the merge using
	 `git merge origin\main`.
6. `git merge develop`
7. `git push origin main`