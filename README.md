<p align="center"><img src="./github-header-image.png"></p>
<h2 align="center">linuxdo 增强插件（linuxdo-scripts）</h2>
<p align="center">脚本持续更新，欢迎提出 issues，提交 pr ~</p>

[中文简体](https://github.com/dlzmoe/linuxdo-scripts/blob/main/README.md) | [English](https://github.com/dlzmoe/linuxdo-scripts/blob/main/README_EN.md)

<p align="center">
<img src="https://img.shields.io/github/v/release/dlzmoe/linuxdo-scripts?label=linuxdo%20%E5%A2%9E%E5%BC%BA%E6%8F%92%E4%BB%B6&labelColor=%235D5D5D&color=%23E97435">
<img src="https://img.shields.io/github/last-commit/dlzmoe/linuxdo-scripts">
<img src="https://img.shields.io/github/stars/dlzmoe%2Flinuxdo-scripts?style=flat">
<img src="https://img.shields.io/github/license/dlzmoe/linuxdo-scripts">
</p>

linux.do 增强插件，话题列表显示创建时间，显示楼层数，新标签页打开话题，强制 block（拉黑屏蔽）某人的话题，话题快捷回复（支持自定义），优化签名图显示防止图裂，在话题列表可直接预览详情及评论，功能设置面板导入导出，楼层抽奖，用户自定义标签，只看楼主，自动滚动阅读，支持自定义 css 样式，中英文混排优化，等级信息查询，AI 总结话题功能、智能生成回复，支持 webdav 同步，切换论坛主题皮肤等，功能持续更新，欢迎提出新想法！

[Github 仓库](https://github.com/dlzmoe/linuxdo-scripts) |
[Greasyfork 商店安装](https://greasyfork.org/scripts/501827) |
[Bug 反馈及功能请求](https://github.com/dlzmoe/linuxdo-scripts/issues/new/choose) |
[使用和开发文档](https://linuxdo-scripts-docs.netlify.app/) |
[Discord 社区](https://discord.gg/n2pErsD7Kg)

> [!TIP] 
> 有什么好玩的功能我会第一时间分享在群聊，感觉自己发帖太频繁了  
> Discord 社区：https://discord.gg/n2pErsD7Kg  

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/anghunk)

## 目录
  - [目录](#目录)
  - [功能特性](#功能特性)
  - [使用方法](#使用方法)
  - [开发说明](#开发说明)
  - [更新日志](#更新日志)
  - [贡献历史](#贡献历史)
  - [免责声明](#免责声明)
  - [版权协议](#版权协议)

---

开发环境为 windows / chrome / 暴力猴，使用其他油猴管理器如果报错或者不生效，可以尝试使用暴力猴（我目前正在使用的，兼容性比较好）。

> [!WARNING]  
>  Arc 浏览器用户请使用暴力猴扩展。
>  Arc 浏览器下篡改猴扩展无法使用，存在兼容性问题，与插件无关，是浏览器和油猴管理器之间的问题。  

## 功能特性

- [x] 话题列表显示创建时间
- [x] 显示楼层数
- [x] 新标签页打开话题
- [x] 强制 block（拉黑屏蔽）某人的话题
- [x] 话题快捷回复（支持自定义）
- [x] 优化签名图显示防止图裂
- [x] 功能设置面板导入导出
- [x] 楼层抽奖
- [x] 只看楼主切换功能
- [x] 自动滚动阅读
- [x] 黑夜模式
- [x] 用户标签功能
- [x] 在话题列表可直接预览详情及评论
- [x] 评论框表情优化
- [x] 支持自定义 css 样式
- [x] 中英文混排优化显示
- [x] 新增等级信息查询
- [x] 切换论坛表情风格
- [x] AI 总结话题功能、智能生成回复
- [x] 支持 webdav 同步
- [x] 切换论坛主题皮肤

<details>
<summary>部分截图演示：</summary>

| ![image](https://github.com/user-attachments/assets/f3fb854f-e6fd-4da4-9a9c-377b6537fab7) | ![image](https://github.com/user-attachments/assets/3b2a9e63-3939-4dbc-a00f-c713ca2c7f33) |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| ![image](https://github.com/user-attachments/assets/2c67ab9f-2359-4ab5-b0dd-0f257560b98b) | ![image](https://github.com/user-attachments/assets/ed4f925c-e26c-43ce-a886-fa764ac341b5) |
| ![image](https://github.com/user-attachments/assets/c6ba9abb-43aa-40ce-a4a1-b9cdae229a2d) | ![image](https://github.com/user-attachments/assets/399c1645-36e1-4fe2-a671-ae40685e87ca) |

</details>


## 使用方法

点击此链接将会自动触发油猴脚本安装程序，后续也可以触发更新。

https://greasyfork.org/scripts/501827


## 使用方法（小白法）
首先我们需要安装一个用户脚本管理器，我用的是Greasemonkey 油猴子https://addons.mozilla.org/zh-CN/firefox/addon/greasemonkey/ 安装完成后在浏览器的扩展部分即可看到油猴子

然后我们就可以点击上述链接，下载该脚本。下载完成后，点击浏览器上部的扩展，点击油猴子，就可以看到linuxdo增强插件，可以自主管理插件。

最后我们打开https://linux.do/论坛就可以正常使用插件了。（但是我第一次安装使用卡了一下，多刷新几次就能出现插件了）
## 开发说明

```
node: v16.15.1
```

功能以组件形式展开，每次新增一个功能，注册一个新的组件避免冲突。

安装本仓库并下载依赖，运行代码。

```shell
git clone https://github.com/dlzmoe/linuxdo-scripts
yarn # 安装依赖
yarn dev # 本地运行
yarn build # 打包构建
```

程序会自动触发本地测试。

> 关于自动构建 Release 包，需要修改 `package.json` 中的 `version` 版本号，并且在 `CHANGELOG.md` 中写入当前版本更新日志。


## 更新日志

[version-log.md](https://github.com/dlzmoe/linuxdo-scripts/blob/main/version-log.md)


## 贡献历史

![Contributor](https://contrib.rocks/image?repo=dlzmoe/linuxdo-scripts)

[![Star History Chart](https://api.star-history.com/svg?repos=dlzmoe/linuxdo-scripts&type=Date)](https://star-history.com/#dlzmoe/linuxdo-scripts&Date)


## 免责声明

本脚本中提供的所有功能均仅在浏览器中运行，所使用的源代码公开透明可见，且本脚本仅学习研究使用，不使用任何盈利方案或参与任何盈利组织，因使用本脚本引起的或与本脚本有关的任何争议，各方应友好协商解决，本脚本对使用本脚本所提供的软件时可能对用户自己或他人造成的任何形式的损失和伤害不承担任何责任。如用户下载、安装和使用本产品中所提供的软件，即表明用户信任本作者及其相关协议和免责声明。


## 版权协议

[Apache-2.0 license](https://github.com/dlzmoe/linuxdo-scripts/blob/main/LICENSE)
