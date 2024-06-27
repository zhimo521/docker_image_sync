# Github Action使用文档
https://docs.github.com/zh

# 密钥变量设置
- 本仓库-Settings-Secrets and variables-Actions
- 添加Secrets
- 使用方式${{ secrets.密钥名称 }}

# 同步镜像
- 支持amd64架构镜像 -> 华为云容器镜像服务
- 支持arm64架构镜像 -> 华为云容器镜像服务
- 支持amd64架构镜像 -> 阿里云容器镜像服务
- 支持arm64架构镜像 -> 阿里云容器镜像服务

> 阿里云可以将命名空间设置为公开
> 华为云需要每个镜像单独设置为公开
