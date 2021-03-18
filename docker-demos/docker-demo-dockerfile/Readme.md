# Dockerfile 基础

### 基本结构

Dockerfile 一般分为四部分：
* 基础镜像信息
* 维护者信息
* 镜像操作指令
* 容器启动时执行指令


### 常用的镜像操作指令

| 指令 | 解释 |
|:---:|:---:|
| FROM| 指定基础镜像，要在哪个镜像建立，必须作为第一条指令 |
| RUN | 在镜像中要执行的命令 |
| WORKDIR | 指定当前工作目录，相当于 cd命令 |
| EXPOSE | 指定容器要打开的端口 |
| ENV | 定义环境变量 |
| COPY | 复制本地主机（为Dockerfile所在目录的相对路径）的文件到容器中 |
| ENTRYPOINT | 容器启动后执行的命令，每个 Dockerfile 中只能有一个 ENTRYPOINT |

### 运行例子

构建Image:
```bash 
$ docker build -t python-docker .
```

> 猜一下运行的结果会是什么？

验证一下猜想：
```bash 
$ docker run python-docker 
```

