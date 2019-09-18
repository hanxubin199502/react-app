react环境搭建及其项目的启动 打包部署



1.首先准备的东西
a.安装node js（下载安装node 一路回车就可以）
b.安装npm（因为国内使用npm很慢所以需要安装cnpm）
c.安装cnpm（npm install -g cnpm --registry=https://registry.npm.taobao.org）
说明：检测自己是否安装node npm cnpm使用node -v， npm -v，cnpm -v

2.搭建环境
a.开始搭建自己react项目的环境，找到自己需要放项目的文件夹（新建一个文件夹即可） 例：F：\reactapp -> 地址栏中   输入cmd出现命令框
b.执行cnpm install -g create-react-app（是全局安装）
c.执行 create-react-app react_app(项目名称)
d.在这里重点说明一下创建自己项目的时候有可能会报错Unexpected end of JSON input while parsing near '....0","dependencies":{"' 也有可能不报错，如果报错的话就执行npm cache clean --force
e.走到这一步项目就已经创建完成了只需要找到项目的根目录执行 npm start启动项目就ok了

3.启动项目执行npm start 

4.编译打包执行 npm run build