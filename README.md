# To devs
If you wanna use these yaml file. Please check you environment. Based on the situation which the writer used. Please check the environment before.

## System Environment
CentOS 7.5 x86_64

## Docker Environment

### Docker Install
Based on the link[https://docs.docker.com/install/linux/docker-ce/centos/#upgrade-docker-ce-1]</br>
First step:
```
sudo yum install -y yum-utils \
  device-mapper-persistent-data \
  lvm2
```

Second step
```
sudo yum-config-manager \
    --add-repo \
    https://download.docker.com/linux/centos/docker-ce.repo
```

Third step:
```
sudo yum-config-manager --enable docker-ce-edge
```

Forth step:
```
sudo yum install docker-ce -y
```
if you were in china and can not download the docker-ce, please run the command below:
```
sudo sed -i 's+download.docker.com+mirrors.tuna.tsinghua.edu.cn/docker-ce+' /etc/yum.repos.d/docker-ce.repo
```

### Docker-compose Install
Based on The link[https://docs.docker.com/compose/install/#install-compose]</br>

```
sudo curl -L "https://github.com/docker/compose/releases/download/1.23.1/docker-compose-$(uname -s)-$(uname -m)" \
    -o /usr/local/bin/docker-compose
```

```
sudo chmod +x /usr/local/bin/docker-compose
```
