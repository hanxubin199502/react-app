# react环境搭建及其项目的启动 打包部署

 - 1.首先准备的东西
 - a.安装node js（下载安装node 一路回车就可以）
 - b.安装npm（因为国内使用npm很慢所以需要安装cnpm）
 - c.安装cnpm（npm install -g cnpm --registry=https://registry.npm.taobao.org）
说明：检测自己是否安装node npm cnpm使用node -v， npm -v，cnpm -v

 # - 2.搭建环境
 - a.开始搭建自己react项目的环境，找到自己需要放项目的文件夹（新建一个文件夹即可） 例：F：\reactapp -> 地址栏中   输入cmd出现命令框
 - b.执行cnpm install -g create-react-app（是全局安装）
 - c.执行 create-react-app react_app(项目名称)
 - d.在这里重点说明一下创建自己项目的时候有可能会报错Unexpected end of JSON input while parsing near '....0","dependencies":{"' 也有可能不报错，如果报错的话就执行npm cache clean --force
 - e.走到这一步项目就已经创建完成了只需要找到项目的根目录执行 npm start启动项目就ok了

 # - 3.启动项目执行npm start 

 # - 4.编译打包执行 npm run build

 # - 5.将本地项目和github仓库相关联并上传项目
 - a.登录自己的github库，点击右上角加号选择 New repository新建仓库，在Repository name栏下填写项目名称，选择开放或者隐私，最后点击Create repository创建仓库完成，号外 号外 号外重要的事情说三遍 记住ssh后面的地址记得复制后面会用到
 - b.找到自己搭建的项目的根目录 鼠标右击选择 git bash here
 - c.执行 git init
 - d.再执行 git add .
 - e.再再执行git commit -m '备注信息'
 - f.再再再执行git remote add origin 你复制的地址（上面说到的这里用到了说明：这里执行的目的是将本地和仓库进行关联）
 - g.最后一步就是将本地代码推到仓库执行 git push -u origin master(这里是你需要推的分支，默认是master分支)
 - h.假如你是仓库的管理者需要拉取合作者加入项目的时候则需要在github库中进入项目目录下找到设置也就是settings -> collaborators这个时候就会
 出现你需要添加的地方 在框中输入被邀请人的用户名或者邮箱都可以，点击add collaborator 对方邮箱或者github库收到验证通过信息，对方通过后 如果
 你在库中列表中看到了就说明成功了，
 - i.这里提一个很多人不知道的操作啊 就是好多人执行完git log后就不知道怎么退出这个命令 直接在英文状态下按下键盘的Q键就可以退出当前这个命令

 # - 6.本地项目的上传与拉取
 - a.git pull （拉取项目）
 - b.git add -A (合并代码)
 - c.git commit -m '备注信息'
 - d.git push -u origin master (将代码推到远程仓库)
 - e.git diff 查看改变
 - f.git status 查看状态
 - g.git remote -v 查看本地与远程仓库关联的地址
 - h.git remote rm origin 地址 移出本地与远程仓库的关联（暂时可以用这个，因为没有亲身实测过所以待我反复测试后再更新）
 
 # - 7.前端最常用的集中编辑器
 - a.Sublime Text3（这个对于前端的初学者非常之好用，简单，自带汉化包，不需要安装任何插件）
 - b.HBuilder （这个编辑器功能就比较多，这个编辑器有好多模式，有开发视图，边改边看模式，webview调试模式，团队同步视图，这几种模式要主要说一下，开发视图就是我们平时开发写代码的模式没有其他的辅助功能，边改边看模式就厉害了它的作用是在编辑器内部就可以打开网页一边修改一边看不需要切换到浏览器中去看，使用起来很方便，webview调试模式则是需要连接手机调试的，团队同步视图好像是没有什么变化，就是把窗口放大了，我理解的是可能想给大家放大了展示代码吧）
 - c.VS Code 和hbuilder差不多就是没有hbuilder那么多功能 速度特别快 还是推荐使用的(一直在用)
