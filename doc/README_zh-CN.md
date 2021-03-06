# CP Editor

<img src=../assets/icon.ico height="80" width="80">

CP Editor 是一个基于 Qt 的轻量级跨平台代码编辑器，专为算法竞赛设计。

它可以让你刷题/打比赛更加轻松 :grin: 因为它自动化了很多算法竞赛中的流程。

[特性](https://cpeditor.github.io/) | [安装](INSTALL_zh-CN.md) | [使用](MANUAL_zh-CN.md) | [更新日志](CHANGELOG.md) | [贡献指南](CONTRIBUTING_zh-CN.md) | [FAQ](#faq) | [English](../README.md)

---

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/ce0f297f31f74485b0d340949d08d605)](https://www.codacy.com/gh/cpeditor/cpeditor)
[![GitHub All Releases](https://img.shields.io/github/downloads/cpeditor/cpeditor/total?label=downloads%40all)](https://github.com/cpeditor/cpeditor/releases)
[![QQ Group](https://img.shields.io/badge/join-QQ%20chat-success)](https://jq.qq.com/?_wv=1027&k=50eq8yF)
[![Help wanted issues](https://img.shields.io/github/issues/cpeditor/cpeditor/help%20wanted)](https://github.com/cpeditor/cpeditor/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)

|  类型  |                            分支                            |                                                                                            构建                                                                                            |                                                                     下载量                                                                     |
| :----: | :--------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------: |
| alpha  | [master](https://github.com/cpeditor/cpeditor/tree/master) | [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/cpeditor/cpeditor/CI:%20Build%20Test/master)](https://github.com/cpeditor/cpeditor/actions?query=branch%3Amaster) |                                                                       -                                                                        |
|  beta  |   [v6.2](https://github.com/cpeditor/cpeditor/tree/v6.2)   |   [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/cpeditor/cpeditor/CI:%20Build%20Test/v6.2)](https://github.com/cpeditor/cpeditor/actions?query=branch%3Av6.2)   | [![Downloads](https://img.shields.io/github/downloads/cpeditor/cpeditor/6.2.1/total)](https://github.com/cpeditor/cpeditor/releases/tag/6.2.1) |
| stable |   [v6.1](https://github.com/cpeditor/cpeditor/tree/v6.1)   |   [![GitHub Workflow Status](https://img.shields.io/github/workflow/status/cpeditor/cpeditor/CI:%20Build%20Test/v6.1)](https://github.com/cpeditor/cpeditor/actions?query=branch%3Av6.1)   | [![Downloads](https://img.shields.io/github/downloads/cpeditor/cpeditor/6.1.3/total)](https://github.com/cpeditor/cpeditor/releases/tag/6.1.3) |

## 开始使用

- [发行版](https://github.com/cpeditor/cpeditor/releases)
- [安装指南](INSTALL_zh-CN.md)
- [使用说明与提示](MANUAL_zh-CN.md)

## 做出贡献

- [提 issue](https://github.com/cpeditor/cpeditor/issues/new/choose)
- [贡献指南](CONTRIBUTING_zh-CN.md)
- [适合新手解决的 issues](https://github.com/cpeditor/cpeditor/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
- [需要帮助的 issues](https://github.com/cpeditor/cpeditor/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)

## 获取帮助

1. 请首先阅读 [使用指南](MANUAL_zh-CN.md) 和 [FAQ](#faq)，并看看应用菜单和设置中有没有能帮到你的。
2. 如果你要问的问题和 CP Editor 本身不太相关，请尝试通过百度来解决问题（例如：如何安装 Clang Format？这个编译错误是什么意思？）。
3. 在 [Issues](https://github.com/cpeditor/cpeditor/issues) 中搜索，确保你是第一个发现这个问题/提出这个请求的。
4. 在提 issue 时，请务必遵守模板，提供详细的信息，这有助于更快地获得更加令您满意的答复。
5. 如果您要报告 bug / 请求新特性，而非询问如何使用，请提 issue 而非在 QQ 群中提问。

- [提 issue](https://github.com/cpeditor/cpeditor/issues/new/choose)
- [在 QQ 群中提问](https://jq.qq.com/?_wv=1027&k=50eq8yF)

## FAQ

- 我在写 Java，代码不能正常运行。
   - 你的代码使用的类名需要是 `a`，而且不能是 public class。
- 打开程序时提示缺失 DLL。
   - 请下载并安装 [Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads)。
- 如何使整个界面都是深色样式？
   - 只有在 KDE, MacOS 等少数平台上可以使整个界面都是深色样式（CP Editor 会使用系统主题）。在支持的平台上，还可以在命令行中使用 `--style` 选项来设置应用样式。详见 [Qt 文档](https://doc.qt.io/qt-5/qstyle.html#details)。
- 如何从网站上获取样例？
   - 你需要在浏览器上安装 [Competitive Companion](https://github.com/jmerle/competitive-companion) 插件, 然后在打开 CP Editor 的情况下使用它（点击绿色加号）。
- 如何在应用内提交代码到 CF 上?
   - 你需要使用 Competitive Companion 获取 CF 题目的样例，或者在标签页的右键菜单中设置题目地址，然后就可以看到提交按钮了。
- 为什么提交按钮无法点击？
   - 这是因为 CP Editor 不能运行 `cf` 命令。你可以将 CF Tool 加入 PATH，或者在首选项中设置 CF Tool 的路径。
- 提交时让我设置 template，那是什么？
   - 请在命令行中使用 `cf config` 来设置用户名，密码和模板。
- 使用 Competitive Companion 时，提示 invalid payload，那是什么?
   - 一般来说多获取几次样例，重启浏览器和 CP Editor，甚至更换浏览器可以解决这个问题。

License
----

[GNU General Public License Version 3.0](https://github.com/cpeditor/cpeditor/blob/master/LICENSE)
