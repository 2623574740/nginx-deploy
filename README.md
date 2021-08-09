# nginx部署包

## 声明

本文档仅针对CentOS 7进行nginx服务部署，请确认好后再使用。如果在使用时出现任何问题，欢迎大家在issue上提交问题。

## 操作步骤

1. 请将压缩包解压后，将nginx-1.20.1，pcre-8.00，deploy.sh上传至服务器

2. 切换到root用户

   ```shell
   su root
   ```

3. 修改deploy.sh执行权限

   ```shell
   chmod 700 deploy.sh
   ```

4. 执行deploy.sh

   ```shell
   ./deploy.sh
   ```

5. 执行完成后，请到对应目录配置nginx

   ```shell
   vim /usr/local/nginx/conf/nginx.conf
   ```

6. 启动nginx

   ```shell
   ./usr/local/nginx/sbin/nginx
   ```

大功告成！请注意，我没有在文档上写如何配置防火墙，如果你的本机无法访问服务器上的nginx，请将80端口打开，并重启防火墙，至于防火墙如何开端口和重启，就请开发者们自己上网查查吧，祝你开发顺利。

## 联系我

电子邮箱：shujarry@gmail.com

