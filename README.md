add_sample_metadata 是一个采样插件

dissect_query 是一个解析query的插件

下载filebeat的源码
在beats/libbeat/processors目录下进行插件开发
在你需要使用的的平台打包 打包命令：go build -buildmode=plugin
启动filebeat filebeat ---plugin ./myplugin.so,多个插件用多个--plugin
插件必须在beats/libbeat/processors目录下编译打包，打包和平台有关，mac下打的包，在linux上不能使用
