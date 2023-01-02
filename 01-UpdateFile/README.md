# Let's create a file and then update it

### To create a file, we gonna do:
```bash
touch <name-file>
```
Then we gonna write something inside the file, like `"This a text"`

### Now, if we run `git status` we can see that exists changes. So we gonna track the file.
To do that, we need to run the next command:
```bash
git add .
```
or
```bash
git add <name-file>
```

### Cool, now let's commit and push it
To commit it:
```bash
git commit -m "First commit"
```
To push it to the repo:
```bash
git push
```

### If we run now `git status`, we can see that now there are no changes anymore, let's update the file now
Just update the text in the file, like `"This is a content"`
And now run `git status` again, are you saw some changes?
That 'cause we update the file, so we need to track it again, commit it and push it.

To commit it:
```bash
git commit -m "Updated File"
```
To push it to the repo:
```bash
git push
```