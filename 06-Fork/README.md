# Fork
This is when we clone a repository that isn't ours. It's only possible with public projects on GitHub. So we need to click on the FORK button on the top-right to start.

## So to start we need to clone the repo that was created with our name that we fork recently.
```bash
git clone https://github.com/<ournickname>/<repo-forked>
```
Now, we can start to work normally. When we fork a project on GitHub, you become the owner of the forked repository, but with a common history of commits to the original. So we can run `push`, and `pull`, make branches, tags, etc.

## How do make merge our changes with the original repository?
In our version of the repo in GitHub we gonna have a button called "New pull request", if we press there, it shows us a new window where we need to select the branch that we gonna merge and the branch of the original repo where we want to apply the changes.

Then, when we are sure about the changes we press the button called "Create pull request". So this shows us a screen to make the pull request (we are asking the owner of the original repo if we can add our changes to their repo)

Now, just we need to wait for the response.

## How to pull latest changes from the original repo to my forked repo?
To do this, follow the next commands. First we need to add the original repo as remote link in our repository.
```bash
# show all our remote links
git remote -v

# Add new remote link
git remote add upstream https://github.com/<original-owner-nick>/<repo-name>.git
```

Then of added it, we need to pull the changes, and push it to our repo. So run:
```bash
# getting changes
git pull upstream master
```
"upstream" is a pointer to the original repo.

```bash
# sending changes to our repo
git push origin master
```