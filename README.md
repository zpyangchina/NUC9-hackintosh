## For NUC9i5/i7/i9QNX、NUC9VXQNX MacOS



## Computer Configuration

- NUC9i9qnx(理论上NUC9全系通用，包括幽灵峡谷、石英峡谷)
- 无线网卡: 板载 Intel ax200网卡、Apple拆机卡 943602cs
- 有线网卡: I219、I210
- 内存: 金士顿 3200MHz 16GBx2 DDR4
- 显卡: 惠普 6600xt 拆机卡
- 硬盘: 西数 SN750 2T
- 声卡: 板载 ALC256

## bios settings

- Advanced

  Video -> Primary Display > IGFX (默认auto即可，若想双显卡输出可设置为IGFX)

  Video -> Internal graphics > enable

  Storage -> SATA Mode Selection > AHCI

- Security (可不进行如下设置)

  Intel Platform Trust Technology > Unchecked

  Intel Software Guard Extension (SGX) > Disabled

  Thunderbold Security Level > Legacy mode

- Boot

  Secure Boot > Disabled

  Boot Priority -> Fast Boot > Unchecked

  Boot Priority -> USB -> Checked

## hardware

- [x] CPU正常睿频
- [x] 核心显卡已驱动，支持HDMI/Tyepc-c显示输出，配合bios设置可双显卡输出
- [x]  独立显卡HP 6600xt
- [x]  USB接口已经定制，所有USB接口均可正常使用
- [x]  声卡驱动正常，前后3.5音频输出皆正常
- [x]  休眠/唤醒正常
- [x]  板载Intel无线网卡
- [x]  蓝牙正常
- [x] 双网口驱动正常，默认屏蔽I210网卡(部分机器启动I210网卡会卡引导)
- [ ] 读卡器无SD卡测试，但读卡器走的USB3.2hub，理论上可以使用
- [ ]  雷电三载系统信息中能看到，但是无雷电硬件测试
