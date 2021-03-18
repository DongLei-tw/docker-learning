# 基础镜像
FROM python:3.8-alpine

# 复制操作
COPY . /app

# 在构建镜像过程中执行命令，能修改镜像内部的文件
RUN echo "print('Hello Docker!')" > /app/app.py

# 在容器启动的时候执行此命令
ENTRYPOINT python /app/app.py

# 容器启动时执行，而不是镜像构建时执行
# CMD python /app/app.py