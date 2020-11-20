# GIT FAQ

## How do I update my feature branch that has fallen behind master
i.e. I did some work a short while back, got bored (was distracted by shinier stuff), went away, and now need to pickup again!

```
git checkout master
git pull
git checkout <feature-branch>
git rebase master
git push --force
```

This will update your local master to the latest and greatest changes in remote. And then move those commits over to your local
repo feature branch, and then add your commits onto the end. And finally you will need to push (and force) to replace the remote
history with this new _rebased_ set of commits.

Worth being aware that this will blow away the remote branch and the set of commits it had before. So anyone who was looking at
or using your feature branch will get confused (or broken).
