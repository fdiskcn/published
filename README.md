# published

公开仓，只存可以外发的程序包（Release 资产）。源码仍在各私有仓，不这里开源。

Public binaries only. Source stays in private repositories.

## 当前发版

| 软件 | 标签 | 说明 |
| --- | --- | --- |
| JK-Tools | [`jk-tools-v0.0.2.3`](https://github.com/fdiskcn/published/releases/tag/jk-tools-v0.0.2.3) | Windows zip + Linux x86_64 tar.gz，对应私有仓 `fdiskcn/jk-tools` 的 `v0.0.2.3` |

直链（无需登录）：

- [JK-Tools-v0.0.2.3-windows.zip](https://github.com/fdiskcn/published/releases/download/jk-tools-v0.0.2.3/JK-Tools-v0.0.2.3-windows.zip)
- [JK-Tools-v0.0.2.3-linux-x86_64.tar.gz](https://github.com/fdiskcn/published/releases/download/jk-tools-v0.0.2.3/JK-Tools-v0.0.2.3-linux-x86_64.tar.gz)

Windows：解压后运行 `JK-Tools.exe`。Linux（Ubuntu 24.04+ x86_64）：`tar xzf … && cd JK-Tools && ./JK-Tools --smoke`。

## 标签约定

`{product}-v{version}`，例如 `jk-tools-v0.0.2.3`。一个仓可挂多个产品，不要把源码推进来。
