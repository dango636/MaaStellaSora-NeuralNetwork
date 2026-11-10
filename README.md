# MaaStellaSora NeuralNetwork 插件（停止维护）

本仓库停止维护并归档，保留历史源码、安装器及 PR 讨论。

神经网络爬塔、模型接入和实机数据采集已转入 [MaaStellaSora](https://github.com/MaaStellaSora/MaaStellaSora) 的原生开发分支，目前正在实测和合并准备。状态空间、训练器与实机研究资料维护在 [StellaSora-Tower-Research](https://github.com/dango636/StellaSora-Tower-Research)。

以下内容为历史插件的使用说明。

MaaStellaSora 项目额外开发的神经网络数值模型插件。

- `maa_value_plugin/`：可编辑源码、模型和相关数据。
- `NeuralNetwork.cmd`：Windows 自解压安装包。
- `build_installer.py`：从 `maa_value_plugin/` 重新生成安装包。

## 训练与研究资料

潜能与音符状态空间、规则数据、实机分析、训练器源码及初始权重维护在 [StellaSora-Tower-Research](https://github.com/dango636/StellaSora-Tower-Research)。

规范化实机总数据见研究仓库的 [Releases](https://github.com/dango636/StellaSora-Tower-Research/releases/tag/real-game-data)。

## 安装

将 `NeuralNetwork.cmd` 放到 `MFAAvalonia.exe` 所在目录，并确保该目录下有官方 Maa 安装包提供的 `python/python.exe`，然后双击运行。

## 修改后重新打包

在本机安装 Python 3 后，在仓库根目录运行：

```bash
python3 build_installer.py
```

公开版本的 `maa_value_plugin/upload_settings.json` 不包含上传令牌。需要使用数据上传功能时，请在本地配置令牌，不要提交到仓库。

## 许可

第三方许可和来源说明见 `maa_value_plugin/licenses.json` 与 `maa_value_plugin/critic/vendor/SOURCE.json`。
