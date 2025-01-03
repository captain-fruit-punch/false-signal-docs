#tool
We're using git for control over this notes document and and the Unity development environment.

Here's a guide of basic use of git:
https://rogerdudler.github.io/git-guide/
https://medium.com/@ramadan123sayed/a-comprehensive-guide-to-git-and-github-from-beginner-to-advanced-with-practical-use-cases-8e1ad98b48db

Internal usage guide:
- Git basics (foundyoufaker will add to this as he sees fit):
    - [[Local and Remote]]
    - [[Commit and Push]]
    - [[Merge]]
- Unity-specific tips:
	- **Merging scenes and prefabs is not advised.** Only **one** person should be working on and pushing changes to a scene or a prefab at a time. You need to revert your changes if you are making commits to the same scene/prefab at the same time as someone else.
    - Always test scene changes before committing.
    - Use prefabs whenever possible.
    - Keep meta files with their assets.
    - Don't force-push to `main` branch.