# nodejs
如何配置node环境变量
安装node环境
打开node.js的官网https://nodejs.org/zh-cn/download/下载需要的版本的node

下载后如下图所示

点击进行安装，直接下一步即可（注意：Node尽量安装到盘符下，不要出现中文路径）
安装完成之后，通过（Win+R,输入cmd）命令行工具，查看Node是否安装成功
输入node -v查看当前node 的版本

找到Node安装的路径，在当前路径下新建两个文件夹

配置基本信息(注意：需要更改为自己文件夹的路径)
语法：
npm config set prefix  "文件路径"  更改全局安装的目录
npm config set cache  "文件路径" 更改缓存的目录

注意：若写错之后无法更改
通过npm config list可以查看所有的config是否设置成功

找到系统中用户下的.npmrc隐藏文件

配置环境变量

计算机右键->属性->高级系统设置->环境变量

若报以下错误，则代表环境变量不能使用

使用Node的原因：
node中有一个强大的包管理工具：
npm  cnpm(国内的淘宝镜像) npx

语法：
npm install 代表安装     install可以简写为 i
npm uninstall 代表卸载
  -g  global 全局安装
--save        安装到本地文件夹  -S
--save-dev 安装到本地文件夹  -D

安装模块语法：

npm install -g 安装的模块 或者npm install 安装的模块 -g

npm i -g 安装的模块  或者  npm i 安装的模块 -g

卸载模块语法 npm uninstall -g 

卸载的模块 或者 npm uninstall  卸载的模块 -g

