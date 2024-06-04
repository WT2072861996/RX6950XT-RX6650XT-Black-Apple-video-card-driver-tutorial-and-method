## macOS原生不支持RX6650XT和RX6950XT，通过SSDT仿冒的方式可以驱动

1.win下获取显卡PCI地址方法：

计算机管理-设备管理器-显示适配器-显卡右键-属性-位置路径

![截屏2024-05-30 01 03 47](https://github.com/WT2072861996/RX6950XT-RX6650XT-Black-Apple-video-card-driver-tutorial-and-method/assets/113539098/d2fbf966-fbd1-42e3-b4a7-ea337365f44a)

图片里面画红线的位置就是显卡路径 记住这个路径

![截屏2024-05-30 01 04 06](https://github.com/WT2072861996/RX6950XT-RX6650XT-Black-Apple-video-card-driver-tutorial-and-method/assets/113539098/bc46a1b5-ff55-4ea3-aa12-b65974e7e42c)

2.然后在 Mac下打开MaciASL.app软件,用MaciASL.app打开我上面分享的SSDT文件修改如下位置

![截屏2024-05-30 00 59 21](https://github.com/WT2072861996/RX6950XT-RX6650XT-Black-Apple-video-card-driver-tutorial-and-method/assets/113539098/9b54dcf8-d520-453f-b044-79369b01cfad)

画红线的位置修改成你在Windows下找到的显卡路径，然后把修改好的SSDT文件放进你的OpenCore或者Clover引导的ACPI文件夹里面然后启动它
