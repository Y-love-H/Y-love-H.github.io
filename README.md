Y-love-H
介绍
{以下是 Gitee 平台说明，您可以替换此简介 Gitee 是 OSCHINA 推出的基于 Git 的代码托管平台（同时支持 SVN）。专为开发者提供稳定、高效、安全的云端软件开发协作平台 无论是个人、团队、或是企业，都能够用 Gitee 实现代码托管、项目管理、协作开发。企业项目请看 https://gitee.com/enterprises}

软件架构
hexo[框架]＋Hexo-Theme-Async[主题]+gitee[代码托管平台]+HexoPro[后台]

安装教程
一、准备工作
1.可参考官方文档
Hexo 是一个快速、简洁且高效的博客框架。Hexo 使用 Markdown（或其他标记语言）解析文章，在几秒内，即可利用靓丽的主题生成静态网页
2.配置环境
这里我们需要下载安装两个软件，我们就去官网下载一下 node.js 和 git
Nodejs下载安装
git下载安装
3. 安装 Hexo
npm install -g hexo-cli
二、项目搭建 1.初始化项目
blog为项目的名称
hexo init blog
2.本地运行项目
hexo clean //清空已经存在的hexo网站文件
hexo generate (可简写g) //依据网页文件和新的css样式生成新的网站文件
hexo server (可简写为s) //启动本地服务器，可以在localhost：4000查看网站修改效果
(如果4000端口被占用可用“ hexo server -p 5000 ”启动项目)
先进入到项目的根目录
cd webstack
编译运行
hexo g
hexo s
默认端口为4000，在浏览器访问 http://localhost:4000/
三、替换主题
1.主题下载
官方主题列表
下载主题
cd themes
_git clone https://github.com/HCLonely/hexo-theme-webstack_
2.修改主题名称
将hexo-theme-webstack修改为webstack
修改_config.example.yaml 为 _config.webstack.yaml
移动_config.webstack.yaml到根目录下
修改主题名称为webstack
3. 本地运行
hexo clean
hexo g
hexo s
四.快速开始
1.安装Hexo pro
npm install --save hexo-pro
hexo server -d
open http://localhost:4000/pro/
2.配置登陆账户与密码
需要在hexo的_config.yml中增加以下配置来使用账户密码登陆后台，
不配置后台会直接登陆。 配置后使用jwt来保护后台访问的接口

hexo_pro:
  username: admin
  password: 123
  avatar: https: image for your own avata
  secret: xxx // jwt secret key
使用说明
xxxx
xxxx
xxxx
参与贡献
Fork 本仓库
新建 Feat_xxx 分支
提交代码
新建 Pull Request
特技
使用 Readme_XXX.md 来支持不同的语言，例如 Readme_en.md, Readme_zh.md
Gitee 官方博客 blog.gitee.com
你可以 https://gitee.com/explore 这个地址来了解 Gitee 上的优秀开源项目
GVP 全称是 Gitee 最有价值开源项目，是综合评定出的优秀开源项目
Gitee 官方提供的使用手册 https://gitee.com/help
Gitee 封面人物是一档用来展示 Gitee 会员风采的栏目 https://gitee.com/gitee-stars/
