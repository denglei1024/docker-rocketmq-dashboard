# RocketMQ Dashboard 部署

这个项目提供了在 Docker 环境中一键部署 RocketMQ 和 Dashboard 的 Docker Compose 配置。

## 快速开始

1. 克隆此仓库到您的环境中

```bash
git clone git@github.com:denglei1024/docker-rocketmq-dashboard.git
cd docker-rocketmq-dashboard
```

2、修改 conf/broker.conf 配置

3、使用 docker-compose up 命令启动容器
```bash
rocketmq docker-compose -p rocketmql_project up -d
```
4、部署完成后，可以通过以下地址访问 RocketMQ Dashboard：
http://localhost:8080
项目结构
- config/: 包含 RocketMQ 的配置文件
  - broker.conf: Broker 配置文件
- data/: 数据持久化目录
  - broker/: Broker 数据和日志
  - namesrv/: Namesrv 数据和日志
 
![image](https://github.com/denglei1024/docker-rocketmq-dashboard/assets/16712298/6381ad11-2a18-4302-877a-f947bfa0fbb4)
