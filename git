1.配置提交用户名邮箱
git config user.name 'lj01583044'  
git config user.email 'lj01583044@alibaba-inc.com'

git终端管理 https://ohmyz.sh/#install 
node需要重新挂载


curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.2/install.sh | bash 下载nvm
点击菜单栏 图标，即可添加任务



2.git 操作
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
● 

● git reset --soft head~1      撤销上次提交的操作
● git  log   展示提交信息
● Git-叹为观止的 log 命令 & 其参数_DRPrincess的博客-CSDN博客_git log





更新代码
    git  add .
● git commit -m 'fix: to #45934669'   提交到本地git仓库
● git  checkout    develop   切换到主分支上
● git  pull  将代码拉下来
● (git pull origin develop)  不用切换到主分支
● git   checkout   lijie/fix/dev/45934669   切换到目标分支
● git   merge  develop   目标分支与develop分支合并
● 在执行 
● git  add .
● git commit -m 'fix: to #45934669'   提交到本地git仓库
● git push origin master（本地要推送的分支名）的意思就是上传本地当前分支代码到master分支。git push是上传本地所有分支代码到远程对应的分支上。（使用）
● git push -u origin master（本地要推送的分支名） 上面命令将本地的master分支推送到origin主机，同时指定origin为默认主机，后面就可以不加任何参数使用git push了





● git branch > text.txt    查看分支并创建一个txt文本展示
● git relog 查看历史版本的提交记录
● 占位标签解析：
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




3.nvm 管理node 操作
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
