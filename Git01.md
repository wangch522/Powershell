# Git 3 个库

工作区  -  写代码
缓存区  -  临时存储， 未提交
本地库 - 历史版本

##1、 工作区 - git add ->缓存区 - git commit -> 本地库

3.6 Git 和代码托管中心 ->帮助维护远程库
    局域网： GitLab  服务器
    外网： 
        1. Github
        2. 码云

3.7 本地库和远程库交互
    1. 团队内部协作
    2. 团队外部协作

4. Git初始化本地库


4.2 # 设置签名
    用户名:
    # Email地址： 
    作用： 区分不同开发人员的身份
    辨析： 这里设置的签名和登入远程库的账号、密码没有任何关系
    命令
        项目级别/仓库级别： 仅在本项目和仓库生效
            git config user.name 
            git config user.email:
        系统用户级别： 登入当前操作系统用户的范围
            git config --global user.name
            git config --global user.email

    级别优先级
        就近原则：项目级别优先于系统用户级别， 二者都有时，采用项目级别签名
        如果只有系统级别签名， 以系统用户级别签名
        二者都没有不允许  
        ***这是加粗体***

        

1. New SSHkey
2. `$ ssh-keygen -t rsa -b 4096 -C "wangch_522@126.com"`
3. `git remote add **alisa name** [ssh url]`
*    这h是另外一个
*      还是另外一个
    * 这我咋知道呢
    * 