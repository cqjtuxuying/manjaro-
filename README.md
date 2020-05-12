# 现在还没有解决的问题
1. 当compton这个包更新为picom时，i3bar的透明效果丢失了，已经删除了compton的配置文件，并在.i3/config中添加了
   ```
   i3bar_command i3bar -t
   ```
   结果是只能实现部分透明效果，也就是最右侧的托盘部分，总之很丑，希望有解决方法的人告知下。
2. Spotify无法输入中文，前端时间网易云音乐无法输入中文的问题，通过别人提供的方法重新编译了安装包解决了，Spotify无
   法输入中文的问题截至目前还没有找到比较好的解决方法，希望好心人提供帮助。
3. 搜狗输入法无法输入中文，期间通过如下命令安装搜狗输入法
   ```
   sudo pacman -S fcitx-im             
   sudo pacman -S fcitx-configtool     
   sudo pacman -S fcitx-sogoupinyin
   ```
   安装完之后在.xprofile中添加如下配置文件
   ```
   export LC_ALL=zh_CN.UTF-8
   export GTK_IM_MODULE=fcitx
   export QT_IM_MODULE=fcitx
   export XMODIFIERS="@im=fcitx"
   ```
   然后在图形化工具里启用搜狗输入法，奈何无法输入中文，界面出来了很迷。最后装个谷歌拼音将就着用。
4. Ulauncher会出现透明边框，很丑，碍眼，强迫症受不了;albert配置的快捷键,只能在调出在托盘无法直接显示到桌面，麻烦；
   rofi还可以，但是在命令行调出时可以显示图标，快捷键就不行。结果就是目前没有一款比较完美的launcher可以使用。
