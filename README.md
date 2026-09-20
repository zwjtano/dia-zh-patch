# Dia 浏览器汉化补丁｜macOS 简体中文 · Dia Chinese Patch

为 **Dia 浏览器**提供简体中文界面汉化的非官方补丁，覆盖菜单、设置、聊天与技能界面。应用于已安装的 Dia，**不包含浏览器本体**。

**[下载 R7 汉化补丁](https://github.com/zwjtano/dia-zh-patch/raw/refs/heads/main/Dia-原位汉化补丁-R7-截图修正.zip)** · [安装方法](#安装方法) · [还原方法](#还原方法) · [反馈问题](https://github.com/zwjtano/dia-zh-patch/issues)

> **适用版本：Dia 1.49.1（87398），macOS / Apple Silicon。实验版，尚有未翻译内容，登录、钥匙串和通行密钥兼容性未完整验证。**

## 安装方法

1. 下载上方 ZIP，解压整个文件夹，保留其中所有文件。
2. 正常退出 Dia。
3. 双击 **安装汉化补丁.command**，等待安装完成。从原来的 Dia 图标启动。

无需输入“安装”确认文字。安装器自动检查版本和原始资源，创建完整应用备份后应用补丁；版本不匹配时停止。

需要本机 **Python 3、Apple 命令行开发工具**以及可写的应用安装目录。补丁在本地编译汉化模块；不是无需依赖的独立安装程序。可双击 `检查版本.command` 单独检查版本。

## 汉化范围

| 界面 | 覆盖内容 |
| --- | --- |
| 顶部菜单与标签页 | 菜单项、标签组、标签页操作等 |
| 设置 | 常见设置页面、部分二级弹窗和说明 |
| 技能、Tools、Formats | 界面名称、按钮与说明；实际执行的提示词和命令保持原文 |
| 聊天与扩展 | 部分界面提示及浏览器内的扩展相关界面 |

仍有部分聊天提示等遗漏，第三方扩展自己的页面不保证中文。用户输入和技能提示词不会为了汉化而改写。

## 还原方法

退出 Dia，双击 **还原原版.command**。

安装器将完整原版备份在 `/Applications/.Dia-zh-patch-backup/Dia.app`，还原时校验文件和签名。请勿手动删除该备份。若 Dia 已更新或被其他工具修改，自动还原会停止，避免覆盖新版本。

应用备份不等于浏览器资料备份。补丁不会主动清空正式浏览资料或修改 Dock 配置。

## 兼容性与当前限制

- 仅适配 **Dia 1.49.1（87398）/ Apple Silicon**，不支持其他版本或 Intel Mac。
- 深度汉化需要本地重新签名、移除官方专属权限，并启用该应用加载汉化模块所需的库验证例外。
- 登录、钥匙串、通行密钥兼容性尚未完整验证，不能将本项目视为稳定发行版。
- 已完成模块检查、静态校验和短时启动验证；这些检查不代表全部账号功能通过测试。
- Dia 更新可能覆盖补丁，新版本需要重新适配。

## 常见问题

**这是中文浏览器安装包吗？** 不是。这是现有 Dia 的汉化补丁，需要先安装匹配版本的官方 Dia。

**为什么技能提示词还是英文？** 本项目只汉化界面，保留技能实际执行的提示词和命令，避免改变行为。

**安装时提示版本不匹配怎么办？** 停止安装，等待匹配版本的补丁，不要跳过校验。

**如何反馈未汉化页面或闪退？** 在 Issues 中提供 Dia 版本、macOS 版本和复现步骤。截图请遮挡邮箱、聊天内容及其他个人资料。

## English

An unofficial Simplified Chinese localization patch for the Dia browser on macOS Apple Silicon. Supports **Dia 1.49.1 (87398) only**. Includes Chinese UI translations for menus, settings, chat and skill interfaces. Requires Python 3 and Apple command-line developer tools. The archive contains the patch and its source files, not the browser. Experimental: some strings remain untranslated, and account / Keychain / passkey compatibility is not fully verified.

本项目与 Dia 开发团队无隶属关系，Dia 名称和相关商标归其各自权利人所有。
