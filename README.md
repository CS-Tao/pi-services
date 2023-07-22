# pi-services

树莓派 Docker 服务集群

[![Docker Image CI](https://github.com/CS-Tao/pi-services/workflows/Docker%20Compose%20CI/badge.svg)](https://github.com/CS-Tao/pi-services/actions)

## 项目依赖

- docker
- docker-compose

## 已配置服务

![services_graph.svg](https://home.cs-tao.cc/pi-services/services_graph.svg)

## 部署方法

1. 克隆本仓库

    ```bash
    git clone https://github.com/CS-Tao/pi-services.git
    ```

1. 添加环境变量文件`.env`到项目根目录，复制`.env.ci`内容到`.env`文件中，并修改其中各项环境变量的值

1. 拉取镜像

    ```bash
    docker-compose pull
    ```

1. 启动容器组

    ```bash
    docker-compose up -d --no-build
    ```
