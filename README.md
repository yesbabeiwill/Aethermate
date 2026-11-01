# 以太同行 / Aethermate

在最终幻想 XIV 游戏内连接自定义模型 API 的聊天插件，支持流式回复、停止生成、重新生成和本地聊天记录。

适用于国服 XIVLauncherCN / Dalamud API 15。

## 获取插件

在游戏中打开 `/xlsettings`，进入“实验性”的“自定义插件仓库”，添加并启用：

```text
https://raw.githubusercontent.com/yesbabeiwill/Aethermate/main/repo.json
```

保存后打开 `/xlplugins`，搜索“以太同行”并安装。后续使用插件安装器检查和安装更新。

以前手动加载过的用户，先停用旧开发插件并移除旧 DLL 路径，再通过插件库安装。保留 `pluginConfigs/Aethermate` 配置目录即可继续使用本机设置和记录。

## 模型聊天

1. 输入 `/aethermate` 打开窗口。
2. 填写兼容 Chat Completions 的 API 根地址和自己的 Key，例如 `https://example.com/v1`。
3. 拉取模型列表，或直接填写模型 ID，保存后即可聊天。

聊天窗口支持发送、停止和重新生成。“新对话”会清除当前会话的本地聊天记录。Key 使用当前 Windows 用户加密保存；模型服务的可用性与调用规则由使用者选择的 API 提供方决定。
