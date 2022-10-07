# Git Commands

## Creating Repos

- **Creating a GitHub repo from CLI ([Doc](https://cli.github.com/manual/gh_repo_create))**
    
    `gh repo create`
    
- **Link to a new remote** (instruction from GitHub)
    
    `git init`
    
    `git add README.md` (optional)
    
    `git add .`
    
    `git commit -m "first commit"`
    
    `git branch -M main`
    
    `git remote add <remote_name> <ssh_or_http_url>` Use `origin` as <remote_name> for a new repo. Copy the remote’s URL from GitHub for <ssh_or_http_url>
    
    `git push -u origin main` After the initial push, we can push with just `git push`
    
- **Clone a remote repo**
    
    `git clone <ssh_or_http_url>` 
    
- ** Clone a single branch
`git clone --single-branch <repo_url>`  Clones just the main branch
`git clone -b <branch_name> --single-branch <repo_url>` Clones the specified branch
    
    

## Working on Repos

- ****Branching and Merging `branch`, `checkout`, `merge`**
    
    **Make a branch**
    
    - `git branch <branch_name>` Creates a new branch
    - `git checkout -b <branch_name>` Creates and switches to the new branch
    
    **Switch between branches**
    
    - `git checkout <branch_name>`
    
    **Merge branches**
    
    - `git merge <branch_name>` (bring contents from <branch_name> to the current branch you are on)
    
    **Delete a branch**
    
    - `git branch -d <branch_name>`
    - `git branch -D` Force delete, same as `--delete --force`
    
    **Show branches**
    
    - `git branch -v`


- **Fetch and Pull `fetch`, `pull` ([Doc](https://github.com/git-guides/git-pull))**
    
    **Fetching changes from a remote** 
    
    - `git fetch --all`
    - `git reset --hard origin/main` ([More on git reset](https://github.com/git-guides/git-pull#undo-a-git-pull))
    
    General fetching, pulling
    
    - `git fetch <remote_name> <branch_name>` Fetch, or receive, commits from a given remote at the given branch. Stores these commits in either the named commit, or in a special, new branch.
    - `git pull <remote_name> <branch_name>` Performs a `git fetch` into a new branch, then merges it into the current branch and removes the fetched branch.


- **Push `push` ([Doc](https://github.com/git-guides/git-push))**
    - `git push (-u) (<remote_name> <branch_name>)` Push, or send, commits to remote at the given branch. `-u` saves the remote and branch names as default for future use.
    - `git push -f` or `--force` will force push local branch to remote ([Doc](https://www.freecodecamp.org/news/git-push-to-remote-branch-how-to-push-a-local-branch-to-origin/))
- **Stage Changes `add`([Doc](https://github.com/git-guides/git-add))**
    - `git add <file_name>` Adds changes made to the given file to the staging area.
    - `git add .` Adds all changes (creating, updating and removing files), to files in this directory and sub-directories, to the staging area.
    - `git add -A` Adds all changes (creating, updating and removing files), in all files, to the staging area.
    - `git add -p` Adds updates in all staged files to the staging area, but runs you through all the changes step by step.
- **Committing Snapshots `commit` ([Doc](https://www.notion.so/Git-Commands-29ecead64aee4a3da088c9e6b3168354))**
    - `git commit -m "awesome commit message"` Saves a snapshot of the filesystem including any changes that have been added/staged as a commit. It saves the commit with a simple description, or *message*, given after `m`.
    - `git commit` Commits as above, but takes you to a text editor (`nano`) to edit the commit's *message*.
- **Go back to the previous commit**
    - `git reset --hard <commit-hash>`

## Reading Repos

- `git remote show origin` Show repo’s remote URL
- `git remote -v` Show all repo URL
- `$ git status` Prints out the current "tracking state" of the repo. The state includes information about changes, additions and deletions of files, whether or not these changes have been added/stages, and sometimes even any merge conflicts.
- `git log` Prints out the commit history of the current branch of the current repo.
- `git branch` & `$ git branch -v` Prints out a list of all available branches in the repo.
- `git diff <branch_or_commit_name>` Prints out information about *differences*, as insertions (in green) and deletions (in red), between the current commit and the given commit (or the most current commit in the given branch).
- `git diff` shows difference between files
