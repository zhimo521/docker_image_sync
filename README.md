# Github Action使用文档
https://docs.github.com/zh

# 密钥变量设置
- 本仓库-Settings-Secrets and variables-Actions
- 添加Secrets
- 使用方式${{ secrets.密钥名称 }}
- 涉及密钥请自行注册对应平台账号获取

# 同步镜像
- 支持amd64架构镜像 -> 华为云容器镜像服务
- 支持arm64架构镜像 -> 华为云容器镜像服务
- 支持amd64架构镜像 -> 阿里云容器镜像服务
- 支持arm64架构镜像 -> 阿里云容器镜像服务
- 支持amd64、arm64等多架构镜像 -> 华为云容器镜像服务
- 支持amd64、arm64等多架构镜像 -> 阿里云容器镜像服务

# images-amd64.txt
用于同步amd64架构镜像，对应工作流配置文件
- docker-sync-amd64-huawei-cloud.yml
- docker-sync-amd64-aliyun-cloud.yml

# images-arm64.txt
用于同步arm64架构镜像，对应工作流配置文件
- docker-sync-arm64-huawei-cloud.yml
- docker-sync-arm64-aliyun-cloud.yml

# images.txt
用于同步多平台架构镜像，对应工作流配置文件
- docker-sync-huawei-cloud.yml
- docker-sync-aliyun-cloud.yml

> 阿里云可以将命名空间设置为公开；
> 华为云需要每个镜像`单独`设置为公开；

# 鸣谢
基于项目[docker_image_pusher](https://github.com/tech-shrimp/docker_image_pusher)改进而来，支持同步多架构、多厂商容器镜像服务仓库。
