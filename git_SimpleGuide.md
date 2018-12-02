# Git - the simple guide

https://git-scm.com/doc

## Getting Start
### Configuration
```shell
$ git config --global user.name "<your.username>"
```
``` shell
$ git config --global user.email "<your.emal.adderss>"
```

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

## Tacking new files
``` shell
$ git add <filename>
```
This is the first step in the basic git workflow. To actually commit these changes use.


