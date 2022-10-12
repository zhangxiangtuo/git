### GitHub推送不成功问题

1.新建SSH keys链接:  

去git设置找到  SSH and GPG keys, 然后新建SSH key

2.具体的key的生成

去c盘用户目录下我的是(C:\Users\DELL\.ssh), 右键打开Git Bash Here输入命令

```git
ssh-keygen -t rsa -C "自己的git账号"
```

3.然后他会提示你输入密码这里密码是看不到的

```Enter passphrase (empty for no passphrase):

Enter passphrase (empty for no passphrase):
Enter same passphrase again:

```

这里会让你输入两遍,然后会生成具体的  "id_rsa.pub"文件,用记事本打开复制内容就是SSH的key了,然后建立新的SSH连接github就可以正常推送(push了)
