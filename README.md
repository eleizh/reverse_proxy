# reverse_proxy

通常的反向代理配置

+ / 对应前端
+ /api/v1 对应后端
+ 仅测试反向代理可以使用python -m SimpleHTTPServer 18000


### 编辑

+ nginx实际上可以不安装什么插件
+ 但安装了通常是匹配/etc/nginx下的.conf文件
+ 在这些目录之外的，需要:set syntax=nginx即可


