# A Branch
It's like a separate new version of your project, and anything that you changes there it isn't modified the principal version of your project (Except when you make a MERGE, we talk bout it later). So, you can manage the same project but with separate version though, without risks for Master/Main branch.
This helps us to make different versions like for "hotfix" (bug fixing), "development", "production", and so on.

# A Merge
When we have two version of one project (kinda Master and Hotfix for example) where we solved some bugs, and we need to MERGE it to the Master/Main branch. Merge helps us to "apply" the changes from a branch to other. This sound really cool, but we could have some conflicts when we merge two branches.

# A cool command that show you the branches
Graphic and simple history of the branches
```bash
git log --all --oneline -5 --decorate --graph
```
To print the existing branches and them history
```bash
git show-branch -all
```
Open a software that help you to manage your git-project (kinda console but more intuitive tho)
```bash
# anyway you can install it with "sudo apt install gitk"

gitk
```