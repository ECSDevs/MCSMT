# MCSMT ( Minecraft Server Manage Tool)
## 运行方式
直接运行源代码   
依赖：requests, flask, watchdog  
扩展插件：wget  
依赖安装方式：  
```bash
pip install requests wget flask watchdog
```
扩展插件可以直接用`extension_downloader.py`安装。  
## 服务端
1. 首先用`config_gen.py`生成服务器配置
2.1. 静态服务端
2.1.1. 直接启动`server.py`,生成引导之后打包传上服务器
2.2. 动态服务端
2.2.1. 直接启动`server_function.py`即可启动便捷式服务器
## 客户端
写一个`Cconfig.json`，像这样：
```json
{
    "requestURL": "http://api.myserver.online/"
}
```
启动`client.py`即可同步
## 工具
### mod downloader
一个mod下载器，需要自己到docs.curseforge.com申请开发者账号。登陆后左侧api-复制token-粘贴进工具即可。
