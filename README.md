
# Git Commands

```
# create new branch
git checkout -b branch-name

# interactive staging
git add -i

# log
git log master --oneline
```

### tag

```
# Assign a tag to a commit
git tag -a v1.1 -m "Version 1.0" dd5c49420a8

# create a tag (next commit)
git tag v0.1

# list tags
git tag --list

# list tags benning with "v2"
git tag --list "v2*"

# push tag to remote
git push origin v1.1
```
## cherry pick

##### picking a commit
```
git cherry-pick sha1
```
