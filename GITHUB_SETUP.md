# GitHub 上传步骤指南

## 已完成 ✅
- ✅ Git 仓库已初始化
- ✅ 文件已添加到暂存区
- ✅ 代码已提交到本地仓库

## 接下来需要做的：

### 1. 在 GitHub 上创建新仓库
1. 访问 https://github.com 并登录
2. 点击右上角 `+` → `New repository`
3. 填写仓库信息：
   - Repository name: `the-star-jar`（或你喜欢的名字）
   - Description: `一个基于物理引擎的情绪手账 Web 应用`
   - 选择 Public 或 Private
   - **不要勾选** "Initialize this repository with a README"
4. 点击 `Create repository`

### 2. 连接本地仓库到 GitHub
创建仓库后，GitHub 会显示命令。在项目目录下运行：

```bash
# 将 YOUR_USERNAME 替换为你的 GitHub 用户名
# 将 the-star-jar 替换为你创建的仓库名

git remote add origin https://github.com/YOUR_USERNAME/the-star-jar.git
git branch -M main
git push -u origin main
```

### 3. 如果遇到认证问题
如果提示需要认证，可以：
- 使用 GitHub Personal Access Token（推荐）
- 或使用 GitHub CLI (`gh auth login`)

### 4. 验证上传
上传成功后，刷新 GitHub 仓库页面，应该能看到所有文件。

## 快速命令（复制粘贴）

```bash
# 1. 添加远程仓库（替换 YOUR_USERNAME 和仓库名）
git remote add origin https://github.com/YOUR_USERNAME/the-star-jar.git

# 2. 设置主分支
git branch -M main

# 3. 推送到 GitHub
git push -u origin main
```

## 后续更新代码

如果以后修改了代码，使用以下命令更新：

```bash
git add .
git commit -m "更新说明"
git push
```

