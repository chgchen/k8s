# k8s

push-images.sh 脚本文件
imagepath.txt 镜像列表文件
.travis.yaml 自动构建文件

push-images.sh脚本内容如下，主要从国外镜像仓库pull镜像，打tag，并push到阿里云或dockerhub.
imagepath.txt主要包含国内无法拉取的镜像列表，注意必须为完整镜像路径和名称
.travis.yaml文件主要监控github仓库的代码变动，当有代码变动时比如imagepath.txt写入新的镜像列表时将触发tarvis的自动构建
