# git演示项目
bug修复
Git 是目前最流行的**版本控制工具**，它能帮助你记录代码的每一次修改，方便你回退、协作开发。以下是 **Git 的基本用法**，包括常用命令和操作流程（以命令行为主）：

---

## 🧱 一、Git 基本概念

* **版本库（Repository）**：保存代码历史记录的地方。
* **工作区（Working Directory）**：你正在编辑的文件夹。
* **暂存区（Staging Area / Index）**：你准备提交的文件区域。
* **HEAD**：指向当前分支的最新提交。

---

## 🚀 二、Git 使用流程

以下是一次完整的 Git 操作流程：

### 1️⃣ 初始化仓库（第一次使用）

```bash
git init
```

> 创建一个 `.git` 隐藏目录，开始版本控制。

---

### 2️⃣ 添加远程仓库（可选，用于 GitHub）

```bash
git remote add origin https://github.com/你的用户名/项目名.git
```

---

### 3️⃣ 查看当前状态

```bash
git status
```

---

### 4️⃣ 添加文件到暂存区

```bash
git add 文件名
# 或添加所有变动文件：
git add .
```

---

### 5️⃣ 提交到本地仓库

```bash
git commit -m "你的提交说明"
```

---

### 6️⃣ 推送到远程仓库（GitHub 等）

```bash
git push -u origin main
```

> 第一次推送需要 `-u` 设置上游；以后可以直接用 `git push`

---

## 🔄 三、常见操作命令

### ✅ 查看提交记录

```bash
git log
```

### ✅ 克隆远程项目

```bash
git clone https://github.com/xxx/项目.git
```

### ✅ 拉取远程代码

```bash
git pull
```

### ✅ 创建新分支

```bash
git branch 新分支名
```

### ✅ 切换分支

```bash
git checkout 分支名
```

### ✅ 合并分支

```bash
git merge 分支名
```

---

## 🧹 四、一些实用命令

| 操作     | 命令                    |
| ------ | --------------------- |
| 删除文件   | `git rm 文件名`          |
| 修改文件名  | `git mv 旧名 新名`        |
| 撤销修改   | `git checkout -- 文件名` |
| 撤销 add | `git reset HEAD 文件名`  |
| 删除分支   | `git branch -d 分支名`   |
| 查看分支   | `git branch`          |
| 查看远程   | `git remote -v`       |

---

## 🧪 五、首次使用前建议设置用户名

```bash
git config --global user.name "你的名字"
git config --global user.email "你的邮箱"
```

---

如果你是初学者，我建议你先从 `git init → add → commit → push` 的流程反复练习。

你想了解更具体的操作吗，比如 [如何上传本地项目到 GitHub](f)、[分支管理实战](f) 或者 [常见错误解决方法](f)？
