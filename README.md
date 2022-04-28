# Pan

个人简易网盘。

https://pan.paulplayer.com/



基于Webd+nginx+ssl搭建的个人简易网盘。

```shell
# ssl证书获取

certbot certonly -d paulplayer.com,pan.paulplayer.com,www.paulplayer.com 
```



```sh
# nginx 配置

cp ./nginx.conf /etc/nginx/sites-available/Webd
cd /etc/nginx/sites-enabled/
ln -s ../site-available/Webd ./Webd
```



```shell
# webd 配置
cp ./webd /user/bin/webd
cp ./webd.conf /etc/webd.conf
```



