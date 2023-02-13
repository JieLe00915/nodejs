### 1.配置提交用户名邮箱
git config user.name 'lj01583044'  
git config user.email 'lj01583044@alibaba-inc.com'

git终端管理 https://ohmyz.sh/#install 
node需要重新挂载


curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.2/install.sh | bash 下载nvm
点击菜单栏 图标，即可添加任务



### 2.git 操作
Git 基本操作 | 菜鸟教程 (runoob.com)
【Git】commit提交代码_春天的菠菜的博客-CSDN博客_git提交commit
git基本操作，一篇文章就够了！ - 掘金 (juejin.cn)

● git init - 初始化仓库
 
● git add . - 添加文件到暂存区。
 
● git commit - 将暂存区内容添加到本地仓库中。
 
● git checkout -b lijie/fix/dev/45934669    创建切换到该分支 

● git branch    查看分支

● git commit -m 'fix: to #45934669'  提交到仓库  编号为需求上的     vscode点击也能直接提交

● git commit --no-verify -m "commit"   就可以跳过代码检查

● git reset --soft head~1      撤销上次提交的操作

● git  log   展示提交信息

● Git-叹为观止的 log 命令 & 其参数_DRPrincess的博客-CSDN博客_git log





### 更新代码
  git  add .
  
● git commit -m 'fix: to #45934669'   提交到本地git仓库

● git  checkout    develop   切换到主分支上

● git  pull  将代码拉下来

● (git pull origin develop)  不用切换到主分支

● git   checkout   lijie/fix/dev/45934669   切换到目标分支

● git   merge  develop   目标分支与develop分支合并

### 在执行 
● git  add .

● git commit -m 'fix: to #45934669'   提交到本地git仓库

● git push origin master（本地要推送的分支名）的意思就是上传本地当前分支代码到master分支。git push是上传本地所有分支代码到远程对应的分支上。（使用）

● git push -u origin master（本地要推送的分支名） 上面命令将本地的master分支推送到origin主机，同时指定origin为默认主机，后面就可以不加任何参数使用git push了





● git branch > text.txt    查看分支并创建一个txt文本展示

● git relog 查看历史版本的提交记录

### ● 占位标签解析：
type:代表某次提交的类型，比如是修复一个bug还是增加一个新的feature。
所有的type类型如下：

scope:scope说明commit影响的范围。scope依据项目而定

subject:是commit的简短描述

body:提交代码的详细描述

footer:如果代码的提交是不兼容变更或关闭缺陷，则Footer必需，否则可以省略。

feat[特性]:新增feature 

fix[修复]: 修复bug     

docs[文档]: 仅仅修改了文档，比如README, CHANGELOG, CONTRIBUTE等等

style[格式]: 仅仅修改了空格、格式缩进、都好等等，不改变代码逻辑

refactor[重构]: 代码重构，没有加新功能或者修复bug

perf[优化]: 优化相关，比如提升性能、体验

test[测试]: 测试用例，包括单元测试、集成测试等

chore[工具]: 改变构建流程、或者增加依赖库、工具等

revert[回滚]: 回滚到上一个版本




### 3.nvm 管理node 操作
brew install nvm

vim .zshrc  配置环境变量


export NVM_DIR="$HOME/.nvm"
  [ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && \. "/opt/homebrew/opt/nvm/nvm.sh"  # This loads nvm
  [ -s "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm" ] && \. "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm"  # This loads nvm bash_completion
：将文件放入  i 编辑  esc  shift+：wq(!强制退出)   x(保存)

source .zshrc

nvm ls remote

nvm install 14.20

nvm  alias default  14.20

nvm ls


1. git配置命令
查询配置信息
1. 列出当前配置：git config --list;
2. 列出repository配置：git config --local --list;
3. 列出全局配置：git config --global --list;
4. 列出系统配置：git config --system --list;
第一次使用git，配置用户信息
1. 配置用户名：git config --global user.name "your name";
2. 配置用户邮箱：git config --global user.email "youremail@github.com";
其他配置
1. 配置解决冲突时使用哪种差异分析工具，比如要使用vimdiff：git config --global merge.tool vimdiff;
2. 配置git命令输出为彩色的：git config --global color.ui auto;
3. 配置git使用的文本编辑器：git config --global core.editor vi;
2. 工作区上的操作命令
新建仓库
1. 将工作区中的项目文件使用git进行管理，即创建一个新的本地仓库：git init；
2. 从远程git仓库复制项目：git clone <url>，如：git clone git://github.com/wasd/example.git;克隆项目时如果想定义新的项目名，可以在clone命令后指定新的项目名：git clone git://github.com/wasd/example.git mygit；
提交
1. 提交工作区所有文件到暂存区：git add .
2. 提交工作区中指定文件到暂存区：git add <file1> <file2> ...;
3. 提交工作区中某个文件夹中所有文件到暂存区：git add [dir];
撤销
1. 删除工作区文件，并且也从暂存区删除对应文件的记录：git rm <file1> <file2>;
2. 从暂存区中删除文件，但是工作区依然还有该文件:git rm --cached <file>;
3. 取消暂存区已经暂存的文件：git reset HEAD <file>...;
4. 撤销上一次对文件的操作：git checkout --<file>。要确定上一次对文件的修改不再需要，如果想保留上一次的修改以备以后继续工作，可以使用stashing和分支来处理；

3. 暂存区上的操作命令
提交文件到版本库
1. 将暂存区中的文件提交到本地仓库中，即打上新版本：git commit -m "commit_info";
2. 将所有已经使用git管理过的文件暂存后一并提交，跳过add到暂存区的过程：git commit -a -m "commit_info";
3. 提交文件时，发现漏掉几个文件，或者注释写错了，可以撤销上一次提交：git commit --amend;
查看信息
1. 比较暂存区与上一版本的差异：git diff --cached;
2. 指定文件在暂存区和本地仓库的不同：git diff <file-name> --cached;
3. 查看提交历史：git log；参数-p展开每次提交的内容差异，用-2显示最近的两次更新，如git log -p -2;

