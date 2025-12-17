**One-time setup**

```bash
git remote add upstream git@github.com:badlogic/pi-mono.git
git remote set-url --push upstream DISABLED
git fetch upstream

git switch main
git branch --set-upstream-to=upstream/main main
git pull --ff-only
git push origin main
```

**Day-to-day workflow**

```bash
git switch main
git pull --ff-only
git push origin main

git switch markus/main
git rebase main
git push --force-with-lease
```
