docker主要分为两部分：container和image
区别就相当于c中的实例和类的区别

image的创建需要根据dockerfile来创建，最好有一种方法能根据image来反向导出dockerfile，从而修改image，可惜没有

常用命令
docker run
根据image 来创建container，参数比较全的命令如下
docker run --gpus all --shm-size 8G -it -v /home/cuizhe/gitrepo:/home/gitrepo phsummerdocker:v1

docker commit
根据container来导出image，适合添加了一些库之后，主要还是不能根据image来反向导出dockerfile，不然就方便了
docker commit <container id> <image id>:<tag>

docker exec
进入现在已有的容器
docker exec <container id>  <ARG>
docker exec -it 75e6ef3ede2d /bin/bash

docker build
根据dockerfile创建image,<ARG>表示模式，代表了dockerfile在哪，如-t就表示是当前目录下的
docker build <ARG> <image id> .
yysy，这个命令基本没用过