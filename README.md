 基于 `0.24.1` 打包脚本，能够将bundle 分为 coreFramework bundle 和 businsess bundle

## Install

```
将reacNAtive node_module 替换为此node_module
```
## running
```
$ react-native bundle \
  --entry-file ReactComponents/index.ios.js \
  --platform ios \
  --dev true \
  --bundle-output "$DEST/main.jsbundle" \
  --assets-dest "$DEST"\
  --bundleType 'b' // a 全部的bundle文件，c coreFramework b businsess 
```

Options, 参数参考react-native命令，增加了参数：

*  --busindessModuleFile 业务逻辑层代码的root目录
