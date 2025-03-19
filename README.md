**OrangeFox Recovery Project (OFRP)**
https://wiki.orangefox.tech/

You can find a compiling guide [here](https://wiki.orangefox.tech/en/dev) and [here](http://forum.xda-developers.com/showthread.php?t=1943625 "Guide").

自用橙狐源码，主要区别是：  
1.更新比原版慢  
2.在原版较新版本的代码基础上，合并部分[skkk开源twrp](https://github.com/sekaiacg/twrp_recovery)修改、功能  

我自己平时linux系统本地编译橙狐常用的两个脚本  
[更新橙狐源码脚本](https://github.com/ymdzq/scripts/blob/main/fox-update)  
[橙狐编译脚本](https://github.com/ymdzq/scripts/blob/main/build_fox.sh)  

为什么搞这个仓库：  
1.我自用的[橙狐云编译器](https://github.com/ymdzq/OrangeFox-Action-Builder)仓库，里面我的修改都是根据这个仓库的commits  
2.云编译器由于是先拉取橙狐官方源码，然后打补丁，所以版本理论上是大于等于这个仓库的，但是如果我的补丁与橙狐更新的代码冲突了，云编译就会失败  
3.方便拿去与官方橙狐仓库对比，这样每次橙狐更新之后，直接cheery-pick就可以完成代码更新，修复云编译失败问题  
4.我对这个仓库的commits用git命令生成补丁，保存在[自用脚本、补丁](https://github.com/ymdzq/scripts)仓库里，供上述云编译器使用
