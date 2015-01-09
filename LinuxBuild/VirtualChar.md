## 常用模块命令 ##
1.  lsmod查看系统中加载的所有模块
2.  dmesg查看加载，卸载模块的信息
3.  root权限下insmod 模块名.ko //插入编译好的模块
4.  root权限下rmmod 模块名（可不加后缀）

## Other ##
1.  设备名定为：char_dev
2.  用命令insmod char_dev.o加载
3.  用命令lsmod察看是否成功加载
4.  使用dmesg察看主设备号
5.  使用mknod char_dev c 253 1在/dev目录下创建设备文件
6.  运行Testchardev.c测试
