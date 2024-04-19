# Presentation de Git 
https://docs.google.com/presentation/d/1vfsG__2-T7xJYGKFs9HfPKmaoMN1Je0V0h7gLyiY1AU/edit?usp=sharing 

# Pré Condition
These steps assume that you [have installed git locally](https://www.atlassian.com/fr/git/tutorials/install-git), that you [have created a GitHub account](https://github.com/join), and [have added your local ssh key](https://help.github.com/en/enterprise/2.15/user/articles/adding-a-new-ssh-key-to-your-github-account) to it.

# Utilisations 

### Fork a Repo
- Go on the repo you want to fork
- Use the fork button in the top right corner
- Now when you go on your repository, you will see the fork repo

### Clone your forked repo locally
- On a terminal : `git clone` ssh ou http path

### Link a project
- Add the original project as a distant repo. `git remote add upstream` original path'repo
- Add local project on github. `git remote add origin` git path'repo

### Branch 
- See all the branch `git branch`
- Get all the branch from the repo (before creating a new one)  `git fetch`
- Init your main branch `git init -b` branch's name
- Create a branch `git branch -b` branch's name
- Go on a branch `git checkout` branch's name

### Commit
- Stage `git add . `
- Commit `git commit -m ` "message"

### Push 
- Push your local branch to your distant repo `git push origin` branch's name

### Pull Request (PR)
Once the PR is (squashed and) merged, don't forget to update your local repo (`git checkout master && git pull upstream master`) and your distant repo (`git push origin master`).

# Contexte

### Add a local project to your git :

- Go to your project on a terminal
- Init your main branch
- Commit
- On Github, create a new repository
- Recover URL of your git
- On your terminal, add local project on github command
- Push

Commit : 

- git add “your file.xx” ⇒ What you want to commit.
- git status ⇒ check that it’s the right file.
- git commit -m “message” ⇒ commit and describe the change.
- git push ⇒ on a distant repo.

Commit a mistake before push ? 

- git log ⇒ show informations about latest commits, take the ID of the commit you want to go back.
- git reset “ID” ⇒ with the good commit’s ID.
- git commit —amend ⇒ for amend (modifier) the message.

Copie Paste a repo :

- fork the repo.
- git clone “http…” on your computer.

Team : do Pull Request :

- do a “Copie Paste a repo”.
- git remote add upstream “Original repo” ⇒ bond your repo and the original.
- git branch ⇒ check the branch.
- git branch “NewBranch” ⇒ create a new branch.
- git checkout “NameBranch” ⇒ go on this new branch.
- do your modifications.
- do a “Commit”.
- git push origin “YourBranch” ⇒ modification of your distant repo
    - it should display a link for your pull request.
- Open  a new pull Request.
- git checkout “mainBranch” &&  git pull upstream “mainBranch” ⇒ modification of your local repo.
- git push origin “mainBranch” ⇒ modification of your distant repo.
