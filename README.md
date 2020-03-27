# Config GitHub how to relate to local repository
[参考教程](https://blog.csdn.net/qq_38716242/article/details/79380825) 
## 1.Verfy the network to GitHub via terminal
ssh -T git@github.com
## 2.Install SSH key
cd ~/.ssh  
ls   
> 查看该 .ssh 目录下是否已经具有ssh keys，即 id_rsa（私钥）和 id_rsa.pub（公钥）这两个文件  
> 如果有记得 先备份当前的这两个文件

## 3.Add your Github account
ssh-keygen -t rsa -C "你自己的github对应的邮箱地址"  
>1：""是需要的  
>2：该命令是在.ssh目录下进行的！  
>3: id_rsa（私钥）和id_rsa.pub（公钥）这两个文件被创建了  
## 4.Add SSH key to GitHub account
# Replace Alibaba resource for Ubuntu 18.04 Apt-get update

- String "bionic" is used for  Ubuntu 18.04  
- Replace "bionic" with "xenial" for Ubuntu 16.04   
* lsb_release -c  to check the code of Ubuntu version  
> deb http://cn.archive.ubuntu.com/ubuntu/ bionic main restricted  
> deb http://cn.archive.ubuntu.com/ubuntu/ bionic-updates main restricted  
> deb http://cn.archive.ubuntu.com/ubuntu/ bionic universe  
> deb http://cn.archive.ubuntu.com/ubuntu/ bionic-updates universe  
> deb http://cn.archive.ubuntu.com/ubuntu/ bionic multiverse  
> deb http://cn.archive.ubuntu.com/ubuntu/ bionic-updates multiverse  
> deb http://cn.archive.ubuntu.com/ubuntu/ bionic-backports main restricted universe multiverse  
> deb http://security.ubuntu.com/ubuntu bionic-security main restricted  
> deb http://security.ubuntu.com/ubuntu bionic-security universe  
> deb http://security.ubuntu.com/ubuntu bionic-security multiverse  

