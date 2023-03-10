## 项目介绍
本项目为react native 新架构demo,只有android端代码。
在运行前先下载react native的环境。
## 文件说明
- [newAcrh](./newAcrh) 项目主程序
- [RTNCalculator](./RTNCalculator/) 新架构模块
- [RTNCenteredText](./RTNCenteredText/) 新架构组件

## 运行
1. cd newAcrh
2. 运行 npm install 或 npm update  下载 node_modules
3. yarn add ../RTNCalculator  添加模块
4. yarn add ../RTNCenteredText 添加模块
5. yarn android 或 yarn react-native run-android  运行android项目

## 其它说明
新架构模块里面的代码每次更新都需要通过 yarn add 重新添加。因为每次yarn add都会把模块代码复制到node_modules里面。
新架构需要通过Codegen代码生成器自动生成代码。
```
cd android
./gradlew generateCodegenArtifactsFromSchema
```
直接调用yarn android也自动生成代码。




