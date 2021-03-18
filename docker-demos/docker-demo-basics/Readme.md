# Docker 基础

### 常用命令

#### Docker Build 

```bash
$ docker build -t my-app:latest .
```

```bash
$ docker build -f path/to/Dockefile -t my-app:latest .
```

### Docker Run 

```bash
$ docker run --rm --name my-server -p 80:80 my-nginx:latest
```


```bash
$ docker run -d -p 80:80 docker/getting-started
```

```bash
$ docker run -it -v {absolute/path/to/file}:{path/in/container} ImageNmae:Tag /bin/bash
```


```bash 
$ docke run -it -v ~/workspace/docker-run/config.json:/1.json ubuntu /bin/bash
```

> 一些参数的解释

| 参数 | 解释 |
|:---:|:---:|
| -d | 让容器在后台运行 |
| -p | 端口映射，宿主机端口:容器内端口 | 
| -v | 挂载宿主机的一个目录，宿主机目录:容器内目录 |
| --name | 指定容器的名称 |
| --rm | 设置该选项，容器在退出时就能够自动清理容器内部的文件系统 |


