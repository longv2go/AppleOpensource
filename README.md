Apple Opensource
------

可编译的苹果开源基础库，以下所有的库都需要配置 [Additional SDK](https://github.com/longv2go/iPhoneOS_Additional_SDK)。


# libmalloc

## 变更

### Build Settings

* 设置 lto 为 no，开启 lto 会导致无法源码调试，具体原因不清楚，猜测 lto 导致 debug 信息丢失。
* 去掉 order file。
* 添加自定义宏 PRIVATE。
* 关闭 bitcode。

## 调试

libmalloc_stress_test

# libdispatch

## 变更

### Build Settings

TODO:

## 调试

TODO:

## 可编译 Targets

* libdispatch introspection
* libdispatch dyld stub 

# objc4

## 变更
* 去掉 bitcode
* 去掉 -lCrashReporterClient

## 调试
TODO: