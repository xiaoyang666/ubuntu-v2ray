ubuntu-v2ray科学上网
之前需要用命令行下载国外的package，ubuntu用的人比较少，基本都是win下的，为了能在Ubuntu下科学上网，我SSR，SSS，VPS都买了，还是推荐买VPS,有几篇博文也是比较坑，我基本都踩过了。其中对于小白来说，config.json的配置是,是比较困难的，所以特地写一篇作为小白的我的踩坑日记，在linux上用的SSR和SS最近封IP的比较多，此处不便推荐我用的是VPS服务器

1.VPS服务器
   拥有一个 VPS 是必需的，选择合适的VPS套餐，VPS套餐来自：搬瓦工（Bandwagon Host）这里就不在说了，这个地方一般没有问题，而且可以在TB买，在win能完    全配置好就ok找到win下v2ray的文件夹，导出config.json 文件牢记，或者配置截图都ok

2.Ubuntu部署
   用Ubuntu16.04安装使用V2ray，其他平台类似，详情参考官方教程
   $ bash <(curl -L -s https://install.direct/go.sh)
   （此处如果需要root，需要输入命令sudo -i）

   此脚本会自动安装以下文件：
   /usr/bin/v2ray/v2ray：V2Ray 程序；
   /usr/bin/v2ray/v2ctl：V2Ray 工具；
   /etc/v2ray/config.json：配置文件；
   /usr/bin/v2ray/geoip.dat：IP 数据文件
   /usr/bin/v2ray/geosite.dat：域名数据文件

   此脚本会配置自动运行脚本。

   脚本运行完成后，你需要：
   编辑 /etc/v2ray/config.json 文件来配置你需要的代理方式；

   $sudo gedit /etc/v2ray/config.json

    config.json 的模板文件

   运行 service v2ray start 来启动 V2Ray 进程；
    之后可以使用 service v2ray start|stop|status|reload|restart|force-reload 控制 V2Ray 的运行。



