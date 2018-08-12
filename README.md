# -
docker的使用 
启动docker容器 systemctl start docker   将docker设为开机启动 systemctl enable docker 
停止docker容器 systemctl stop(restart) docker
查看docker容器的所有镜像 docker images
删除docker容器镜像 docker rmi “容器id”
查看运行中的docker容器 docker ps 
docker ps -a  所有容器包括不运行的

启动一个容器 docker run -d(指定在后台启动) =p（映射端口） 容器名：版本
docker run -d -p 8888:8080 tomcat:latest
docker run -d --name mytomcat tomcat:latest
停止docker容器 docker stop 容器id

移除容器 docker rm  容器id
