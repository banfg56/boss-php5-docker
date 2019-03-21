
# BOSS docker 配置文件

## 注意事项
1. 日志以及缓存目录要配置可写权限
2. 数据库账号、数据初始化请自己配置
3. 请修改 MYSQL_ROOT_PASSWORD 中对应密码 mysql root 密码
4. 请求数据库中的连接地址为mariadb

## 如何运行 
直接在根目录运行 docker-compose up -d

## 目录结构
```sh
.
├── README.md
├── conf
│   ├── nginx
│   │   ├── Dockerfile
│   │   ├── crm3.conf
│   │   └── nginx.conf
│   └── php.ini
├── data-mysql
├── data-www
│   └── www
│       └── index.php
├── docker-compose.yml
└── logs
    └── nginx
```

## 参考文档
* [docker CE安装](https://docs.docker.com/install/)
* [docker 容器](https://docs.docker.com/get-started/part2/)
* [docker 服务](https://docs.docker.com/get-started/part3/)
* [docker compose参考](https://docs.docker.com/compose/reference/overview/)
* [PHP-FPM Docker Image](https://github.com/nanoninja/php-fpm)
* [docker-nginx-php-mysql](https://github.com/nanoninja/docker-nginx-php-mysql)

