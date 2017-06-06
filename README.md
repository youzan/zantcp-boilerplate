# Youzan Zan TCP Boilerplate

- 该boilerplate项目是配合 [zan-installer](https://packagist.org/packages/youzan/zan-installer) 使用的，直接克隆下来后无法直接运行。

## 如何使用
1. 安装swoole扩展，编译参数：
`./configure --enable-async-httpclient  --enable-sockets --enable-async-redis  --enable-openssl`

2. 安装 Composer [Getting Started](https://getcomposer.org/doc/00-intro.md)
```bash
curl -sS https://getcomposer.org/installer | php
```

3. 在根目录下执行 `composer update`

4. 配置php.ini
```ini
zanphp.RUN_MODE = test
zanphp.DEBUG = true
```

5. 启动tcp server `php bin/nova`

6. 启动zan http server访问tcp server