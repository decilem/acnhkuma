# 送给Kuma的破解教程（from DECILEM）
## 所有步骤请以Homebrew网站为准
[点此进入网站](https://switch.homebrew.guide/)   只不过网站有点复杂，我帮着缕一缕
### 第1步（准备SD卡）
[一键制卡网站](http://www.sdsetup.com/)
进入一键制卡网站以后选择Recommended Defaults
下面的一堆选项里面记得勾选上JKSV，忘记勾选也没关系，可以另外再下载，JKSV是把动森存档导出的关键工具
![勾选JKSV](https://github.com/decilem/acnhkuma/raw/main/pic/makingSD.png)
<img src="https://github.com/decilem/acnhkuma/raw/main/pic/makingSD.png" width="800">

完成以后拖到最后选择download your ZIP就好了

解压以后的ZIP应该包含两个文件夹，一个payload一个sd，payload可以 先不管，只用sd文件夹里的内容就行了

>在准备把东西拷入sd卡之前，记得把sd卡格式化一下，选择FAT32格式，把sd卡插入switch，开机一下，然后就可以关机把卡拔出来了，这时候卡里会自动生成一个Nintendo文件夹，保留这个文件夹

然后把刚才sd文件夹里的所有文件拷入sd卡根目录，你的sd卡应该看起来像下图这样

[sd卡内容](https://imgur.com/oIQdrVB)

### 第2步
现在sd卡已经准备好了，这时候机子应该是关机状态

1. 插入sd卡

2. 把右手柄拔出来，把注入器插进去，把短接器插入右手柄那个位置

3. 长按注入器上的按键，变成蓝色的灯是大气层专用

4. 关键的一步来了，同时按住音量+和电源键，

5. 注入器会亮蓝色的灯，如果注入器只是闪了一下就灭了，重试步骤4

6. 成功的话，这时候就可以进入一个暗色的界面（Hekate） 

### 第3步
恭喜你，到这里你就已经破解成功了。 从现在开始注入器和短接器都可以拔掉了，下次关机重新开机的时候才用得到。不插注入器按电源键正常开机就是OFW原装系统了。
后面还有很多可以折腾的东西，不过到这就可以折腾动森了。

不过在进入之前，强烈建议备份一下系统，以备不时之需。备份系统看下面的链接：

[备份NAND](https://switch.homebrew.guide/hacking/caffeine/safetyprecautions)

## 其他解释
> [这个网站](https://www.reddit.com/r/SwitchHaxing/comments/gip0jb/>current_methods_and_exploits_beginner_faq_3_its/)有更详细的名词解释

OFW： Original Firmware 也就是原装的系统

CFW： Custom Firmware 也就所谓的（Modified）破解系统

NAND: Switch机子的内置内存

emuNAND： 这个是为了玩盗版游戏而把机子NAND完整copy到sd卡上的应该虚拟系统。**注意**！这个系统非常危险，应该保持全程断网。
