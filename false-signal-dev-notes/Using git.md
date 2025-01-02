We're using git for control over this notes document and and the Unity development environment.
Here's a guide of basic use of git:
https://rogerdudler.github.io/git-guide/
https://medium.com/@ramadan123sayed/a-comprehensive-guide-to-git-and-github-from-beginner-to-advanced-with-practical-use-cases-8e1ad98b48db
Internal usage guide:
- Commit Guidelines:
    - Commit frequently with clear messages
    - Use prefixes like:
        - `feat:` for new features
        - `fix:` for bug fixes
        - `docs:` for documentation
        - `refactor:` for code refactoring
- Branch Strategy:
    - `main` - production-ready code
    - `develop` - main development branch
    - `feature/*` - new features
    - `bugfix/*` - bug fixes
    - `release/*` - release preparation
- Unity-specific tips:
    - Always test scene changes before committing
    - Use prefabs whenever possible
    - Keep meta files with their assets
    - Don't force-push to main branches