# cha1 - git config
-----------------------------
### 1. 最重要的安全和隐私问题
>git config --list 查看所有配置, core 配置 是局部的配置, 往上是 局部的配置
##### 对全局的设置
> git config --global 全局设置
> git config --global user.name ''
> git config --global user.mail ''

对局部的设置
> git config --local 全局设置
> git config --local user.name ''
> git config --local user.mail ''

### 2. 设置别名, 提高工作效率
> git config --global alias.st status
> git config --global alias.pu push
> git config --list

### 3. 设置默认选项

# git clone && git tag 2018/6/1
--------------------------------

### 1. clone 某一个分支

> git clone -b {{name}} {{address}}

### 2. git tag

> git tag -a v0.1 -m "v0.1"         // 打标签
> git push --tag                    // 是推送标签

也可以对多个内容打标签

也可以补充标签
> git log --pretty==oneline
> git tag -a v0.1 afasfasdasf2120 -m "v0.1"
> afasfasdasf2120 是 由第一个命令得到的提交序号

还可以 查看 某一特定的标签

> git tag -l "v0.1"


# git status && git diff
----------------------
### 文件状态类型
> 1. 以追踪的文件
>
> 2. 未追踪的文件

# git branch
-------------------------
> git branch -a                 // 所有分支
> git checkout                  // 切换分支
> git checkout -b               // 创建分支并切换分支
> git merge                     // 分支合并
> 会有 conflict 手动选择 然后记得 git add . && git commit -m 
