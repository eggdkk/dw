## 配置git

1. ssh-keygen -t rsa -C "monitor200@outlook.com"；

2. 讲生成的公钥放到github里面的 ssh—key里面

3. ssh -T git@github.com   出现continue点yes 得到You've successfully authenticated, but GitHub does not provide shell access. 表示成功创建

4. git config --global user.email "you@example.com" 设置邮箱

5.  git config --global user.name "Your Name" 设置用户名

   ### 文件上传

6.  git clone  https://github.com/monitor403/dw.git 下载仓库的源码

7. cd /文件目录下，手动添加文件 git add 。。。

8. git commit -m "文件备注信息"

9.  git remote add origin https://github.com/monitor403/dw.git 连接远程上的仓库，如果使用git bash 连接显示 **fatal: not a git repository (or any of the parent directories): .git** 则  **git init**  始化在连接。

10. git push -u origin master   推送上传

## 删除，更新仓库文件

1. git rm --cached filename
2. git commit -m "备注信息“
3.  git push -u origin master 推送
4. git fetch从远程仓库下载分支及数据，git merge从远程仓库提取数据并合并到当前分支 

## zsh安装

```
 apt-get update
 apt-get install zsh -y
```

```
sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"安装oh my zsh
```

## i3安装

```html
apt-get install i3 feh  i3status dmenu i3lock xbacklight  conky
```

进入界面之后就一顿回车就ok

快捷键：**alt+enter**创建新的终端，**alt+v** 垂直分割，**alt+h** 水平分割，**alt+d** 调出应用搜索，**alt+shift+e** 退出i3界面，**alt+shift+q**退出应用。