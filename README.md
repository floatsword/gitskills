
# Git 常用命令

- `git init`： 创建版本库

- `git status`：查看当前git 仓库状态

- `git add`： 将文件\修改提交到暂存区

- `git commit`：将文件\修改从暂存区提交到分支

- `git log`：查看提交日志

- `git reset`： 回退到指定版本

- `git reflog`： 查看所有分支的所有操作记录

- `git checkout -- file`： `git checkout -- readme.txt`意思就是，把`readme.txt`文件在工作区的修改全部撤销，这里有两种情况：

  - `readme.txt`自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态。

  - `readme.txt`已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。

    总之，就是让这个文件回到最近一次`git commit`或者`git add `时的状态

- `git checkout 分支名`： 切换分支

- `git merge 分支名`： 合并分支

- `git branch 分支名`： 创建分支

- `git branch -D 分之名`： 删除分支

### 远程版本库操作

- `ssh-keygen -t rsa -C "457009712@qq.com"`：创建秘钥
- `git remote add origin diz 库`：关联远程库
- `git push -u origin master 内容`：推送分支