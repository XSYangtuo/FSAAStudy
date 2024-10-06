# 配置环境
## vscode配置
- （选做）如果不适应英文环境的vscode，可以下载中文语言包，在扩展中搜索`Chinese`，然后安装。
## 远程git的连接（以浙大版gitlab为例）
- 先登录[https://git.zju.edu.cn/](https://git.zju.edu.cn/){:target="_blank"}注册自己的zju git账号（记得连接校网）
- 首先，在终端中输入`git config --global user.name "your name"`和`git config --global user.email "your email"`来设置你的用户名和邮箱。
- 然后输入`ssh-keygen -t rsa -C "your email"`来生成ssh密钥。
- 然后根据提示寻找生成的密钥文件，默认文件名是叫`id_rsa.pub`。（注意查看里面的fingerprint）
- 打开这个文件，复制里面的内容。
- 登录zju git，点击右上角的头像，选择`Settings`，然后选择`SSH Keys`，将刚才复制的密钥粘贴到`Key`中，然后点击`Add Key`。
- 然后输入`ssh -T git@git.zju.edu.cn`来测试连接是否成功。（有可能会需要输入fingerprint）
- 如果连接成功，会显示欢迎信息。
## 创建工作目录并拉取内容
- 创建一个新文件夹，在用vscode打开这个文件夹。
- 快捷键"ctrl+~"打开终端，输入`git init`来初始化git仓库。
- 在仓库页面（FSAA的页面为[https://git.zju.edu.cn/fsaa/fsaa](https://git.zju.edu.cn/fsaa/fsaa){:target="_blank"}）中点击 `code`，然后选择`SSH`，复制链接。
- 在终端中输入`git remote add origin 你复制的链接`来添加远程仓库。
- 输入`git pull origin master`来拉取远程仓库的内容，这时工作区将会出现相应mkdocs项目文件
- 输入`mkdocs serve`来启动mkdocs服务，在浏览器中打开[http://127.0.0.1:8000/](http://127.0.0.1:8000/){:target="_blank"}即可看到mkdocs项目的内容。如果能成功看到内容，说明环境配置成功。