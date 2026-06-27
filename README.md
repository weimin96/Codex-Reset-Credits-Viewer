# ChatGPT Codex 重置额度查看器

这是一个可通过 GitHub 关联 Greasy Fork 发布的用户脚本，用于在 `chatgpt.com` 页面查看当前账号的 Codex reset credits、最近过期时间和下次额度重置时间。

## 发布文件

发布到 Greasy Fork 时使用：

```text
Codex-Reset-Credits-Viewer.user.js
```

脚本不依赖外部 JavaScript、图片或样式资源，主体代码直接包含在发布文件中。

## Greasy Fork 关联 GitHub

在 Greasy Fork 后台创建或编辑脚本时，将代码同步地址设置为：

```text
https://raw.githubusercontent.com/weimin96/Codex-Reset-Credits-Viewer/main/Codex-Reset-Credits-Viewer.user.js
```

之后在 GitHub 更新 `Codex-Reset-Credits-Viewer.user.js` 并递增 `@version`，Greasy Fork 即可从该 raw 地址同步新版本。

## 安装方式

1. 安装 Tampermonkey 或 Violentmonkey。
2. 在 Greasy Fork 新建脚本，粘贴 `Codex-Reset-Credits-Viewer.user.js` 的完整内容，或使用上方 GitHub raw 地址同步。
3. 保存并安装脚本。
4. 打开 `https://chatgpt.com/`，登录后点击页面右下角的“Codex 额度”按钮查看数据。

## 权限说明

- `@match` 仅匹配 `https://chatgpt.com/*`。
- `@grant none`，不使用用户脚本管理器扩展 API。
- `@homepageURL` 和 `@supportURL` 指向 GitHub 仓库，便于 Greasy Fork 展示源码与反馈入口。
- 数据请求只访问当前页面同源的 ChatGPT 接口，并携带当前登录态。

## 发布检查

发布前至少确认：

- metadata 中包含 `@name`、`@description`、`@namespace`、`@version`、`@match`、`@license`、`@homepageURL` 和 `@supportURL`。
- 版本号在每次修改脚本代码后递增。
- 脚本未压缩、未混淆，且功能与描述一致。
