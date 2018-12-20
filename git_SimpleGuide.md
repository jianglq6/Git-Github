# Git - the simple guide

https://git-scm.com/doc

    add     ->     commit    ->     push
  (workspace)   (stage:local)  (branch: repository)  

## Getting Start
### Configuration
```shell
$ git config --global user.name "<your.username>"
```
``` shell
$ git config --global user.email "<your.emal.adderss>"
```
！！！除非你只用一个git账号，如果有公司或者小组账号的话，git有三种配置选项，分别对应--system, --global, --local ！！！


### Getting Help
``` shell
$ git help <verb>
$ man git <verb>
```
These commands can be accessed anywahere, even offline.

If you just need a quick refersher on the available options for a Git command:
```shell
$ git <verb> -h
```
or
```shell
$ git <verb> --help
```

## Creat a new repository
``` shell
$ git init
```

## Checkout a repository
creat a working copy of a local repository by running the command
``` shell
$ git clone /path/to/repository
```
when using a remote server, your command will be
```shell
$ git clone username@host:/path/to/repository
```

## Checking the Status of Your Files
``` shell
$ git status
```

## Change and Commit 
#### Tacking new files
``` shell
$ git add <filename>
```
This is the first step in the basic git workflow. To actually commit these changes use.
#### Staging modified files
``` shell
$ git status
```
#### View changes
``` shell
$ git diff
```
#### Commit changes
``` shell
$ git commit -m "Commit message"
```

## Pushing changes
To send those changes to your remote repository, execute 
``` shell
$ git push origin master
```

If you have not cloned an existing repository and want to connect your repository to a remote server, you need to add it with
``` shell
$ git remote add origin <server>
```

## Branching
Create a new branch named "new" and switch to it using
``` shell
$ git checkout -b new
```

switch back to master
``` shell
$ git checkout master
```

delete the branch again
``` shell
$ git branch -d new
```

a branch is not available to others unless you push the branch to your remote repository
``` shell
$ git push origin <branch>
```
## Update && Merge
To update your locat repository to the newest commit
``` shell
$ git pull
```

To merge another branch into your active branch, use
``` shell
$ git merge <branch>
```

After changing, you need to mark them as merged with
``` shell
$ git add <filename>
```
before merging changes, you can also preview them by using
``` shell
$ git diff <source_branch> <target_branch>
```

如何利用好分支 https://www.zhihu.com/question/21995370
