以Unraid为例

安装`User Scripts`插件

将`dll ca.7z`解压后移动到unraid中如我存放的路径/mnt/user/appdata/ca/

在`User Scripts`插件中新建名为`emby`的脚本,并设置为`At First Array Start Only`
粘贴以下内容:
 ```
 !/bin/bash
 cp -rf /mnt/user/appdata/ca/default.conf /etc/nginx/conf.d/default.conf
 nginx -s reload
 ```

劫持`mb3admin.com`至unraid后运行
