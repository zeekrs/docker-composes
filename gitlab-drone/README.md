# GitLab/Drone

---

本仓库包含一个docker-compose.yml文件和.env文件 

端口映射以及配置信息可在.env文件中修改  

###### GitLab 
- `GITLAB_HOSTNAME`  GitLab域名  
- `GITLAB_PORT` GitLab 映射端口  
- `GITLAB_SSL_PORT` GitLab ssl映射端口  
- `GITLAB_SSH_PORT` GitLab ssh映射端口  
- `GITLAB_SSH_HOST` GitLab ssh域名  
- `GITLAB_DIR` GitLab 数据存储目录  


###### Drone


- `DRONE_HOST_NAME` Drone域名
- `DRONE_GITLAB_CLIENT_ID` GitLab 配置 application 中获取
- `DRONE_GITLAB_CLIENT_SECRET` Gitlab 配置 application 中获取
- `DRONE_RPC_SECRET` Drone server 和 runner 交互的秘钥  可以随机生成一个
- `DRONE_SERVER_PROTO` Drone server 和 runner 传输协议  `http` | `https`
- `DRONE_PORT` Drone 映射端口
- `DRONE_SSL_PORT` Drone ssl 映射端口
- `DRONE_DATA_DIR` Drone 数据存储目录
- `DRONE_ADMIN_USERNAME` Drone 的管理员用户名 需为 GitLab 中用户名一致

- `DRONE_RUNNER_CAPACITY` Drone Runner 运行时并发的管道数量
- `DRONE_RUNNER_PORT` Drone Runner 映射端口




### 参考

- [GitLab Document](https://docs.gitlab.com/ee/install/docker.html)

- [Drone Document](https://docs.drone.io/server/provider/gitlab/)
