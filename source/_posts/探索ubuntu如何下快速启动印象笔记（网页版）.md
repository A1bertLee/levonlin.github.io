title: 探索ubuntu如何下快速启动印象笔记（网页版）
date: 2015-05-27 20:38:46
tags: [ubuntu,linux,印象笔记]
categories: 小探索
---
作为一个日渐变成印象笔记重度用户的人，在ubuntu下没有其客户端简直就是对我的折磨。虽然有网页版，但是每次要打开浏览器再去点书签总让人觉得蛋疼且低效（至于chrome应用商店里那个evernote应用我就不得不吐槽了，本质上也就是个网页版的书签啊，还只是国际版的，要不要这么敷衍。。。）。有鉴于此，我便开始了寻找快速启动方法的折腾：

## 不了了之：将链接放到桌面
这是最直接的方法，直接把书签拖到桌面或者建个指向其url的.desktop文件，.desktop文件配置如下：

```
[Desktop Entry]
Encoding=UTF-8
Name=印象笔记网页版
Comment=印象笔记网页版
Type=Application 
Terminal=false 
URL=https://app.yinxiang.com/Home.action
Icon=图标路径
Categories=Application;
```

![加上图标之后已经貌似native应用了有木有](http://ww4.sinaimg.cn/large/85ad0d9cgw1esj6k8b6yjj206a03jglk.jpg)

本来这样就可以结束了，但既然要快速那我们就快速到底，而上述做法美中不足的是这个连接是无法放到启动器上的，想要在桌面被盖住时使用，你还得切回桌面去点那个图标，那还不如使用浏览器书签呢。于是接下来我自然就想编个应用程序了，于是没怎么想就开始了造轮子，但是拎着就能带走的东西，哪里还用得着轮子？就算造出来也还是会跳转到浏览器，让它在启动栏上停留更是画蛇添足。

所以，结果就是浪费时间买教训，也给诸君看了个笑话，最后不了了之。

## 目前解决方案：固定标签页
在操作系统上解决这个问题我已然是无能为力了，所以还是回到浏览器上来，浏览器本身就能快速启动，只要在启动时让印象笔记（网页版）自动启动就可以了。设为主页怕会手贱关掉，所以就用了固定标签页的手段。事实证明这是个不错的曲线救国方案，反正作为重度用户，笔记也会一直开着，降低点浏览器启动速度还是很值得的。
