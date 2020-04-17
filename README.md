#   FX86FE OpenCore0.5.8
    ——Support Device: FX86FE(I7-8750H)
    华硕飞行堡垒6（FX86FE）基于OpenCore的引导文件，已同步更新至0.5.8（网卡建议更换为DW1820A）
#   注：需解锁CFG后食用！
#   -解CFG锁方法：
    经过查BIOS文件得，CFG Lock的偏移量为0x5C2.（这个值适用于302至306版本BIOS）
    1.进入OC选择Shell，回车
    2.输入:   setup_var_3 0x5C2 0x0   回车
    3.输入:   reboot  回车重启
#   -支持：
    MacOS 10.13-10.15(可以恢复模式联网安装)
#   -Bug：
    1.键盘灯快捷键（等后期AsusSMC作者更新）
    2.HDMI（可通过购买Mac能用的USB转HDMI线解决）
#   -正常的：
    核显UHD630驱动
    原生NVRAM
    睡眠唤醒完美
    原生电源管理
    触摸板手势（从QiuChenly的Clover移植而来）
    Fn快捷键
    声卡ALC235正常，外放，内置麦克风，3.5接口均正常
    SideCar，接力，隔空投送（网卡更换为DW1820A）
#   -交流群：854752511
![](https://github.com/EricCui2333/FX86FE-OpenCore-0.5.5/blob/master/854752511.jpg)
#   -如果觉得好用，请给我打赏支持下
![](https://github.com/EricCui2333/FX86FE-OpenCore-0.5.5/blob/master/打赏.jpg)
