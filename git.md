#############################################
# 🔧 Git Configuration
#############################################

# Set user name and email
git config --global user.name "Your Name"
git config --global user.email "you@example.com"

# Set default text editor
git config --global core.editor "code --wait"

# View all configurations
git config --list

# Set up aliases
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci commit
git config --global alias.st status

#############################################
# 📁 Repository Initialization & Cloning
#############################################

# Initialize a new Git repository
git init

# Clone an existing repository
git clone <repository_url>

# Clone a specific branch
git clone -b <branch_name> <repository_url>

#############################################
# 📄 Staging & Committing Changes
#############################################

# Check the status of your files in the working directory
git status

# Add a specific file to the staging area
git add <file_name>

# Add all files to the staging area
git add .

# Commit staged changes with a message
git commit -m "Your commit message"

# Add and commit in one step
git commit -am "Your commit message"

# Amend the previous commit
git commit --amend

#############################################
# 🔍 Viewing Changes
#############################################

# View unstaged changes
git diff

# View staged changes
git diff --staged

# View commit history
git log

# View commit history in one line per commit
git log --oneline

# View commit history with a graph
git log --graph --oneline --all

#############################################
# 🌿 Branching & Merging
#############################################

# List all branches
git branch

# Create a new branch
git branch <branch_name>

# Switch to a branch
git checkout <branch_name>

# Create and switch to a new branch
git checkout -b <branch_name>

# Rename the current branch
git branch -m <new_branch_name>

# Delete a branch
git branch -d <branch_name>

# Merge a branch into the current branch
git merge <branch_name>

# Abort a merge
git merge --abort

#############################################
# 🔄 Rebasing
#############################################

# Rebase the current branch onto another branch
git rebase <branch_name>

# Abort a rebase
git rebase --abort

# Continue a rebase after resolving conflicts
git rebase --continue

# Skip the current patch during a rebase
git rebase --skip

# Interactive rebase of the last n commits
git rebase -i HEAD~<n>

#############################################
# 📌 Tagging
#############################################

# List all tags
git tag

# Create a lightweight tag
git tag <tag_name>

# Create an annotated tag
git tag -a <tag_name> -m "Tag message"

# Delete a local tag
git tag -d <tag_name>

# Push a tag to the remote repository
git push origin <tag_name>

# Delete a remote tag
git push origin --delete <tag_name>

#############################################
# 📦 Stashing Changes
#############################################

# Stash current changes
git stash

# List all stashes
git stash list

# Apply the most recent stash
git stash apply

# Apply and drop the most recent stash
git stash pop

# Drop a specific stash
git stash drop stash@{n}

# Clear all stashes
git stash clear

#############################################
# 🚀 Remote Repositories
#############################################

# Add a remote repository
git remote add origin <repository_url>

# View remote repositories
git remote -v

# Remove a remote repository
git remote remove origin

# Rename a remote repository
git remote rename origin upstream

#############################################
# 📥 Fetching & Pulling
#############################################

# Fetch changes from the remote repository
git fetch

# Pull changes from the remote repository
git pull

# Pull with rebase
git pull --rebase

#############################################
# 📤 Pushing Changes
#############################################

# Push changes to the remote repository
git push

# Push a specific branch
git push origin <branch_name>

# Push all branches
git push --all

# Push tags
git push --tags

# Force push
git push --force

#############################################
# 🧹 Undoing Changes
#############################################

# Unstage a file
git reset <file_name>

# Unstage all files
git reset

# Revert a commit by creating a new commit
git revert <commit_hash>

# Reset to a specific commit (soft)
git reset --soft <commit_hash>

# Reset to a specific commit (mixed)
git reset --mixed <commit_hash>

# Reset to a specific commit (hard)
git reset --hard <commit_hash>

#############################################
# 🔍 Inspecting Repository
#############################################

# Show information about a commit
git show <commit_hash>

# Show changes between commits
git diff <commit1> <commit2>

# Show who changed what in a file
git blame <file_name>

# Search for a pattern in the repository
git grep "search_term"

#############################################
# 🛠️ GitHub CLI (gh) Commands
#############################################

# Authenticate with GitHub
gh auth login

# Create a new repository
gh repo create

# Clone a repository
gh repo clone <repository>

# View repository information
gh repo view

# Create a pull request
gh pr create

# View pull requests
gh pr list

# Merge a pull request
gh pr merge

# View issues
gh issue list

# Create a new issue
gh issue create

# View notifications
gh notifications

# View the current user's profile
gh user view

# View help for a command
gh help <command>