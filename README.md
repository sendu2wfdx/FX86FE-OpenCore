#   FX86FE OpenCore0.5.5
    ——Support Device: FX86FE(I7-8750H)
    
    华硕飞行堡垒6（FX86FE）基于OpenCore0.5.5的黑苹果引导文件
    支持原生NVRAM（网卡建议更换为DW1820A）95%完美
# ****-注：需解锁CFG后食用！！！
#   万一出现问题重刷BIOS即可
#   -解CFG锁方法：
    经过查BIOS文件得，
    CFG Lock的偏移量为0x5C2.
    （这个值适用于302至306版本BIOS）
    
    1.下载Shell文件，
    
    2.放到U盘EFI文件夹，
    
    3.给Shell.efi添加引导(推荐使用BOOTICE)
    
    4.开机按ESC，选择Shell
    
    5.输入:‘setup_var_3 0x5C2 0x0’按回车即可
    （若要开启，同理把0x0改为0x1即可）
    
    6.输入‘reboot’按回车重启

#   -使用方法：
    1.将OC，BOOT两个文件夹放在EPS分区的EFI文件夹中
    给BOOT文件夹中的BOOTX64.efi添加引导
    （推荐使用BOOTIECE，或在BIOS中添加）
    
    2.重启，F2进入BIOS，按F7进入高级选项，
    关闭安全启动 secure boot
    （有能力重装系统的可将SATA模式改为AHCI，即可识别固态硬盘）
    其余选项无需操作
    （包括但不限于VT-D，FastBoot，我已经在OC里做好相应屏蔽）
    F10，回车保存即可
    
    3.开机按ESC，
        选择OC引导。
    
    4.Enjoy it.

#   -支持：
    MacOS 10.13-10.15
#   -Bug：
    1.键盘灯快捷键调节（V2版本快捷键有反应，但是无法调节。后期AsusSMC作者可能会支持）
    2.HDMI（此机型HDMI接口直连独显，尝试过在10.13给独显打webdriver，无果，遂放弃）
#   -正常的：
    核显UHD630 2G显存
    原生NVRAM支持（得益于OpenCore 0.5.5）
    USB定制
    睡眠唤醒完美(快捷键，盒盖，系统睡眠均正常，且支持电源小憩)
    原生电源管理（X86加载正常，即节能四项）
    触摸板手势（从QiuChenly的Clover移植而来）
    部分Fn快捷键
    声卡ALC235正常，外放，内置麦克风，3.5接口均正常
    SideCar，接力，隔空投送（网卡更换为DW1820A）
