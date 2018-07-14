# FairyOpenssl

Openssl编译动态库

## 下载Openssl

[地址](https://github.com/guardianproject/openssl-android)

## 修改

### 修改`AndroidManifest.xml`文件

修改`android:minSdkVersion`

### 修改`default.properties`文件
 
修改 `target `

### 修改jni里面的`Application.mk`

修改`NDK_TOOLCHAIN_VERSION`

### 修改crypto里面的`Android.mk`

增加`LOCAL_LDLIBS += -lz`
 
### 修改ssl里面的`Android.mk`

增加`LOCAL_LDLIBS += -lz`

## 编译

在`jni`目录下执行`ndk-build`.动态库即在libs文件夹下。

![](https://github.com/guxiaonian/FairyOpenssl/blob/master/png/demo.png)