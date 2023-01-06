# Tags
### To make a tag you need to run the next command with the commit-id
```bash
# "v0.1" is the name of version, common usage is "v0.1", "v0.2", "v1.1", etc
# <commit-id> example: 60ae10e

git tag -a v0.1 -m "Some message for the version" <commit-id>
```
and show you a list of tags, you can execute
```bash
git show-ref --tags
```

### Then to push the tags to the repo:
```bash
git push origin --tags
```

### How to remove a tag?
```bash
git tag -d <name-tag>
```
then you need to push it, to save it. To do this we gonna run the next commands:
```bash
git push origin --tags
```
```bash
# we need to run this command cuz with this one you delete the tag in github
git push origin :refs/tags/<name-tag-deleted>
```