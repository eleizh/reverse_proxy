# reverse_proxy

通常的反向代理配置，应对后端有zuul这类应用级网关做了服务接口聚合的情况

事实上这里再做匹配也很容易，就是多一条urlrewrite的正则配置，具体到这里

+ / 对应前端
+ /api/v1 对应后端
+ 仅测试反向代理可以使用python -m SimpleHTTPServer 8001

另外，最外层应用网关可以负责扛流量，做最外层的路由分流，人肉配置realserver负载并不失为一个较佳的选择

### vim 编辑

+ nginx实际上可以不安装什么插件
+ 但安装了通常是匹配/etc/nginx下的.conf文件
+ 在这些目录之外的，需要:set syntax=nginx即可

