# Sync another repo into existing repo


```
// By default it will show like this
$ git remote -v
origin  https://github.com/navdeepsingh/test.git (fetch)
origin  https://github.com/navdeepsingh/test.git (push)

// and to add new repo to sync
$ git remote add sync https://github.com/anotherrepo/anotherrepo.git

//after that
$ git remote -v
origin  https://github.com/navdeepsingh/test.git (fetch)
origin  https://github.com/navdeepsingh/test.git (push)
sync  https://github.com/anotherrepo/anotherrepo.git (fetch)
sync  https://github.com/anotherrepo/anotherrepo.git (push)
```

