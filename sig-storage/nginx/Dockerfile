# 使用官方nginx基础镜像
FROM nginx:latest
 
# 将当前目录下的文件复制到容器的/usr/share/nginx/html目录下
COPY . /usr/share/nginx/html
 
# 暴露80端口
EXPOSE 80
 
# 当Docker容器启动时，自动启动nginx服务
CMD ["nginx", "-g", "daemon off;"]

LABEL MAINTAINER=master@zisgood.top BUILDTYPE=Aliyun
