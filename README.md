#Git Submodule Tutorial

A simple tutorial for using Git submodules.  
  
[Reference Guide 1](https://chrisjean.com/git-submodules-adding-using-removing-and-updating/)
[Reference Guide 2](http://blog.jacius.info/git-submodule-cheat-sheet/)

---

##Add a repository as a submodule
```sh
git submodule add <repo>
```

##Get the latest submodule repository updates
```sh
cd <path-to-submodule>
```

```sh
git pull
```

```sh
cd ..
```

```sh
git status
```

```sh
git commit -am "Update submodule to latest version"
```

```sh
git push
```

##Clone a Project with Submodules
```sh
git clone <project-repo>
```

```sh
cd <path-to-submodule>
```

The submodule directory will be empty, so we need to initialize and update with contents
```sh
git submodule update -init
```
Shorthand would be:
```sh
git submodule update -i
```
