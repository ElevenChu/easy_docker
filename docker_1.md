## 什么是Docker
：解决了运行环境和配置问题软件容器，方便做持续集成并有助于整体发布的容器虚拟化技术

### 虚拟机的缺点

1.资源占用多

2.冗余步骤多

3.启动慢

### 比较Docker与传统虚拟化
![image](https://user-images.githubusercontent.com/57619422/133393584-086ab448-7c9d-45cc-8e7c-58cafeaba27e.png)



### Docker的架构图
Images->镜像；Registry->仓库

![` 54T0P Y(T B8YQ%E VLU](https://user-images.githubusercontent.com/57619422/133225377-90bdad1b-6618-491e-8c74-7d6152dfc770.png)



### Docker的基本组成
- 1.镜像
![image](https://user-images.githubusercontent.com/57619422/133226240-745ce404-6297-4ff3-93b4-845d2d435f8d.png)

- 2.容器
- ![image](https://user-images.githubusercontent.com/57619422/133226718-1fd8dca7-7e56-488d-9407-e9c971f4fe7d.png)

- 3.仓库
![image](https://user-images.githubusercontent.com/57619422/133227306-3684c6d6-e4d8-4a79-b094-8ea84e0c7351.png)


## Docker镜像加载原理

![image](https://user-images.githubusercontent.com/57619422/133535071-f19ffe49-d582-4c2e-aa6c-9828c6af311c.png)


- 联合文件系统UnionFS
![image](https://user-images.githubusercontent.com/57619422/133535538-d4a1bd93-374f-467a-a4f8-68fbd87ac875.png)

## Docker容器数据卷
![image](https://user-images.githubusercontent.com/57619422/133538834-b3685fdc-dfbb-47f3-b663-4f8cab8f107d.png)

数据卷类似于Redis中持久化的RDB和AOF文件

作用：

 1.容器持久化
      
 2.容器间继承+共享数据

### DockerFile

什么是 Dockerfile？

： Dockerfile 是一个用来构建镜像的文本文件，文本内容包含了一条条构建镜像所需的指令和说明。

- 写容器卷的主流步骤
- 
![image](https://user-images.githubusercontent.com/57619422/133571504-b9c8f787-7cdf-4d12-ba36-39a9b6f7f5be.png)

- 关系
![image](https://user-images.githubusercontent.com/57619422/133573745-87d4d7be-838e-421c-8e08-2b51383cb65d.png)



- ENTRYPOINT 和 CMD的区别

:![image](https://user-images.githubusercontent.com/57619422/133579003-4644c007-9eca-431f-a0fa-78e1a597c70c.png )

- 自定义一个镜像（例子centOS）\
![image](https://user-images.githubusercontent.com/57619422/133585030-cac92666-5ac0-4508-b4f7-eab0ce1634cd.png)

 


