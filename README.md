#### G2呼叫组件PC端源码

##### 简介：
组件基于网易云信提供的G2 SDK与信令SDK进行封装，简化了呼叫流程（包括视频通话呼叫、音频通话呼叫），并提供话单等功能。
用于帮助开发者快速接入G2音视频能力、快速了解G2 SDK使用方式
##### 依赖：
>* G2 SDK 3.7.0
>* IM SDK 8.1.0

##### 集成方式：
VS配置示例（以VS2019为例）
>* 将component目录添加至VS工程（wrapper目录可移除）
>* 将NertcSDK头文件，即nertc_sdk文件夹添加至VS工程
>* 将DLL与lib文件拷贝至自己的运行目录下
>* 在VS工程中配置“附加包含目录”，添加nertc_sdk所在目录
>* 在VS工程中配置“附加库目录”与“附加依赖项”
>* 配置完毕，此时可以使用AvChatComponent类，创建对象、使用音视频2.0功能

完整使用示例，请参见[nim_demo](https://github.com/netease-im/NIM_PC_Demo.git "nim_demo")仓库
组件位于nim_demo仓库：tool_kits\ui_component\g2_kit\component