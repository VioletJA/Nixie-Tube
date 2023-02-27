## 辉光管时钟
年显示：<br>
![image](https://github.com/VioletJA/Nixie-Tube/blob/main/img/IMG_20230227_104334.jpg width="100px")
时分显示：<br>
![image](https://github.com/VioletJA/Nixie-Tube/blob/main/img/IMG_20230227_104306.jpg width="100px")

### 硬件部分
采用低成本方法，自己画了控制电路，网上买了一个5v-170v的升压模块。<br><br>
如果想要自己做可以到立创开源平台上找一找，有很多升压的电路原理图<br><br>
硬件采用一节3.7v锂电池供电<br><br>

俯视图：<br>
![image](https://github.com/VioletJA/Nixie-Tube/blob/main/img/IMG_20230227_103618.jpg width="100px")
正视图：<br>
![image](https://github.com/VioletJA/Nixie-Tube/blob/main/img/IMG_20230227_103645.jpg width="100px")

### 软件部分
软件使用stm32控制的，库是用stm32cubeMX生成的HAL库<br><br>
软件主要是利用了一个按键控制显示切换时分显示、年显示、分秒显示的循环。<br><br>
软件本打算利用低功耗模式，实现超长时间待机，但是在画硬件电路时太赶了，忘记加MOS管控制DS3231的电源和升压模块的电源的开断了。<br><br>
具体说明放在CSDN了
