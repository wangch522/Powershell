1. cd到~/.ssh生成ssh-key
     ```
        cd ~/.ssh
        ssh-keygen -t rsa -C "youremail@address.com" -f id_rsa_second
    ```

2. 将新的ssh public key 添加到内部的gitlab仓库
   
3. 在~/.ssh 目录下创建config文件，用于配置私钥对应服务器，内容：
   ```
    Host gitlab.xxx.com ##可以随意命名      
    HostName gitlab.xxx.com   
    User git    
    Port 22   
    IdentityFile ~/.ssh/id_rsa_second
   ```
4. 克隆仓库即可
   ```
    git clone git@gitlab.xxx.com/xx.git
   ```

:::warning注意
git根据配置文件的user.email来获取git账号显示author信息
对于多账号用户一定要将user.email改为相应的email（second@mail.com)
:::
