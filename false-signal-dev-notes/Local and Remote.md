#tool 
### Local Branches
For the purposes of this project, we are primarily using two branches: main and develop.

- Branch Strategy:
    - `main` - production-ready code
    - `develop` - main development branch
    - `feature/*` - new features
    - `bugfix/*` - bug fixes
    - `release/*` - release preparation
### Remote Branches
In the initial setup, you ran the following commands to clone our local repositories into your remote branch:

`git clone git@github.com:captain-fruit-punch/false-signal.git` 
`git clone git@github.com:captain-fruit-punch/false-signal-docs.git`

You will be doing development using the `develop` branch. Check out this branch using the following  command within the corresponding worktree:

`git checkout -B develop origin/develop`