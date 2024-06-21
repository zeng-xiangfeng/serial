# serial
获取传感器数据
//sudo gedit /etc/udev/rules.d/70-ttyACM.rules     在/etc/udev/rules.d目录下创建70-ttyACM.rules文件
//在文件中添加一下内容，如：KERNEL=="ttyACM*", OWNER="root", GROUP="root", MODE="0666" 。   保存，重启系统即可获取权限


//下面2个是暂时打开串口权限，每次重启电脑都需要操作一遍
//sudo chmod 666 /dev/tty  先打开串口权限
// 若上面sudo chmod 666 /dev/tty 不行，则sudo su 进入root模式


// Gas.msg文件中用float32编译可以通过，但是用double却不行
