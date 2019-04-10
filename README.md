# Git Submodule Tutorial
Include other Git repositories in repositories.

**Table of Contents**
* [Git Submodules to the Rescue](#git-submodules-to-the-rescue)
* [Your First Submodule](#your-first-submodule)
* [Update a Submodule](#update-a-submodule)
* [Clone a Project with Submodules](#clone-a-project-with-submodules)

## Git Submodules to the Rescue


## Your First Submodule
**Add a repository as a submodule**
```sh
git submodule add <repo>
```

## Update a Submodule
**Get the latest submodule repository updates**
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

## Clone a Project with Submodules
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

## Clone a Project with Submodules and their contents
```sh
git clone --recursive <project-repo>
```

## Update all submodules for a project already cloned
```sh
git submodule foreach git pull origin master
```

---
[Reference Guide 1](https://chrisjean.com/git-submodules-adding-using-removing-and-updating/)  
[Reference Guide 2](http://blog.jacius.info/git-submodule-cheat-sheet/)
