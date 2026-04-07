# 让 AI 帮你 commit

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
```

## 第一步：把 Token 给 AI

告诉你的 AI：

> "这是我的 GitHub Token：ghp_xxxxx，请帮我保管好，用来往我的 context 仓库 push 内容。"

AI 会把它存在安全的地方，不会暴露给别人。

## 第二步：告诉 AI 仓库名

> "我的 context 仓库是 `你的用户名/my-context`"

比如：`CheckedX/my-context`

## 第三步：正常对话

正常跟 AI 聊天，聊你的目标、你的困惑、你学到的东西。

AI 会自动识别值得记录的内容。

## 第四步：一键 commit

当 AI 问你：

> "今天有需要记的吗？"

或者你觉得某段对话值得记，你只需要说：

> "commit 这个内容"

AI 就会：
1. 整理成结构化的文档
2. 推送到你的 GitHub 仓库
3. 告诉你上传完成

## 实际例子

**对话**：
> 你：我今天学到了什么是 Token，它是 AI 操作 GitHub 的钥匙。
> AI：这个值得记吗？
> 你：commit
> AI：已推送到 `learnings/2026-04/token-knowledge.md`

**就这么简单。**

## 不想每次都确认？

你可以告诉 AI：

> "以后你觉得值得记的内容，直接 commit，不用问我。"

或者：

> "每次整理完后，给我看一眼，我确认了再 commit。"

选择适合你的模式。
