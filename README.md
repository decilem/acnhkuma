# 大气层新手简陋教程（偏动森向）作者：DECILEM
## 所有步骤请以Homebrew网站为准
[点此进入网站](https://switch.homebrew.guide/)   只不过网站有点复杂，我帮着缕一缕
### 第1步（准备SD卡）
[一键制卡网站](http://www.sdsetup.com/)
进入一键制卡网站以后选择Recommended Defaults
下面的一堆选项里面记得勾选上JKSV，忘记勾选也没关系，可以另外再下载，JKSV是把动森存档导出的关键工具
<img src="https://github.com/decilem/acnhkuma/raw/main/pic/makingSD.png" width="800">

完成以后拖到最后选择download your ZIP就好了

解压以后的ZIP应该包含两个文件夹，一个payload一个sd，payload可以 先不管，只用sd文件夹里的内容就行了

>在准备把东西拷入sd卡之前，记得把sd卡格式化一下，选择FAT32格式，把sd卡插入switch，开机一下，然后就可以关机把卡拔出来了，这时候卡里会自动生成一个Nintendo文件夹，保留这个文件夹

然后把刚才sd文件夹里的所有文件拷入sd卡根目录，你的sd卡应该看起来像下图这样
<img src="https://github.com/decilem/acnhkuma/raw/main/pic/SDcard.png" width="800">

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
后面还有很多可以折腾的东西，到这就可以折腾动森了。

不过在进入之前，强烈建议备份一下系统，以备不时之需。备份系统看下面的链接：

[备份NAND](https://switch.homebrew.guide/hacking/caffeine/safetyprecautions)

NAND备份上面这个链接其实写的已经很清楚了，我觉得我也不会说的更好。总之就是这么几步：
1. 备份boot0boot1

2. 把卡拔出来把backup文件夹备份到电脑，然后删除sd卡上的backup文件夹

3. 再插入卡，进去按说明备份RAW GPP

4. 再把卡拔出来，重复步骤2，把两个backup文件夹分别保存

5. 再次插卡，进入Hekate界面，按说明备份key

6. 拔卡，把prod.key这个文件保存到电脑

7. 结束，这样你有三个文件需要保存（第一次的backup文件夹，第二次的backup文件夹，和prod.key）


### 第4步
[进入破解系统](https://switch.homebrew.guide/hacking/caffeine/aftersetup)

从Hekate界面进入破解系统的话需要选Launch -> CFW(sysMMC) 然后就进入到了CFW真实破解系统，从这里按一下平常打开相册的按钮就进入到自定义app界面，对于初学者来说，这里能用到的目前只有JSKV，其他不用管。打开JKSV，选择那个Switch机子图标（Device Saves）进入，里面应该可以看到动森了，这时候按Y导出全部，就把机子的存档导出来了，存档的名字叫 “Device Saves - XXXXXX”，这个就是你原机的存档了，在SD卡的JKSV文件里可以看到这个存档，这个是你原装的存档，记住多备份几遍在电脑上，以备不时之需。
## JKSV和NHSE
关于JKSV和NHSE的用法我分开写到wiki里了
[点击进入wiki](https://github.com/decilem/acnhkuma/wiki)


## 其他解释
> [这个网站](https://www.reddit.com/r/SwitchHaxing/comments/gip0jb/>current_methods_and_exploits_beginner_faq_3_its/)有更详细的名词解释

OFW： Original Firmware 也就是原装的系统

CFW： Custom Firmware 也就所谓的（Modified）破解系统

NAND: Switch机子的内置内存

emuNAND： 这个是为了玩盗版游戏而把机子NAND完整copy到sd卡上的应该虚拟系统。**注意**！这个系统非常危险，应该保持全程断网。

## 更新大气层
去大气层的[官方github](https://github.com/Atmosphere-NX/Atmosphere/releases)下载最新的文件,下载完以后把这些文件覆盖到你现在的sd卡就好了，非常简单。不过这次的0.16.1的更新需要同时把Hekate也更新到最新，参考下面同时把Hekate也更新

## 更新Hekate
去Hekate的[官方github](https://github.com/CTCaer/hekate/releases)把最新的release下载完成（大概就叫`hekate_ctcaer_5.5.1_Nyx_0.9.7.zip`的这个文件），解压完以后有两个文件，一个BootLoader文件夹覆盖到sd卡，另外一个叫`hekate_ctcaer_5.5.1.bin`的文件需要复制到你的注入器里面，atmosphere那个文件夹下面，里面有一个文件叫`payload.bin`，把这个文件删除，把你新复制进来的那个文件改名成`payload.bin`。

然后大功告成，就可以按正常步骤进去系统了
## 安全第一，预防为主

没有人可以说清楚老任说怎么ban机的，理论上只要上了破解道路就要做好随时被ban的准备。

当然根据网友们的猜测，有些方法可以减少风险，举几个例子：

1. 使用完JKSV导入存档以后，直接关机，然后正常开机在正版系统里开动森会减少很多风险。

2. 关闭动森的那个备份存档功能

3. 关闭机子自动更新软件以及下面那个收集信息还是什么来着的选项。

4. 别玩盗版（等你想玩的时候咱们再另外讨论）

## FAQ

