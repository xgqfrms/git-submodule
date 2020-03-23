# git-submodule


https://git-scm.com/book/zh/v2/Git-%E5%B7%A5%E5%85%B7-%E5%AD%90%E6%A8%A1%E5%9D%97


```sh
$ git submodule -h



➜  mweb git:(master) ✗ git submodule -h
usage: git submodule [--quiet] add [-b <branch>] [-f|--force] [--name <name>] [--reference <repository>] [--] <repository> [<path>]
   or: git submodule [--quiet] status [--cached] [--recursive] [--] [<path>...]
   or: git submodule [--quiet] init [--] [<path>...]
   or: git submodule [--quiet] deinit [-f|--force] (--all| [--] <path>...)
   or: git submodule [--quiet] update [--init] [--remote] [-N|--no-fetch] [-f|--force] [--checkout|--merge|--rebase] [--[no-]recommend-shallow] [--reference <repository>] [--recursive] [--] [<path>...]
   or: git submodule [--quiet] summary [--cached|--files] [--summary-limit <n>] [commit] [--] [<path>...]
   or: git submodule [--quiet] foreach [--recursive] <command>
   or: git submodule [--quiet] sync [--recursive] [--] [<path>...]
   or: git submodule [--quiet] absorbgitdirs [--] [<path>...]


```


![image](https://user-images.githubusercontent.com/7291672/77306322-765fbe80-6d32-11ea-9e98-e4f0e9276f8b.png)


***


## git submodule tutorials

https://git-scm.com/book/en/v2/Git-Tools-Submodules

https://git-scm.com/docs/git-submodule

> steps

```sh
# step 01: create an empty submodule folder
$ mkdir demo_repo

# step 02: git submodule add
$ git submodule add http://git.xgqfrms.xyz/git-submodule

```
### step 03: create an `.gitmodules` config file

```.gitmodules

[submodule "demo_repo"]
  path = demo_repo
  url = http://git.xgqfrms.xyz/git-submodule.git

```

```sh
# step 04: init submodule
$ git submodule init

# step 05: clone submodule
$ git submodule update

```
