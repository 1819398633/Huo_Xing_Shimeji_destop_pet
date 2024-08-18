Shimeji桌宠：霍星-魔角侦探
Shimeji Desktop Pet: Huo Xing - MojoSpy

==== 有关该桌宠 About this Shimeji ====

原作品：魔角侦探

画师：太公小望（钟鸣）

动画修改/图片修改：B站@孤独的小路灯(https://space.bilibili.com/168821367)

软件：Shimeji-ee (http://kilkakon.com/shimeji)

代码维护：Kilkakon

同人作品 非商用

这是以《魔角侦探》中霍星为形象制作的桌宠，十年前的赛博旧物。它由望姐（太公小望）在百度贴吧“魔角侦探吧”首次发布。作为童年白月光形象的桌宠，它给我留下了深刻的印象。
如今原件依赖的JAVA6已逐渐远去，甚至提供桌宠代码的Shimeji制作组也已停止开发。幸好有热心网友至今仍在维护代码，也给了霍星桌宠重生的机会。
我在原件的基础上修改，并增加了一些动画。希望这个桌宠能够继续陪伴喜欢《魔角侦探》和霍星的朋友。

原件资源：魔角侦探官方资源@魔角侦探吧(https://pan.baidu.com/s/1jLEpC#list/path=%2Fsharelink2000836218-174267432978472%2F%E9%AD%94%E8%A7%92%E4%BE%A6%E6%8E%A2%E5%AE%98%E6%96%B9%E8%B5%84%E6%BA%90%40%E9%AD%94%E8%A7%92%E4%BE%A6%E6%8E%A2%E5%90%A7&parentPath=%2Fsharelink2000836218-174267432978472)

资源包里面还有齐乐天、小桃和蓝叉叉团子的桌宠（有谁知道蓝团子的作者么）。这些都是基于JAVA6的版本

（望姐似乎退网了，唯一能搜到的是她22年的时候还在 非人哉。希望她如果知道桌宠修复了会开心~）

==== 注意 ====

本桌宠的简中汉化文件基于使用场景特化了。如果你需要制作自己的桌宠并使用这个汉化文件，请使用language_zh_formal.properties（也会在Kilkakon的下一个版本中加入）。

运行环境要求

1. Windows Vista或更高版本
2. 安装 Java 8

==== 使用方法 ====

1. 下载Huo_Xing_Destop_Pet.zip文件并解压
2. 运行Shimeji-ee.jar文件
3. 在托盘区域会有一个星星图标
4. 点击星星以召唤霍星
5. 右键星星以查看主菜单
6. 右键桌宠以查看该桌宠的菜单
7. 其他请自己探索
8. 如果不需要每次启动显示信息页面，请在主菜单取消选择“启动时总是显示信息栏”
9. 退出：右键星星或桌宠，选择“关闭程序”
10. 卸载：删除解压出的文件夹即可
11. 教程（b站搬运）：https://www.bilibili.com/video/BV1AG4y1T7Ch
12. 常见问题FAQ（b站搬运）：https://www.bilibili.com/video/BV1ke4y1N7Dg
13. Discord 群: https://discord.gg/dcJGAn3

以下是原版的README：

Shimeji-ee: Shimeji English Enhanced

Shimeji-ee is a Windows desktop mascot that freely wanders and plays around the screen.  The mascot is very configurable; its actions are defined through xml and its animations/images can be (painstakingly) customized.  Shimeji was originally created by Yuki Yamada of Group Finity (http://www.group-finity.com/Shimeji/).  This branch of the original Shimeji project not only translates the program/source to English, but adds additional enhancements to Shimeji by Kilkakon and other members of the community.

==== Contents ==== 

1. Homepage
2. Requirements
3. How to Start
4. Basic Configuration
5. Advanced Configuration
6. How to Quit
7. How to Uninstall
8. Source
9. Library
10. Trouble Shooting

==== Homepage ==== 

Homepage: http://kilkakon.com/shimeji

==== Requirements ==== 

1. Windows Vista or higher
2. Java 8

==== How to Start ==== 

Double Click the Shimeji-ee file (Shimeji-ee.jar).

Right click the tray icon for general options.

Right click a Shimeji for options relating to it.

For a tutorial on how to get Shimeji running, watch this video: https://www.youtube.com/watch?v=S7fPCGh5xxo

You can also watch the FAQ if you encounter problems: https://www.youtube.com/watch?v=A1y9C1Vbn6Q

You can also join my Discord group: https://discord.gg/dcJGAn3

==== Basic Configuration ==== 

If you want multiple Shimeji types, you must have multiple image sets.  Basically, you put different folders with the correct Shimeji images under the img directory.

For example, if you want to add, say, a new Batman Shimeji:

1. Create an img/Batman folder.
2. You must have an image set that mimicks the contents of img/Shimeji.  Create and put new versions of shime1.png - shime46.png (with Batman images of course) in the img/Batman folder.  The filenames must be the same as the img/Shimeji files.  Refer to img/Shimeji for the proper character positions.
3. Start Shimeji-ee.  Now Shimeji and Batman will drop.  Right click Batman to perform Batman specific options.  Adding "Call Shimeji" from the tray icon will randomly create add either Shimeji or Batman.

When Shimeji-ee starts, one Shimeji for every image set in the img folder will be created.  If you have too many image sets, a lot of your computer's memory will be used... so be careful.  Shimeji-ee can eat up to 60% of your system's free memory.  

Shimeji-ee will ignore all the image sets that are in the img/unused folder, so you can hide image sets in there.  There is also a tool, Image Set Chooser, that will let you select image sets at run time.  It remembers previous options via the conf/settings.properties file.  Don't choose too many at once.

For more information, read through the configuration files in conf/.  Most options are somewhat complicated, but it's not too hard to limit the total number of Shimeji or to turn off certain behaviors (hint: set frequency to 0.)

==== Advanced Configuration ==== 

All configuration files are located in the in the conf folders.  In general, none of these should need to be touched.

The logging.properties file defines how logging errors is done.
The actions.xml file specifies the different actions Shimeji can do.  When listing images, only include the file name.  More detail on this file will hopefully be added later.
The behaviors.xml file specifies when Shimeji performs each action.  More detail on this file will /hopefully be added later.
The settings.properties file details which Shimeji are active as well as the windows with which they can interact. These settings can be changed using the program itself.

Each type of Shimeji is configured through:

1. An image set.  This is located in img/[NAME].  The image set must contain all image files specified in the actions file. 
2. An actions file.  Unless img/[NAME]/conf/actions.xml or conf/[NAME]/actions.xml exists, conf/actions.xml will be used.
3. A behaviors file.  Unless img/[NAME]/conf/behaviors.xml or conf/[NAME]/behaviors.xml exists, conf/behaviors.xml will be used.

When Shimeji-ee starts, one Shimeji for every image set in the img folder will be created.  If you have too many image sets, a lot of your computer's memory will be used... so be careful.  Shimeji-ee can eat up to 60% of your system's free memory.  

Shimeji-ee will ignore all the image sets that are in the img/unused folder, so you can hide image sets in there.  There is also a tool, Image Set Chooser, that will let you select image sets at run time.  It remembers previous options via the ActiveShimeji file.  Don't choose too many at once.

The Image Set Chooser looks for the shime1.png image.  If it's not found, no image set preview will be shown.  Even if you're not using an image named shime1.png in your image set, you should include one for the Image Set Chooser's sake.

Editing an existing configuration is fairly straightforward.  But writing a brand new configuration file is very time consuming and requires a lot of trial and error.  Hopefully someone will write a guide for it someday, but until then, you'll have to look at the existing conf files to figure it out.  Basically, for every Behavior, there must be a corresponding action.  Actions and Behaviors can be a sequence of other actions or behaviors.

The following actions must be present for the actions.xml to be valid:

ChaseMouse
Fall
Dragged
Thrown

The following behaviors must be present for the behaviors.xml to be valid:

ChaseMouse
Fall
Dragged
Thrown

The icon used for the system tray is img/icon.png

==== How to Quit ==== 

Right-click the tray icon of Shimeji, Select "Dismiss All"

==== How to Uninstall ==== 

Delete the unzipped folder.

==== Source ====

Programmers may feel free to use the source.  The Shimeji-ee source is under the New BSD license.
Follow the zlib/libpng licenses.

==== Library ====

lib / jna.jar and lib / examples.jar of the JNA library.
JNA follows the LGPL.
lib / AbsoluteLayout.jar from Netbeans.

==== Trouble Shooting ====

For a tutorial on how to get Shimeji running, watch this video: https://www.youtube.com/watch?v=S7fPCGh5xxo

You can also watch the FAQ if you encounter problems: https://www.youtube.com/watch?v=A1y9C1Vbn6Q

You can also join my Discord group: https://discord.gg/dcJGAn3

Shimeji-ee takes a LOT of time to start if you have a lot of image sets, so give it some time.  Try moving all but one image set from the img folder to the img/unused folder to see if you have a memory problem.  If Shimeji is running out of memory, try editing Shimeji-ee.bat and change "-Xmx1000m" to a higher number.

If the Shimeji-ee icon appears, but no Shimeji appear:

1. Make sure you have the newest version of Shimeji-ee.
2. Make sure you only have image set folders in your img directory.
3. Make sure you have Java on your system.
4. If you're somewhat computer savvy, you can try running Shimeji-ee from the command line.  Navigate to the Shimeji-ee directory and run this command: "C:\Program Files (x86)\Java\jre6\bin\java" -jar Shimeji-ee.jar
5. Try checking the log (ShimejiLogX.log) for errors.  If you find a bug (which is very likely), post it up on the Shimeji-ee homepage in the issues section.