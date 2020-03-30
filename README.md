# 7559-i7
7559黑苹果，i7-6700HQ 16G 128G + 1T GTX960M 4G +英特尔高清显卡530 ALC256 BIOS1.2.8
 当前存在的问题：  
  1.启动过程中外接音箱爆音，解决办法：开机后再插音箱。  
  2.外接显示屏需要开机再插，否则出现黑屏。  
  3.WiFi无法使用，这个通病，需要更换无线网卡。  
整个安装过程参考江南小虫虫的教程：https://github.com/fengwenhua/dell-7559-hackintosh  
CSDN地址：https://blog.csdn.net/A807296772/article/details/102488864  
         https://www.tonymacx86.com/threads/guide-dell-inspiron-15-7559-skylake.260876/  
此处记录个人需要注意的（也是我走过的很多弯路）  
一、每次升级理论上更新最新CLOVER然后直接更新即可，现在为macOS10.15.4,试用CLOVER为5107（BOOTX64.efi替换EFI/BOOT文件夹中的同名文件。
CLOVERX64.efi替换EFI/CLOVER文件夹中的同名文件。）  
二、出现黑屏或者启动时候需要拔电池，拔掉所有外设等问题：  
  BIOS设置：
  - 恢复BIOS默认设置
  - AHCI mode 选择 SATA(AHCI)
  - 关闭 VT for direct I/O
  - 关闭 Advanced Battery Charging
  - 关闭 Secure boot
  - 关闭 SupportAssist System Resolution
  - 关闭 Firmware TPM
  Press F12 on boot screen and under other options disable Pheriperial Device Setting (OPROM Setting)  
三、修复爆音后重启禁行标志：  
  此处需要特别注意，我到现在没总结出来原因，可能为修复失败、重建缓存失败、没有解锁权限。  
 
