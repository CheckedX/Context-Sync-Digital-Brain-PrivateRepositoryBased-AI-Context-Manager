# Context-Sync-Digital-Brain-PrivateRepositoryBased-AI-Context-Manager
消除 AI 孤岛，让所有 Agent 共享同一个大脑。

基于 GitHub 私有仓库构建的跨平台个人上下文同步方案。

支持自动总结对话、跨 Agent 异步同步，通过 Git 持久化自己的偏好与知识，实现 Agent 间的无缝认知传递。 

通过 Git 协议，实现真正的 Personal Knowledge as a Service (PKaaS)。

# 与其让数据碎片化在不同的 AI 厂商服务器里，

# 不如将自己的 Context 握在自己手里。


[English](#english) | [中文](#中文)

---

<a name="中文"></a>
## 这是什么？

一个让你的 AI 助手自动整理对话内容、并推送到 GitHub 私有仓库的工作方法。

**你需要什么**：
- 一个 GitHub 账号
- 一个 AI 助手
- 5 分钟配置时间

**你能得到什么**：
- AI 自动帮你整理值得记住的内容
- 一键 commit 到你的私有仓库
- 跨平台、跨设备调用你的 context
- AI 越来越懂你

---

## 为什么需要这个？

**没有 context 管理的痛苦**：
- 每次对话从零开始
- AI 记不住你说过的话
- 重复解释自己的背景和偏好

**有了 context 管理**：
- AI 记住你的目标、偏好、经历
- 对话越来越高效
- 你的知识库持续积累

---

## 核心流程

```
你跟 AI 对话
    ↓
AI 识别值得记录的内容
    ↓
AI 整理成文档
    ↓
你说"commit"
    ↓
AI 自动推送到 GitHub
    ↓
你的 context 库持续增长
```

---

## 第一步：创建 GitHub 仓库

### 1.1 新建仓库

1. 登录 GitHub
2. 点击右上角 `+` → `New repository`
3. 填写：
   - Repository name: `my-context`（或任何你喜欢的名字）
   - 选择 `Private`（私有仓库）
   - 勾选 `Add a README file`
4. 点击 `Create repository`

### 1.2 推荐的仓库结构

```
my-context/
├── README.md           # 仓库说明
├── profile/            # 个人档案
│   └── identity.md     # 基本信息、目标、偏好
├── projects/           # 项目经验
├── learnings/          # 学到的知识
├── decisions/          # 重要决策及理由
├── idea-seeds/         # 想法种子
└── glossary.md         # 术语表
```

---

## 第二步：获取 Personal Access Token

### 2.1 为什么需要 Token？

Token 是一把钥匙，让你的 AI 助手能通过 API 操作你的仓库。

### 2.2 获取步骤

1. 登录 GitHub
2. 右上角头像 → `Settings`
3. 左侧菜单最下方 → `Developer settings`
4. `Personal access tokens` → `Tokens (classic)`
5. 点击 `Generate new token (classic)`
6. 填写：
   - Note: `context-manager`（随便写，方便识别）
   - Expiration: `No expiration` 或 `90 days`
   - 勾选权限：**`repo`**（完整仓库权限）
7. 点击 `Generate token`
8. **立即复制保存**（只显示一次！）

Token 长这样：`ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`

### 2.3 安全提醒

⚠️ Token 相当于你仓库的钥匙，不要泄露给别人！

如果泄露了：
1. 立刻回到 Token 管理页面
2. 点击 `Delete` 删除这个 Token
3. 重新生成一个新的

---

## 第三步：让 AI 帮你 commit

### 3.1 把 Token 给你的 AI

告诉你的 AI：
> "这是我的 GitHub Token：ghp_xxxxx，请帮我保管好，用来往我的 context 仓库 push 内容。"

AI 会把它存在安全的地方（比如加密文件），不会暴露给别人。

### 3.2 告诉 AI 你的仓库名

> "我的 context 仓库是 `你的用户名/my-context`"

### 3.3 开始对话

正常跟 AI 聊天。聊到值得记录的内容时，AI 会提醒你。

### 3.4 一键 commit

当 AI 问你"要不要 commit"时，你只需要说：
> "commit"

AI 就会自动整理内容并推送到 GitHub。

---

## 第四步：定期复盘

### 4.1 设置定时提醒

让 AI 在固定时间提醒你复盘：
> "每天中午 12 点和晚上 10 点，提醒我看看有没有要记的内容。"

### 4.2 复盘流程

AI 会问你：
> "今天我们的对话有需要记的吗？"

你回答：
- "有，把 XX 记一下" → AI 整理并 commit
- "没有" → 跳过

---

## 什么值得记录？

### ✅ 值得记录

| 类型 | 例子 |
|------|------|
| 方法论 | "如何用 GitHub 管理 context" |
| 决策+理由 | "为什么选择 XX 职业方向" |
| 可复用知识 | 行业术语、工具技巧 |
| 项目经验 | 完整的项目记录 |
| 关键洞察 | 你突然想到的点子 |

### ❌ 不值得记录

- 日常闲聊
- 临时操作细节
- 没有沉淀价值的信息

---

## 常见问题

### Q: Token 泄露了怎么办？

立刻删除并重新生成。步骤见 [第二步](#第二步获取-personal-access-token)。

### Q: 私有仓库安全吗？

比你想象的更安全：
- 只有你能看到
- GitHub 有完善的安全机制
- 敏感内容建议放本地，不要传 GitHub

### Q: 每次都要说"commit"吗？

不一定要。你可以让 AI 自己判断何时提醒你，或者设置定时复盘。

### Q: 我能自己手动上传吗？

可以。你随时可以登录 GitHub 手动编辑或上传文件。AI 自动化只是更省事。

### Q: 换了一个 AI 怎么办？

你的 context 在 GitHub，不属于任何一个 AI。把仓库和 Token 给新的 AI，它就能继续用。

---

## 进阶玩法

### 使用模板仓库

1. Fork 这个仓库模板
2. 把示例内容替换成你自己的
3. 配置 Token，开始使用

---

## 反馈与贡献

这个项目由 CheckedX 和格子 共同创建。

如果你觉得有用，欢迎：
- Star 这个仓库
- 分享给朋友
- 提出改进建议

---

*a smarter way to work with AI*
