#tool 
### Local Branches
For the purposes of this project, we are primarily using two branches: main and develop.

- Branch Strategy:
    - `main` - "trunk" where release-ready code is located. We will branch off of this trunk in order to create demos.
    - `develop` - main development branch. You will create remote branches off of this branch for your development and merge them back into this branch. Use your best judgment and only work on 
### Remote Branches
In the initial setup, you ran the following commands to clone our local repositories into your remote branch:

`git clone git@github.com:captain-fruit-punch/false-signal.git` 
`git clone git@github.com:captain-fruit-punch/false-signal-docs.git`

You will be doing development using the `develop` branch. Check out this branch using the following  command within the corresponding worktree:

`git checkout -B develop origin/develop`