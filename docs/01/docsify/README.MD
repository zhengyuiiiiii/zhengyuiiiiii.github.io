## 01、在GitHub上新建一个存储库
注意命名 zhengyuiiiiii.github.io

---

## 02、安装git并连接github
git链接地址：[链接](https://git-scm.com/download)

---

## 03、生成一个ssh key放到github中
> ssh -keygen -t rsa -C "452885853@qq.com"

一路回车，在出现选择时输入Y，再一路回车直到生成密钥。会在/Users/86159/路径下生成一个.ssh文件夹，密钥就存储在其中。可以在提示的那个/Users/xx/路径中用记事本打开id_rsa.pub,并把那段内容复制到github的setting的SSH and GPG keys，选择add keys。

---

## 04、用vscode部署
以vscode作为预设的editor，在终端输入git init
> git init

启动


> git config_--globaluser.name"zhengyuiiiiii"_

> git config_--globaluser.email"452885853@qq.com"_

设置好之后，可以验证
> git config --global --list



继续在终端输入
> **ssh -T **git@github.com:zhengyuiiiiii/zhengyuiiiiii.github.io.git

之后会有个提示你输入yes，就可以连接成功了


然后在vscode的终端输入
> git remote add origin git@github.com:zhengyuiiiiii/zhengyuiiiiii.github.io.git


```
git remote add origin git@github.com:zhengyuiiiiii/zhengyuiiiiii.github.io.git
```