# AIGC 作品集 · GitHub Pages 上线指南

本仓库已包含可直接发布的静态站点：

- `index.html` — 简约作品集页面（深色风格，点击封面灯箱播放）
- `assets/covers/*.jpg` — 5 张作品封面
- `assets/videos/*.mp4` — 5 个已压缩视频（单文件均 <100MB，符合 GitHub 限制）

作品顺序：寒王殿下的隐婚药妃 → 家有一姥 → 夜噬 → 野火 → Mustang 汽车广告

---

## 你只需做 3 步（在本机该文件夹打开终端执行）

### 1. 在 GitHub 新建空仓库

登录 github.com → New repository → 填仓库名（如 `aigc-works`，**不要**勾选 README/.gitignore）→ Create。

### 2. 推送到 GitHub

把下面命令里的 `<用户名>` 和 `<仓库名>` 换成你自己的，逐条执行：

```bash
git remote add origin https://github.com/<yu131405-netizen>/<yuxiaoteng-AIGC>.git
git branch -M main
git push -u origin main
```

> 推送时会要求输入用户名和密码：**密码处填你的 GitHub Personal Access Token（不是账号密码）**。  
> 没有 Token？github.com → Settings → Developer settings → Personal access tokens → 生成，勾选 `repo` 权限。

### 3. 开启 GitHub Pages

仓库页 → Settings → Pages → Source 选 **main** 分支、文件夹 **/root** → Save。  
等待 1～2 分钟，访问 `https://<用户名>.github.io/<仓库名>/` 即可看到作品集。

---

后续更新：修改文件后 `git add -A && git commit -m "更新" && git push`。
