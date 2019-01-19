# 以太坊：Java语言版源码解读准备

欢迎转载，但须指明出处：[https://github.com/chenjw13097/papers](https://github.com/chenjw13097/papers/blob/master/%E5%8C%BA%E5%9D%97%E9%93%BE/%E4%BB%A5%E5%A4%AA%E5%9D%8A%EF%BC%9AJava%E8%AF%AD%E8%A8%80%E7%89%88%E6%BA%90%E7%A0%81%E8%A7%A3%E8%AF%BB%E5%87%86%E5%A4%87/%E4%BB%A5%E5%A4%AA%E5%9D%8A%EF%BC%9AJava%E8%AF%AD%E8%A8%80%E7%89%88%E6%BA%90%E7%A0%81%E8%A7%A3%E8%AF%BB%E5%87%86%E5%A4%87.md)  

### 链接

[https://github.com/ethereum/ethereumj](https://github.com/ethereum/ethereumj)  
此项目名为EthereumJ，是以太坊黄皮书的Java实现。  

### 下载

笔者使用Git克隆了master分支到本地。  
![](./引用/图片1.png)  

### IntelliJ IDEA打开

为了打开源码，需要事先安装[Gradle](../../软件或工具/Gradle环境搭建/Gradle环境搭建.md)和Git，并配置它们的环境变量。  
  
使用IntelliJ IDEA打开./build.gradle。  
![](./引用/图片2.png)  
  
第一次打开比较耗时，会自动下载需要的包，如下代码跳转正常。  
![](./引用/图片3.png)  
  
运行编译和测试也通过。  
![](./引用/图片4.png)  
  
如果读者不习惯Gradle，可以将配置文件.\ethereumj-core\build.gradle转换为POM文件，从而使用Maven构建工具来操作并顺利阅读代码。  
