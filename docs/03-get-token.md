# 获取 Personal Access Token

## Token 是什么？

**Token = 一把钥匙**

它让你的 AI 助手能通过 API 操作你的 GitHub 仓库。

不是密码，而是专门给程序用的"通行证"。

## 获取步骤

### 步骤 1：进入设置页面

1. 登录 GitHub
2. 右上角头像 → `Settings`

### 步骤 2：找到开发者设置

左侧菜单最下方 → `Developer settings`

### 步骤 3：进入 Token 页面

`Personal access tokens` → `Tokens (classic)`

### 步骤 4：生成新 Token

点击 `Generate new token (classic)`

### 步骤 5：填写信息

| 字段 | 填什么 |
|------|--------|
| Note | `context-manager`（随便写，方便识别） |
| Expiration | `No expiration` 或 `90 days` |
| 权限 | 勾选 **`repo`** ✅ |

> 只需要勾选 `repo`，其他不用勾

### 步骤 6：保存 Token

点击 `Generate token`

**立刻复制保存！**

Token 长这样：`ghp_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`

⚠️ **只显示一次，关掉就看不到了！**

## 安全提醒

| 做 ✅ | 不做 ❌ |
|------|--------|
| 存在安全的地方 | 发给别人 |
| 只给信任的 AI | 发到公开群聊 |
| 定期更换 | 写在公开文档里 |

## 泄露了怎么办？

1. 立刻回到 Token 管理页面
2. 找到泄露的 Token
3. 点击 `Delete`
4. 重新生成一个新的

**删除后，旧的 Token 立刻失效。**

## 下一步

把 Token 给你的 AI 助手，它就能帮你 commit 了。
