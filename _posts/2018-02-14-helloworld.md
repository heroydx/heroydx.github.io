---
layout:     post
title:      踩坑达人之破马张飞
subtitle:   踩坑达人之博客第一个大坑
date:       2018-02-14
author:     heroydx
header-img: img/post-bg-miui6.jpg
catalog: true
tags:
    - daily
    - 博客维护
---
# 初次搭建博客

初次搭建博客按照**BY**大神的[快速搭建个人博客](http://qiubaiying.top/2017/02/06/%E5%BF%AB%E9%80%9F%E6%90%AD%E5%BB%BA%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2/)基本没有踩坑，这里完全套用了**BY**的模板和一些图片。

# 二次搭建博客

## 评论系统中gitalk的设置

* 首先，如果按照**BY**的经验按步骤走，设置仓库为*用户名.github.io*的话会出现*Error: Not Found.*，我的解决方法是新建一个名为**issue**的仓库，用它专门来产生评论。

* 其次，直接从[**BY**仓库](https://github.com/qiubaiying/qiubaiying.github.io)fork来的需要添加一行*id: 'window.location.pathname'*，否则也会报错。这里在**BY**后续的[为博客添加-Gitalk-评论插件](http://qiubaiying.top/2017/12/19/%E4%B8%BA%E5%8D%9A%E5%AE%A2%E6%B7%BB%E5%8A%A0-Gitalk-%E8%AF%84%E8%AE%BA%E6%8F%92%E4%BB%B6/)中有提及，但是像我这样粗心大意的直接fork难免会出错，这里给大家提醒吧。

![mark](http://p3vekuvea.bkt.clouddn.com/blog/180214/BHl1e536Kf.png?imageslim)

可能是目前*gitalk*的小bug或者是*github*本身对于**issue label**的长度限制，*title*过长会出现*Error: Validation Failed.*。目前我还没有找到合适的解决方法，如果大家谁有好办法可以私信给我。这里先谢过了。

我甚至想过可以直接关闭评论系统，奈何强迫症又要犯了~~

评论系统已经修改好了，只要把**_posts**文件夹中**.md**文件的文件名改短一些就可以了，希望对大家能够有所帮助。

## 自定义域名

* 自定义域名时如果从[阿里云](https://wanwang.aliyun.com/domain/?spm=5176.8006371.1007.dnetcndomain.q1ys4x)上购买**一定记得实名制**，初次搭建博客时没有实名制，一时间焦头烂额。甚至麻烦了**BY**亲自发邮件指导，这里对**BY**的热情和细心表示感谢。同时也因为自己的疏忽给别人造成麻烦而道个歉。

> 根据《中国互联网络域名管理办法》的规定，目前注册 .xin 域名、.cn/.中国/.公司/.网络 等国内域名、.com/.net 国际域名、.top 域名、.xyz/.club/.vip/.shop/.wang/.ren/.site/.我爱你/.集团/.biz/.red/.kim/.pro/.info/.mobi/.ltd/.group/.link/.ink/.在线/.中文网/.网址/.work/.online/ .tech/.fun/.store/.网店/.live/.social/.pub/.video 域名等都要求必须进行实名认证。未完成实名认证的域名会处于 Serverhold 状态，无法正常使用，待实名审核通过后，1-2 个工作日恢复 ok 状态。

* 如果不想使用自定义域名，只需要清空*CNAME*并提交即可。更改*CNAME*文件并上传以后，一定要清空浏览器缓存才会生效。

# 总结

博客至此搭建起来了，具备了评论系统、统计系统、自定义域名。成就感爆棚，希望以后能成为一个高产的博客吧，多和诸位同学交流。这里也祝大家过年好哇！