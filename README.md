---

# 1. Setup & Configuration (First-time use)

```bash
git config --global user.name "Name"
git config --global user.email "email@example.com"
git config --global core.editor vim
git config --global init.defaultBranch main
git config --list
git help <command>
```

---

# 2. Repository Creation & Cloning (Start Working)

```bash
git init
git init <directory>
git clone <repo-url>
git clone <repo-url> <directory>
```

---

# 3. Basic File Tracking (Daily Basics)

```bash
git status
git add <file>
git add .
git add -A
git restore <file>
git restore --staged <file>
git commit -m "message"
git commit
git commit --amend
```

---

# 4. Viewing History & Changes

```bash
git log
git log --oneline
git log --graph --all
git log --stat
git log --patch
git show
git show <commit>
git diff
git diff --staged
git diff <commit1> <commit2>
```

---

# 5. Branching & Navigation

```bash
git branch
git branch <name>
git branch -d <name>
git branch -D <name>
git branch -a
git switch <branch>
git switch -c <branch>
git checkout <branch>          # legacy
git checkout -b <branch>       # legacy
git checkout <file>
```

---

# 6. Merging & Rebasing

```bash
git merge <branch>
git merge --no-ff <branch>
git merge --abort
git rebase <branch>
git rebase -i <commit>
git rebase --continue
git rebase --abort
git rebase --skip
```

---

# 7. Remote Repositories (Collaboration)

```bash
git remote
git remote -v
git remote add origin <url>
git remote remove origin
git remote rename origin upstream
git fetch
git fetch --all
git pull
git pull --rebase
git push
git push origin <branch>
git push -u origin <branch>
git push --force
git push --force-with-lease
```

---

# 8. Undoing & Recovery (Critical Skills)

```bash
git reset --soft <commit>
git reset --mixed <commit>
git reset --hard <commit>
git revert <commit>
git revert --no-commit <commit>
git reflog
git checkout HEAD~1
```

---

# 9. Stashing (Temporary Work)

```bash
git stash
git stash push
git stash list
git stash show
git stash apply
git stash pop
git stash drop
git stash clear
```

---

# 10. Tagging & Releases

```bash
git tag
git tag <tag>
git tag -a <tag> -m "message"
git tag -d <tag>
git show <tag>
git push origin <tag>
git push origin --tags
```

---

# 11. Cleaning & Maintenance

```bash
git clean -n
git clean -f
git clean -fd
git gc
git fsck
git prune
```

---

# 12. Searching & Inspection

```bash
git grep "text"
git blame <file>
git shortlog
git describe
```

---

# 13. Advanced History Rewriting

```bash
git cherry-pick <commit>
git cherry-pick --abort
git cherry-pick --continue
git filter-branch
git replace
git rerere
```

---

# 14. Submodules & Subtrees

```bash
git submodule add <repo>
git submodule init
git submodule update
git submodule update --remote
git submodule foreach
git subtree add --prefix=<dir> <repo> <branch>
git subtree pull --prefix=<dir> <repo> <branch>
```

---

# 15. Hooks, Attributes & Ignore

```bash
git config core.hooksPath
git check-ignore -v <file>
.gitignore
.gitattributes
```

---

# 16. Worktrees & Multiple Checkouts

```bash
git worktree add <path> <branch>
git worktree list
git worktree remove <path>
```

---

# 17. Bisect (Debugging Tool)

```bash
git bisect start
git bisect bad
git bisect good <commit>
git bisect run <command>
git bisect reset
```

---

# 18. Archives & Exporting

```bash
git archive --format=zip HEAD > code.zip
git bundle create repo.bundle --all
git bundle verify repo.bundle
```

---

# 19. Credential & Security

```bash
git config --global credential.helper store
git config --global gpg.program gpg
git commit -S
git verify-commit
git verify-tag
```

---

# 20. Plumbing Commands (Low-level / Internal – Advanced)

```bash
git hash-object
git cat-file
git rev-parse
git update-index
git write-tree
git commit-tree
git read-tree
git symbolic-ref
git show-ref
git for-each-ref
```

---

# 21. Rare but Valid Commands

```bash
git daemon
git instaweb
git notes
git notes add
git notes show
git format-patch
git send-email
```

---
