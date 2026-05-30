# AGI-DPA 独立版

一个纯前端的 AI 伴侣，无需服务器，手机浏览器打开即用。

👉 **[点此直接使用](https://ydsgangge-ux.github.io/AGI-HTML/)** 👈

## 功能

- 🧠 **独立运行** — 直接调用 LLM API，不需要电脑
- 💬 **智能对话** — 支持 DeepSeek / OpenAI / Moonshot / 智谱 / 通义千问
- 📝 **自动记忆** — 每 40 条对话自动整理重点摘要，长期记忆不丢失
- 🎭 **自定义人格** — 名字、性格、世界观，想怎么设怎么设
- 📱 **手机适配** — 深色主题，适配刘海屏和底部安全区
- 🔒 **数据本地** — 对话和配置全部存在你的浏览器，不上传任何服务器

## 使用方法

1. 点开上面的链接
2. 选择 API 服务商，填入你的 API Key
3. 开始聊天

就这么简单。

## 获取 API Key

| 服务商 | 注册地址 | 免费额度 |
|---|---|---|
| DeepSeek | [platform.deepseek.com](https://platform.deepseek.com) | 有 |
| 智谱 GLM | [open.bigmodel.cn](https://open.bigmodel.cn) | 有 |
| 通义千问 | [dashscope.aliyuncs.com](https://dashscope.aliyuncs.com) | 有 |
| Moonshot | [platform.moonshot.cn](https://platform.moonshot.cn) | 有 |
| OpenAI | [platform.openai.com](https://platform.openai.com) | 无 |

## 技术原理

整个应用是一个自包含的 HTML 文件（约 20KB），所有逻辑在浏览器端完成：

- 对话历史 → localStorage 持久化
- 记忆摘要 → 每 40 条自动调用 LLM 整理，注入后续对话的 system prompt
- LLM 调用 → 浏览器直接 fetch API，无中间服务器

## 分享

直接把链接发给朋友即可，每人填自己的 API Key，数据互不影响。

## License

MIT
