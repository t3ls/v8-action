# Github Action 极简搭建 v8 环境
a simple method to get v8 source code with github action

用法可以看 https://zhuanlan.zhihu.com/p/159646912 的介绍

fork后做了一些改动：
- 添加了编译v8的步骤，可以通过指定`BUILD_DEBUG=true`或者`BUILD_RELEASE=true`来开启编译debug或者release版本
- 添加了在切换到指定commit后打patch的功能，patch的代码要放在`patch.diff`里面，然后把`PATCH_FLAG`改成true
- 优化压缩的命令

基本上就是一键搭建，会下载就行（懒人必备）
