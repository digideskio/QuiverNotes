#Remove things from GitHub after they're added to .gitignore
- Adding things to .gitignore untracks them, but it doesn't remove them from GitHub.
- Ideally, set up .gitignore before making the first commit so that the things you don't want tracked are never added to GitHub in the first place.

```html
git rm -r --cached .
git add .
git commit -am "Remove ignored files"
```

source: [Making Git forget about a file that was tracked but is now in gitignore](http://stackoverflow.com/questions/1274057/making-git-forget-about-a-file-that-was-tracked-but-is-now-in-gitignore)