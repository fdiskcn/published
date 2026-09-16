# published

公开仓，只存可以外发的程序包（GitHub Release 资产）。源码仍在各私有仓。

Public binaries only. Source stays in private repositories.

## 标签约定

`{product}-v{version}`，例如 `jk-tools-v0.0.2.3`。一个仓可挂多个产品；不要把源码或 zip 推进 git。

## JK-Tools

对应私有仓 [`fdiskcn/jk-tools`](https://github.com/fdiskcn/jk-tools) 已打好的便携包。公开发布后会出现：

- 标签 `jk-tools-v0.0.2.3`
- `JK-Tools-v0.0.2.3-windows.zip`
- `JK-Tools-v0.0.2.3-linux-x86_64.tar.gz`

Windows：解压后运行 `JK-Tools.exe`。Linux（Ubuntu 24.04+ x86_64）：`tar xzf … && cd JK-Tools && ./JK-Tools --smoke`。

私有仓已加 `Mirror to published` workflow；跨仓上传需要在 `jk-tools` 仓库 Settings → Secrets 里放一条能写本仓的 `PUBLISHED_TOKEN`，或本机 `gh auth login --with-token` 后手动 `gh release upload`。
