# 创建 GitHub 仓库

## 第一步：新建仓库

1. 登录 GitHub（没有账号先注册一个）
2. 点击右上角 `+` → `New repository`

![new repo](./images/new-repo.png)

3. 填写信息：

| 字段 | 填什么 |
|------|--------|
| Repository name | `my-context`（或任何你喜欢的名字） |
| Description | 我的 AI 记忆库（可选） |
| 可见性 | 选择 `Private`（私有）✅ |
| README | 勾选 `Add a README file` |

4. 点击 `Create repository`

## 第二步：创建文件夹结构

你的仓库应该长这样：

```
my-context/
├── README.md           # 仓库说明
├── profile/            # 个人档案
│   └── identity.md     # 基本信息
├── projects/           # 项目经验
├── learnings/          # 学到的知识
├── decisions/          # 重要决策
├── idea-seeds/         # 想法种子
└── glossary.md         # 术语表
```

### 各文件夹的作用

| 文件夹 | 存什么 |
|--------|--------|
| profile/ | 你是谁、你的目标、你的偏好 |
| projects/ | 你做过或正在做的项目 |
| learnings/ | 你学到的知识、方法论 |
| decisions/ | 你做过的重要决定和理由 |
| idea-seeds/ | 你的灵感和想法 |
| glossary.md | 行业术语、专业词汇 |

## 第三步：创建第一个文件

在 GitHub 网页上：

1. 点击 `Add file` → `Create new file`
2. 文件路径输入：`profile/identity.md`
3. 内容填写：

```markdown
# 个人档案

## 基本信息
- 姓名：
- 年龄：
- 职业：

## 目标
- 

## 偏好
- 

## 当前困境
- 
```

4. 点击 `Commit new file`

## 完成！

你的 Context 仓库建好了。下一步：获取 Token，让 AI 能操作它。
