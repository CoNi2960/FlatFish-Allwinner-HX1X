# [FlatFish]-DevBoard-Allwinner-HX1X
the lib of project [FlatFish]


本项目基于全志H618，使用成品核心板。底板为2层板设计，方便打样，元件封装尺寸较小，焊接需仔细。

[FlatFish]的正面有一块0.5寸 ssd1306芯片驱动的OLED，通过I2C0连接，反面安装核心板。

有一个注意要点：usb 2.0 母座在设计上出现了一点小瑕疵，四个脚位序号标反了， 在焊接底板的时候，usb母座需要翻过来焊接!!!焊接完毕后，需要确保usb母座的舌片在下方！！！

建议先焊接电源部分比如板上的TPS82130，测量输出电容电压3.3v即为正常，type-C接口输出5v~5.2v即为正常，HDMI +5v in端点5v即为正常，led的电源位于核心板，因此测量无电压为正常。

底板各部分供电测量无误后，可以焊接核心板。刷入img镜像之后测量axp313周边电容均输出正确电压后则正常[这个电压是可以进行配置的，一般有3.3v 1.1v 0.9v]。

连接ch343p串口，等待系统启动成功，然后，就可以利用[FlatFish]去完成你想做的计划了！


This project is based on Allwinner H618 and uses a finished core board. The bottom plate is designed as a 2-layer board, which is convenient for proofing, and the component package size is small, and the soldering needs to be careful.

There is a 0.5-inch SSD1306 chip driven OLED on the front of [FlatFish], which is connected via I2C0 and the core board is mounted on the reverse.

There is a key point to note: the USB 2.0 female connector has a small flaw in the design, the serial number of the four pins is reversed, and the USB female connector needs to be turned over for soldering when soldering the base plate!! After soldering, you need to make sure that the tongue of the USB receptacle is underneath!!

It is recommended to weld the power supply part first, such as the TPS82130 on the board, the measured output capacitor voltage of 3.3v is normal, the output of the type-C interface is 5v~5.2v is normal, HDMI +5v in the endpoint of 5v is normal, and the power supply of the LED is located on the core board, so the measurement of no voltage is normal.

After the power supply measurement of each part of the base plate is correct, the core plate can be welded. After flashing the IMG image, the capacitors around the AXP313 are measured, and the correct voltage is output [this voltage is configurable, generally 3.3V, 1.1V, 0.9V].

Connect the ch343p serial port, wait for the system to boot successfully, and then you can use [FlatFish] to complete the plan you want to do!
