# VMware 16 安装 CentOS 7.9 详细图文教程

~~~
说明：如果是centos7.9以下，最好选择vmware16以下的版本进行安装
~~~



# 1. 创建虚拟机

1. 新建虚拟机

![img](https://img-blog.csdnimg.cn/img_convert/30f3d517c29a7b7e07a41d19eb509c82.png)

1. 选自定义(高级)，下一步

![img](https://img-blog.csdnimg.cn/img_convert/f0b2702150089cc135a86128513825f6.png)

1. 下一步

![img](https://img-blog.csdnimg.cn/img_convert/19b7005bb35d239607e07e9f54384cfd.png)

1. 选稍后安装操作系统，下一步

![img](https://img-blog.csdnimg.cn/img_convert/6c1a2a4a872a7b1eb923dcf253206191.png)

1. 选Linux，并选择版本CentOS 7 64位，下一步

![img](https://img-blog.csdnimg.cn/img_convert/735e9f09a01bba14ee550f85e0daa31c.png)

1. 指定虚拟机名称，并修改存放虚拟机的位置，下一步

![img](https://img-blog.csdnimg.cn/img_convert/7d33dcd0a2c0f60e108ac2b5bbb5d99f.png)

1. 根据你的电脑配置，选择处理器数量和内核数量（虚拟机总核心数不能超过主机核心数），下一步

![img](https://img-blog.csdnimg.cn/img_convert/6c7aa4467c75a077a77570e5af49419f.png)

1. 根据电脑配置选择虚拟内存，下一步

![img](https://img-blog.csdnimg.cn/img_convert/2753b4b11b0249001bbd1c58165976cb.png)

1. 网络类型建议选择NAT，下一步

![img](https://img-blog.csdnimg.cn/img_convert/48693a54e6685da1e507edf044b6d2f0.png)

1. scsi控制器和磁盘类型都选系统推荐选项，下一步

![img](https://img-blog.csdnimg.cn/img_convert/9853274724889547720e997e65fc2961.png)

![img](https://img-blog.csdnimg.cn/img_convert/82742958f96cd1993b34c8c448e53f4a.png)

1. 选创建新虚拟磁盘，下一步

![img](https://img-blog.csdnimg.cn/img_convert/ba9d44b5e91b91f25c59fac034f4df75.png)

1. 修改最大磁盘大小，再选中将虚拟磁盘储存为单个文件，下一步

![img](https://img-blog.csdnimg.cn/img_convert/1754deddab0b00b3188cca1d33f4f8ad.png)

1. 指定.vmdk的位置，然后点击下一步，之后选择完成

![img](https://img-blog.csdnimg.cn/img_convert/3e14f8a8cd81ae8474aa94756bfe1c02.png)

1. 点击自定义硬件，配置处理器虚拟化

![img](https://img-blog.csdnimg.cn/img_convert/88cb3eff1e1fc4dad053b71b5d675000.png)

![img](https://img-blog.csdnimg.cn/img_convert/ffba0c4c3c46d84f1accc53a939af067.png)

1. 再选择CD/DVD选项，再点击使用ISO映像文件将之前下载的centos7.9的.iso文件选中即可，然后点击确定

![img](https://img-blog.csdnimg.cn/img_convert/c0a196d00bbaefd6ecd72a1d2c028135.png)

1. 关闭声卡启动时连接

![img](https://img-blog.csdnimg.cn/img_convert/1384863673002218be8aff1dd33e73e9.png)

1. 虚拟机创建完成

![img](https://img-blog.csdnimg.cn/img_convert/86a0fc98b381cafe3a12a56ba04b726c.png)

# 2. 安装 CentOS 7.9

1. 开启虚拟机，选择Install CentOS 7

![img](https://img-blog.csdnimg.cn/img_convert/e1f46c37b10292953b6f1de0108dfe9e.png)

1. 选择语言，添加中文和英文

![img](https://img-blog.csdnimg.cn/img_convert/4381fe38357044a3ccd2008b97d51161.png)

![img](https://img-blog.csdnimg.cn/img_convert/d7909e8e7654fcafa0109207e249df55.png)

![img](https://img-blog.csdnimg.cn/img_convert/1857636a365d7796358055eca012bf30.png)

![img](https://img-blog.csdnimg.cn/img_convert/88fe9426bb98afdde670dcb1c98f4521.png)

![img](https://img-blog.csdnimg.cn/img_convert/3c566f5f51cd0d45d69c6c650ff21b2e.png)

![img](https://img-blog.csdnimg.cn/img_convert/ec65472983405afb0af3ee48457f324f.png)

![img](https://img-blog.csdnimg.cn/img_convert/564c356c321c7a6ea771fa175acb7e64.png)

![img](https://img-blog.csdnimg.cn/img_convert/5d962b238fc3815a620a7c53af050a22.png)

1. 对磁盘进行分区，点击安装位置和我要配置分区，点完成

![img](https://img-blog.csdnimg.cn/img_convert/c4ef66a034fbfa0bb186bfcff4892156.png)

1. 点击 “+” 首先给 /boot 分区 200MB ，再给swap分区分配空间，其大小与内存大小相同，最后将剩下的存储空间都给 / 根分区

![img](https://img-blog.csdnimg.cn/img_convert/d6c52bd508c4cc36e5034c0976031dde.png)

![img](https://img-blog.csdnimg.cn/img_convert/fe014887691bf609d43e92f450de49a7.png)

![img](https://img-blog.csdnimg.cn/img_convert/ae254f2bf2478509823cf4bb545e8276.png)

![img](https://img-blog.csdnimg.cn/img_convert/c58ed85cb64d713db646a366a502c96d.png)

![img](https://img-blog.csdnimg.cn/img_convert/9413f7e0b636c1633bdbba2d89843618.png)

1. 点 “接受更改”

![img](https://img-blog.csdnimg.cn/img_convert/ddfa5bba1c351ec6ae49f8fe156c4ce1.png)

1. 配置网络和主机名

![img](https://img-blog.csdnimg.cn/img_convert/0cd6420634d935e7cf1139df159f5059.png)

![img](https://img-blog.csdnimg.cn/img_convert/c71d241bbd2b431672955ad74d7d62da.png)

![img](https://img-blog.csdnimg.cn/img_convert/d6ff591ffeea65325ad8859ddbbbc97a.png)

![img](https://img-blog.csdnimg.cn/img_convert/fc008ae106c46aed2bb3a1f93da7c67a.png)

1. 点击开始安装

![img](https://img-blog.csdnimg.cn/img_convert/c3be650b17e3953d7b4e43faed2767bd.png)

1. 设置ROOT密码

![img](https://img-blog.csdnimg.cn/img_convert/36b3949ac5188e6e0b2549ec143e3f4e.png)

![img](https://img-blog.csdnimg.cn/img_convert/e821affd9cd612c90fad72f883817345.png)

1. 等待安装完成重启

![img](https://img-blog.csdnimg.cn/img_convert/0c3cc84cb747fe7188ebb2812c12dfbf.png)