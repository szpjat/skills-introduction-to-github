<!--
  <<< Author notes: Step 5 >>>
  Instructions for creating and initializing a new repository.
-->

## Step 5: Initialize a New Repository

_Great work on completing the GitHub basics! :rocket:_

Now that you understand branches, commits, and pull requests, let's learn how to initialize a completely new repository and push your local work to GitHub.

**What is a remote?**: A _[remote](https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories)_ is a repository stored on another computer, in this case on GitHub's servers. Adding a remote allows you to push your local work to GitHub and collaborate with others.

**What is initializing a repository?**: Initializing means setting up a new Git repository either on GitHub or on your local machine, and then connecting them so you can push your code.

### :keyboard: Activity: Create and initialize a new repository

Follow these steps to create a new repository and push your code to GitHub:

#### Step 1: Create a new repository on GitHub

1. Go to [GitHub.com](https://github.com) and click the **+** icon in the top right corner
2. Select **New repository**
3. Enter a repository name (for example: `ProjektFinal`)
4. Choose whether to make it public or private
5. **Do not** initialize with a README, .gitignore, or license (since you'll push existing code)
6. Click **Create repository**

GitHub will show you the commands needed to push an existing repository.

#### Step 2: Connect your local repository to GitHub

In your terminal, navigate to your project directory and run these commands:

```bash
# Add the remote repository URL
git remote add origin https://github.com/YOUR-USERNAME/ProjektFinal.git

# Rename your branch to main (if it's not already)
git branch -M main

# Push your code to GitHub
git push -u origin main
```

> [!IMPORTANT]
> Replace `YOUR-USERNAME` with your actual GitHub username in the commands above.

#### What do these commands do?

- **`git remote add origin [URL]`**: Connects your local repository to the remote repository on GitHub. The name "origin" is the default name for the primary remote repository.
  
- **`git branch -M main`**: Renames your current branch to `main`. The `-M` flag forces the rename even if a branch named `main` already exists.

- **`git push -u origin main`**: Pushes your code to the remote repository. The `-u` flag sets up tracking, so future pushes and pulls are easier (you can just use `git push` or `git pull`).

### Additional useful commands

Once you've set up your remote repository, here are some commands you'll use frequently:

```bash
# View all configured remotes
git remote -v

# Push changes to the remote repository
git push

# Pull the latest changes from the remote repository
git pull

# Check the status of your repository
git status
```

### :tada: Congratulations!

You now know how to:
- Create a new repository on GitHub
- Connect a local repository to GitHub
- Push your code to a remote repository
- Use basic Git commands to manage your remote repository

For more information, see "[About remote repositories](https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories)" in GitHub Docs.
