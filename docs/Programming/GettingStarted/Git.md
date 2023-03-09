# Git
## Why use Git?
- Git is a version control system that allows us to track changes to our code. It also allows us to collaborate with other people on the same codebase. Git is a very powerful tool that is used by many companies and open source projects. It is also a very important skill to have as a software developer.

- We have a Github organization that we use to host our code. Github is a website that allows us to host our code and collaborate with others. It also allows us to keep track of our code and see what changes have been made.

- If you are not familiar with Git, you can read the [Git book](https://git-scm.com/book/en/v2) to learn more about it. It is a very good resource and will teach you everything you need to know about Git.

- And if you haven't already, ask Jasper, Jacob, Cameron R, or Cam Wolf to add you to the Github organization.

-----------------------------------------

## Important Git commands
- `git clone <repo>`: Clones a repository to your local machine.
- `git status`: Shows the status of your local repository.
- `git add <file>`: Adds a file to the staging area.
- `git commit -m "<message>"`: Commits the changes in the staging area to your local repository.
- `git push`: Pushes your local commits to the remote repository.
- `git pull`: Pulls the latest changes from the remote repository to your local repository.
- `git checkout <branch>`: Switches to a different branch.
- `git branch <branch>`: Creates a new branch.
- `git merge <branch>`: Merges the changes from the specified branch into the current branch.
- `git stash`: Stashes the changes in your working directory.
- `git stash pop`: Pops the changes from the stash and applies them to your working directory.
- `git log`: Shows the commit history of the current branch.
- `git reset --hard <commit>`: Resets the current branch to the specified commit.
- `git reset --hard origin/<branch>`: Resets the current branch to the specified remote branch.


#### Side note / Alternative to Git commands
- If you are not comfortable using the command line, you can use a GUI for Git. There are many GUIs for Git, but the one we recommend is [GitHub Desktop](https://desktop.github.com/). It is a very simple and easy to use GUI for Git. It is also very similar to the command line, so you can easily switch between the two if you want to.

- Another alternative is [GitKraken](https://www.gitkraken.com/). It is a very powerful GUI for Git, but it is a bit more complicated to use. It is also a paid software, but you can use it for free if you don't mind the watermark.

- Lastly, the team's favorite is through [VSCode](https://code.visualstudio.com/). It has a built in Git GUI that is very powerful and easy to use. It is also free and open source. We recommend using this if you are already using VSCode. It has both a built in terminal and a built in Git GUI, so you can use it for both Git and the command line.

-----------------------------------------

## Git workflow
- Workflow varies from team to team, so we won't be covering it too indepth. What ever works for you is fine. However, we do have a few recommendations.
    + **We recommend using a feature branch workflow.** This means that you should create a new branch for each feature you are working on. This allows you to work on multiple features at the same time without having to worry about merge conflicts. It also allows you to easily revert changes if you need to.
    + **We also recommend using a pull request workflow.** This means that you should create a pull request for each feature you are working on. This allows you to easily review the changes you are making and make sure that they are correct. It also allows you to easily revert changes if you need to.
    + **We also recommend using a squash and merge workflow.** This means that you should squash and merge your pull requests. This allows you to keep your commit history clean and easy to read. It also allows you to easily revert changes if you need to.
    + `Key points:`
        * Create a new branch for each feature you are working on.
        * Create a pull request for each feature you are working on.
        * Squash and merge your pull requests.
        * Keep your commit history clean and easy to read.
        * Revert changes if you need to.

-----------------------------------------

## Git best practices
- **Commit often.** This allows you to easily revert changes if you need to. But not too often. You don't want to commit every time you make a small change. You should commit when you have made a significant change to your code.
- **Write good commit messages.** This allows you to easily see what changes you have made. It also allows you to easily revert changes if you need to. *(Basically don't be like Jasper, his commit message has emojis for some reason :'D)*
- **Always pull:**
    + before you push. This allows you to easily resolve merge conflicts if you need to. It also allows you to easily revert changes if you need to.
    + before you start working on a new feature. This allows you to easily resolve merge conflicts if you need to. It also allows you to easily revert changes if you need to.
- **Always push:**
    + after you have committed your changes. This allows you to easily revert changes if you need to.
    + after you have merged your pull request. This allows you to easily revert changes if you need to.
- **Always merge:**
    + after you have pushed your changes. This allows you to easily revert changes if you need to.
    + after all your teammates have reviewed your pull request. To make sure that everyone is on the same page.
    + after you have reviewed your pull request. This allows you to easily revert changes if you need to.
- **Avoid making changes directly to the `master`/`main` branch.** This branch should only be used for production code. If you need to make changes to the `master`/`main` branch, you should create a new branch and then merge it into the `master`/`main` branch.
- **Branch name should be descriptive.** This allows the team to easily see what the branch is for. For example, if you are working on a feature that adds a new button to the home page, you should name your branch something like `feature/add-home-button`. For when you're working on a bug, you should name your branch something like `bug/fix-home-button`. More on this:
- **Branch names should follow the following format:**
    + `feature/<feature-name>`: For when you are working on a new feature.
    + `bug/<bug-name>`: For when you are working on a bug.
    + `refactor/<refactor-name>`: For when you are refactoring code.
    + `test/<test-name>`: For when you are writing tests.
    + `docs/<docs-name>`: For when you are writing documentation.
    + `misc/<misc-name>`: For when you are working on something that doesn't fit into any of the other categories.
- Ofcourse, you can name your branch whatever you want, but we recommend following this format. It makes it easier for the team to see what you are working on. But really it's up to you, and we don't care lol.

-----------------------------------------

## Git resources
- [Git book](https://git-scm.com/book/en/v2): A very good resource for learning Git.
- [Git cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf): A very good cheat sheet for Git.
- [GitKraken cheat sheet](https://www.gitkraken.com/learn/git/cheat-sheet): A very good cheat sheet for GitKraken.
- [VSCode Git cheat sheet](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf): A very good cheat sheet for VSCode's built in Git GUI.
- [GitHub cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf): A very good cheat sheet for GitHub.
- [GitHub Desktop cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf): A very good cheat sheet for GitHub Desktop.