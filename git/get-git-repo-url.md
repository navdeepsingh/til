# Get git repo url by command

THe following command can ask your key

```
git remote show origin | grep 'Fetch URL'
// or
git remote -v
```

To avoid being asked for the key, use -n option
