# help

> git --help
>
> man git
>
> man git-config

# config

> git config
>
> man git-config
>
> git config -l

```
[root@node_106_192.168.183.106 ~]#  git config -l
[root@node_106_192.168.183.106 ~]#  git config --global user.name Kinson.Pan
[root@node_106_192.168.183.106 ~]#  git config --global user.email Kinson@Pan.com
[root@node_106_192.168.183.106 ~]#  git config -l
user.name=Kinson.Pan
user.email=Kinson@Pan.com
[root@node_106_192.168.183.106 ~]#
```

# add

* 将文件添加到暂存区域

> git add FILENAME
>
> git add .

# commit

```
git commit -m "v0.0.1"
```

# log

```
git log：查看提交日志；
```

# init

* 创建或者重新初始化

```
[root@node_106_192.168.183.106 ~/testgit/dir1]#  git init
Initialized empty Git repository in /root/testgit/dir1/.git/
[root@node_106_192.168.183.106 ~/testgit/dir1]#  tree .git/
.git/
├── branches
├── config
├── description
├── HEAD
├── hooks
│   ├── applypatch-msg.sample
│   ├── commit-msg.sample
│   ├── post-update.sample
│   ├── pre-applypatch.sample
│   ├── pre-commit.sample
│   ├── prepare-commit-msg.sample
│   ├── pre-push.sample
│   ├── pre-rebase.sample
│   └── update.sample
├── info
│   └── exclude
├── objects
│   ├── info
│   └── pack
└── refs
    ├── heads
    └── tags

9 directories, 13 files
[root@node_106_192.168.183.106 ~/testgit/dir1]#
```

# clone

```
[root@node_106_192.168.183.106 ~/testgit/dir1]#  cd ../
[root@node_106_192.168.183.106 ~/testgit]#  git clone dir1/ dir1cloned
Cloning into 'dir1cloned'...
warning: You appear to have cloned an empty repository.
done.
[root@node_106_192.168.183.106 ~/testgit]# 
```

# status

```
[root@node_106_192.168.183.106 ~/testgit]#  git status
fatal: Not a git repository (or any of the parent directories): .git
[root@node_106_192.168.183.106 ~/testgit]#  cd dir1
[root@node_106_192.168.183.106 ~/testgit/dir1]#  git status
# On branch master
#
# Initial commit
#
nothing to commit (create/copy files and use "git add" to track)
[root@node_106_192.168.183.106 ~/testgit/dir1]# 
```

# ls-files

```
git ls-files            # 列出索引中的文件列表，使用原始文件名
git ls-files -s         # 显示暂存文件和对象的关系 权限，对象名，暂存号，原始文件名
git ls-files -o         # 显示未被追踪的文件
```

# rm

```
git rm：删除工作目录中的文件，及索引中的映射；
git rm --cached：只删除索引中的映射；
```

# mv

```
git mv：改变工作目录中的文件名，及索引中的映射；
```































































