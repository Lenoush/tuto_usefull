## Presentation de Git 
https://docs.google.com/presentation/d/1vfsG__2-T7xJYGKFs9HfPKmaoMN1Je0V0h7gLyiY1AU/edit?usp=sharing 

## Pré ConditionThese steps assume that you [have installed git locally](https://www.atlassian.com/fr/git/tutorials/install-git), that you [have created a GitHub account](https://github.com/join), and [have added your local ssh key](https://help.github.com/en/enterprise/2.15/user/articles/adding-a-new-ssh-key-to-your-github-account) to it.

## Fork a Repo


Add a local project to your git :

- go to your project on a terminal.
- git init -b “mainBranch” ⇒ init your main branch.
- do a “Commit”.
- go on Github and create a new repository.
- recover URL of your git.
- go on your terminal.
- git remote add origin “URL”. ⇒ bond
- git remote -v ⇒ check the URL
- git push -u origin main

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
