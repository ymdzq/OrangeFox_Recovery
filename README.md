**OrangeFox Recovery Project (OFRP)**
https://wiki.orangefox.tech/

You can find a compiling guide [here](https://wiki.orangefox.tech/en/dev) and [here](http://forum.xda-developers.com/showthread.php?t=1943625 "Guide").

自用橙狐源码，主要区别是：  
1.更新比原版慢  
2.在原版较新版本的代码基础上，合并部分[skkk开源twrp](https://github.com/sekaiacg/twrp_recovery)修改、功能  

这个仓库没有补全中文翻译文本，所以还是橙狐原来那个惨不忍睹的翻译，  
我是不想哪天橙狐更新了文本，多一个地方要改，反正我提的翻译pr这几年了橙狐也都是无视，  
所以我翻译文本都是习惯放在设备树里，编译的时候直接覆盖的同名文件  
[简体中文翻译xml文件](https://github.com/ymdzq/OFRP-device_xiaomi_mondrian/blob/fox_12.1-a14/recovery/root/twres/languages/zh_CN.xml)  
[繁体中文翻译xml文件](https://github.com/ymdzq/OFRP-device_xiaomi_mondrian/blob/fox_12.1-a14/recovery/root/twres/languages/zn_TW.xml)  

我2年前根据最上面橙狐写的那个guide，写的本地编译安卓10(安卓11)分支橙狐方法：  
[橙狐源码编译方法](https://github.com/ymdzq/OFRP-device_xiaomi_bomb/blob/fox_12.1/%E8%AF%B4%E6%98%8E/1%E5%A6%82%E4%BD%95%E4%BD%BF%E7%94%A8.txt)  
[后续更新橙狐源码方法](https://github.com/ymdzq/OFRP-device_xiaomi_bomb/blob/fox_12.1/%E8%AF%B4%E6%98%8E/3%E6%9B%B4%E6%96%B0%E6%BA%90%E7%A0%81.txt)  
至今没更新，已过时，仅供参考，建议以最上面那个英文guide为准  

反正我自己平时linux系统本地用的，最后就简化成了两个脚本了  
[更新橙狐源码脚本](https://github.com/ymdzq/scripts/blob/main/fox-update)  
[橙狐编译脚本](https://github.com/ymdzq/scripts/blob/main/build_fox.sh)  

为什么搞这个仓库：  
1.我自用的[橙狐云编译器](https://github.com/ymdzq/OrangeFox-Action-Builder)仓库，里面我的修改都是根据这个仓库的commits  
2.云编译器由于是先拉取橙狐官方源码，然后打补丁，所以版本理论上是大于等于这个仓库的，但是如果我的补丁与橙狐更新的代码冲突了，云编译就会失败  
3.方便拿去与官方橙狐仓库对比，这样每次橙狐更新之后，直接cheery-pick就可以完成代码更新，修复云编译失败问题  
4.我对这个仓库的commits用git命令生成补丁，保存在[自用脚本、补丁](https://github.com/ymdzq/scripts)仓库里，供上述云编译器使用
