## libstdc-.6.0.9

Help people download the libstdc-6.0.9 library file.

真机路径：
/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS12.0.sdk/usr/lib
模拟器路径：
/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/SDKs/iPhoneSimulator12.0.sdk/usr/lib
替换完成后在模拟器iOS10.0以上运行会出现一个错误：
Reason: no suitable image found.  Did find:
/usr/lib/libstdc++.6.dylib: mach-o, but not built for iOS simulator

这里还需要拷贝旧Xcode中的/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/Library/CoreSimulator/Profiles/Runtimes/iOS.simruntime/Contents/Resources/RuntimeRoot/usr/lib/libstdc++.6.0.9.dylib并改名为libstdc++.6.dylib后粘贴到新Xcode同样的位置。（注意在/Profiles/Runtimes/iOS.simruntime这里时需要右键显示包内容）。
