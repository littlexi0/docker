# docker 
## docker安装
```bash
sudo apt update
sudo apt install docker.io
```
## 设置docker镜像源
这里我们直接用阿里云的镜像源，到阿里云控制台搜索镜像，然后点进去就有bash命令
## docker命令
### docker 进程命令
启动docker  
`systemctl start docker`  
关闭docker  
`systemctl stop docker`  
重启docker  
`systemctl restart docker`  
查看docker状态  
`systemctl status docker`  
开机自启动docker  
`systemctl enable docker`
### docker 镜像相关命令
查看镜像：查看本地所有镜像  
`docker images`  
`docker images -q`  
搜索镜像：从网络中查找需要的镜像  
`docker search 镜像名称`  
拉取镜像  
`docker pull 镜像名称`  
删除镜像  
`docker rmi 镜像id # 删除指定本地镜像`  
<code>docker rmi `docker images -q`</code> # 删除所有本地镜像
