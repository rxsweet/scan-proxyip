# 使用大佬的扫描IP(scan-proxy.yml)
https://github.com/exball/sing-box-config

1.actions使用Scan Proxy：
去掉actions中的actions/checkout@v4使用的token那一行。
去掉actions中的upload-kv代码再运行。


2.如果resolver.exbal.my.id等ip信息查询站不能用了，可使用下面方法
ip信息查询
https://github.com/rxsweet/ip-resolver
可将代码库中的ip-resolver.js部署到workers,部署几次，
将查询网站地址替换到文件proxyip.ts代码中的ip.resolver1.workers.dev下面的if处，如：resolver.exbal.my.id
