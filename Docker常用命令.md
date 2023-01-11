# Docker常用命令速查

## Docker引擎的启停命令

* **systemctl start docker**：启动docker
* **systemctl restart docker**：重启docker
* **systemctl status docke**r：查看docker状态
* **systemctl stop docker**：停止docker
* **systemctl enable docker**：开启开机自启动docker
* **systemctl disable docker**：关闭开机自启动docker

## 镜像命令

* **docker images**   查看本地所有镜像资源信息。携带-q选项后，仅显示本地所有镜像的
  imageID。
* **docker search** 从docker hub上查看指定名称的镜像。
* **docker pull**      将指定的镜像从docker hub拉取到本地。
* **docker rmi**  删除指定的本地镜像。一次可以删除多个。
* **docker save**    将一个镜像导出为一个tar文件。
* **docker load**      将一个tar文件导入为一个镜像。

## Dockers容器

**doker run**         启动和运行容器

--name=“容器名称”：为容器指定一个名称
-i：以交互模式运行容器，一般与-t同时使用
-t：为容器分配一个伪终端
-d：以守护进程方式运行容器
-h：指定容器的主机
-e：指定容器启动所需要的环境，例如连接密码
-p(小写)：指定端口映射 主机端口:容器端口

**exit** 退出并停止容器

**Ctrl + P + Q**退出不停止容器

**docker ps**     查看容器进程
-a：列出所有容器，包含当前正在运行的与曾经运行过的
-l：列出最新创建的容器，无论其是否正在运行
-n 数字：列表最新创建的指定个数的容器
-q：仅显示容器ID，要与前面的选项同时使用

**docker attach**     使用容器进程进入容器（为创建新的容器）**docker exec**         新建进程并进入容器

**docker start** [容器名|容器ID] 启动容器

**docker restart** [容器名|容器ID] 重启容器

**docker stop** [容器名|容器ID] 优雅停止容器：当前容器正在被其它进程访问，则在访问结束后再停止

**docker kill** [容器名|容器ID] 强制停止容器：容器当前是否被其它进程访问都直接停止

**docker rm** 删除容器

**docker cp**     命令可以完成容器与宿主机中文件/目录的相互复制

## 数据卷

**docker run –it –v /宿主机目录绝对路径:/容器内目录绝对路径 镜像**        创建读写数据卷

**docker run–it –v /宿主机目录绝对路径:/容器内目录绝对路径:ro 镜像**     创建只读数据卷

## dockerfile

- FROM
  构建镜像基于哪个镜像

- MAINTAINER
  镜像维护者姓名或邮箱地址

- RUN
  构建镜像时运行的指令

- CMD
  运行容器时执行的shell环境
- VOLUME
  指定容器挂载点到宿主机自动生成的目录或其他容器

- USER
  为RUN、CMD、和 ENTRYPOINT 执行命令指定运行用户

- WORKDIR
  为 RUN、CMD、ENTRYPOINT、COPY 和 ADD 设置工作目录，就是切换目录

- HEALTHCHECH
  健康检查

- ARG
  构建时指定的一些参数

- EXPOSE
  声明容器的服务端口（仅仅是声明）

- ENV
  设置容器环境变量

- ADD
  拷贝文件或目录到容器中，如果是URL或压缩包便会自动下载或自动解压

- COPY
  拷贝文件或目录到容器中，跟ADD类似，但不具备自动下载或解压的功能

- ENTRYPOINT
  运行容器时执行的shell命令