# DevOps Class Activity

## Practical Version Control Workflow Verification Challenge

### Student Details
- Name: Ubaidullah Zubair
- SAP ID: 51650
- GitHub Username: Ubaid-555
- Repository: https://github.com/Ubaid-555/devops-git-challenge

## Commit History

The following history was captured on main after merging the pull
request and pulling the merged changes locally, before committing
this proof file.

```text
6eb3c4a Merge pull request #1 from Ubaid-555/development
c1c0922 Merge staging into development and resolve environment conflict
2e9e5bd Configure staging deployment
a77dc4d Configure development deployment
49c9b59 Add initial deployment script and README

```

## Q1: Difference between Git and GitHub

Git is a distributed version control system that tracks changes in a local repository.
It allows developers to create commits, manage branches, and merge changes without an internet connection.
GitHub is an online platform that hosts Git repositories and provides collaboration features such as pull requests, issues, and reviews.
In this activity, I used Git for local version control and GitHub to host the repository and merge a pull request.

## Q2: Working Directory, Staging Area, and Local Repository

The working directory contains the project files that I can edit directly.
The staging area holds the specific changes selected for the next commit using git add.
The local repository stores committed snapshots and their history inside the .git directory.
Editing deploy.sh changed the working directory, git add staged the change, and git commit recorded it in the local repository.

## Q3: Difference between git stash pop and git stash apply

Both git stash pop and git stash apply restore changes previously saved in a stash.
The apply command keeps the stash entry after restoring its changes, allowing it to be reused.
The pop command removes the stash entry after applying it successfully.
If pop produces conflicts, the stash entry is retained and can be explicitly removed after resolving the conflicts and confirming that it is no longer needed.

## Q4: Difference between git fetch and git pull

The git fetch command downloads remote objects and updates remote-tracking references without integrating them into the current branch.
This allows developers to inspect remote changes before deciding how to incorporate them.
The git pull command fetches changes and then integrates them into the current branch according to its options and configuration.
In this activity, git pull --ff-only origin main updated my local main after the GitHub merge and would refuse an update requiring reconciliation of divergent history.

## Merged Pull Request: https://github.com/Ubaid-555/devops-git-challenge/pull/1