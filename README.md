# docker_k8s

k8s 安装时，会去google下载镜像。导致安装会卡住很长时间，镜像也下载不下来。

所以先将运行 k8s 运行所需的镜像编译到 docker hub 中

安装k8s 步骤

  1. 安装docker
	2. 安装 kubeadm,kubelet,kubectl
	3. kubeadm 安装 master节点
		3.1	拉取国外镜像太慢，所以需先下载好镜像
		3.2 在/etc/kubernetes/manifests 下有所需镜像的名称版本	
