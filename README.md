#   FX86FE OpenCore0.5.5
    ——Support Device: FX86FE(I7-8750H)
    华硕飞行堡垒6（FX86FE）基于OpenCore0.5.5的黑苹果引导文件，支持原生NVRAM（网卡建议更换为DW1820A），95%完美。
# ****-注：需解锁CFG后食用！！！****
#   解CFG锁方法：
    查BIOS文件得，CFG Lock的偏移量为0x5C2.（适用于305，306版本BIOS，其他版本可升级至上述版本BIOS，或自行查找偏移值。由于BIOS版本不对应或者指令输错产生的问题概不负责）
    进Shell（Shell文件已上传，放到U盘EFI文件夹，添加引导。可在BIOS高级选项，BOOT里添加），输入:‘setup_var_3 0x5C2 0x0’按回车即可（若要开启，把0x0改为0x1即可）
    输入‘reboot’按回车重启
#   -支持：
    MacOS 10.13
    MacOS 10.14
    MacOS 10.15
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
    部分Fn快捷键（只有键盘灯快捷键暂时不可用，后期AsusSMC作者可能会修复）
    声卡ALC235正常，外放，内置麦克风，3.5接口均正常
    SideCar，接力，隔空投送（网卡更换为DW1820A）



