# 读书助手 (Reading Coach)

91 个 AI 读书提示词，覆盖从选书到蜕变的完整读书旅程。网页版打开即用，支持接入任意大模型 API。

## 功能

- **14 个分类 × 91 条提示词**：慧眼识书 → 与书对谈 → 落纸成金 → 知行合一 → 与贤对饮 → 穿针引线 → 量体裁衣 → 温故知新 → 授人以渔 → 横岭侧峰 → 良师益友 → 对症下药 → 善假于物 → 脱胎换骨
- **填入参数，一键生成个性化指令**
- **支持接入任意 OpenAI 兼容 API**（DeepSeek、OpenAI、通义千问、智谱、硅基流动等）
- **支持 AI 对话**（流式输出，边聊边学）
- **纯前端，无需安装**

## 下载 & 使用

1. 从 [Releases](https://github.com/huige-opc/reading-coach/releases) 下载最新版 `index.html`
2. 浏览器直接打开 `index.html` 即可
3. 无需安装任何软件，无需 Node.js，无需 Python

> 也可以直接 clone 仓库：`git clone https://github.com/huige-opc/reading-coach.git`

## API 设置

首次使用需配置大模型 API（不配置则只能生成指令，不能用 AI 对话功能）：

1. 点击左下角 **⚙ API 设置**
2. 填入以下信息：

| 字段 | 说明 | 示例 |
|------|------|------|
| API 地址 | 服务商 API 端点 | `https://api.deepseek.com` |
| API Key | 你的 API 密钥 | `sk-xxxxxxxx` |
| 模型名称 | 模型 ID | `deepseek-chat` |

3. 点击保存。右上角状态灯变绿即配置成功

**支持的 API 服务商**（兼容 OpenAI Chat Completions 格式即可）：

| 服务商 | API 地址 | 推荐模型 |
|--------|----------|----------|
| DeepSeek | `https://api.deepseek.com` | `deepseek-chat` |
| OpenAI | `https://api.openai.com` | `gpt-4o-mini` |
| 硅基流动 | `https://api.siliconflow.cn` | `Qwen/Qwen2.5-7B-Instruct` |
| 智谱 AI | `https://open.bigmodel.cn/api/paas/v4` | `glm-4-flash` |
| 阿里百炼 | `https://dashscope.aliyuncs.com/compatible-mode/v1` | `qwen-plus` |
| Moonshot | `https://api.moonshot.cn` | `moonshot-v1-8k` |

## 使用方法

1. 左侧选择分类（如"慧眼识书"）
2. 点击提示词卡片（如"值不值得读"）
3. 填写参数（如书名）
4. 点击 **生成指令** → 自动复制到剪贴板，粘贴到任意 AI 对话中使用
5. 或点击 **生成并对话** → 直接在页面内与 AI 对话

## 提示词分类

| 分类 | 数量 | 场景 |
|------|------|------|
| 慧眼识书 | 6 | 选对书、读对书 |
| 与书对谈 | 9 | 读懂、读透、读进去 |
| 落纸成金 | 5 | 记住、输出、用起来 |
| 知行合一 | 8 | 让书解决现实问题 |
| 与贤对饮 | 6 | 跟作者/角色/思想对话 |
| 穿针引线 | 6 | 把不同书之间打通 |
| 量体裁衣 | 8 | 根据个人情况读书 |
| 温故知新 | 5 | 让读书成为成长记录 |
| 授人以渔 | 4 | 把书变成影响力 |
| 横岭侧峰 | 8 | 让读书更有趣更深刻 |
| 良师益友 | 6 | 让书成为人生教练 |
| 对症下药 | 8 | 职场/关系/财富细分 |
| 善假于物 | 7 | 笔记/表格/清单模板 |
| 脱胎换骨 | 5 | 让书重塑你这个人 |

## 安全说明

- API Key 仅保存在浏览器 localStorage，不上传任何服务器
- 所有请求直接从浏览器发送到你配置的 API 地址
- 源码公开，欢迎审计

## 进阶玩法：用 AI Agent 调教专属读书助手

这个工具本身可以通过 AI Agent（如 Claude Code、Trae、Cursor 等）持续迭代优化。你可以告诉 Agent：

- "把回复风格改成我喜欢的xxx作家风格"
- "帮我加一个读书计时功能"
- "新增一个分类，专门用来帮我写读书笔记"
- "调整系统提示词，让 AI 回复更口语化/更学术/更毒舌"

**不需要懂代码。** 打开 Agent，把 `index.html` 或 `SKILL.md` 扔进去，用自然语言描述你想要的效果，AI 帮你改完直接预览。迭代到你满意为止。

## 联系

- 微信：HgAiAgent（扫码添加，拉你进 AI 学习交流群）
- 邮箱：[szlihui801@gmail.com](mailto:szlihui801@gmail.com)
- GitHub：[github.com/huige-opc](https://github.com/huige-opc)

## 许可证

本项目基于 [MIT License](LICENSE) 开源，可自由使用、修改和分发。
