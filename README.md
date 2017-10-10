Apple Opensource
------

可编译的苹果开源基础库，需要使用 [Additional SDK](https://github.com/longv2go/iPhoneOS_Additional_SDK)。

# 变更

## libmalloc

### Build Settings

* 设置 lto 为 no，开启 lto 会导致无法源码调试，具体原因不清楚，猜测 lto 导致 debug 信息丢失。
* 去掉 order file。
* 添加自定义宏 PRIVATE。
* 关闭 bitcode。