# 🚀 MBCB 酒厂档案网页 - GitHub Pages 傻瓜教程

> 目标：把你的酒厂档案网页变成公开链接，发给朋友看！
> 预计时间：10-15分钟
> 难度：⭐⭐（有手就行）

---

## 第一步：注册 GitHub 账号（如果已有，直接跳到第二步）

1. 打开 [github.com](https://github.com)
2. 点击右上角 **"Sign up"**（注册）
3. 输入邮箱 → 设置密码 → 创建用户名
4. 按提示完成验证（可能会让你识别图片中的自行车/红绿灯 😂）
5. **记住你的用户名！** 后面会用到

---

## 第二步：创建仓库（Repository）

1. 登录 GitHub 后，点击右上角 **"+"** 号 → **"New repository"**

   ```
   + 号位置：页面右上角，你的头像左边
   ```

2. 填写仓库信息：

   | 项目 | 填写内容 | 说明 |
   |------|---------|------|
   | **Repository name** | `mbcb-breweries` | 仓库名字，可以随便取 |
   | **Description** | `MBCB酒厂档案展示页` | 描述，可选 |
   | **Public / Private** | ✅ **Public** | 必须选公开，否则Pages不免费 |
   | **Add a README** | ❌ **不要勾选** | 先不选，后面再说 |

3. 点击最下方绿色按钮 **"Create repository"**

---

## 第三步：上传网页文件

### 方法A：网页直接上传（推荐，最简单）

1. 进入刚创建的仓库页面
2. 你会看到 **"Quick setup"** 页面，点击 **"uploading an existing file"** 链接

   ```
   页面中间偏下位置，蓝色文字链接
   ```

3. 点击 **"choose your files"** 或直接把文件拖进去
4. 选择这个文件上传：
   ```
   /Users/damengmeng/Documents/Kimi/Workspaces/MBCB/breweries/index.html
   ```

5. 页面往下拉，看到 **"Commit changes"** 部分：
   - 第一个框写：`add brewery archive page`
   - 第二个框可以空着
   - 点击绿色按钮 **"Commit changes"**

### 方法B：命令行上传（如果你会用Terminal）

```bash
# 1. 进入网页所在目录
cd /Users/damengmeng/Documents/Kimi/Workspaces/MBCB/breweries

# 2. 初始化git
git init

# 3. 添加文件
git add index.html

# 4. 提交
git commit -m "add brewery archive page"

# 5. 关联远程仓库（把下面的 YOUR_USERNAME 换成你的GitHub用户名）
git remote add origin https://github.com/YOUR_USERNAME/mbcb-breweries.git

# 6. 推送
git branch -M main
git push -u origin main
```

---

## 第四步：开启 GitHub Pages

1. 在仓库页面，点击顶部菜单 **"Settings"**（⚙️ 齿轮图标）

   ```
   位置：仓库页面顶部，Code / Issues / Settings 那一排
   ```

2. 左侧边栏点击 **"Pages"**

   ```
   在左侧菜单里往下找，Code and automation 分类下
   ```

3. 在 **"Build and deployment"** 部分：
   - **Source**：选择 **"Deploy from a branch"**
   - **Branch**：选择 **"main"** → 文件夹选 **"/(root)"**
   - 点击 **"Save"**

4. 等待 1-3 分钟，刷新页面
5. 看到绿色提示框：
   ```
   Your site is live at https://YOUR_USERNAME.github.io/mbcb-breweries/
   ```
   🎉 **这就是你的公开链接！**

---

## 第五步：分享给朋友

把链接发给他们，例如：
```
https://YOUR_USERNAME.github.io/mbcb-breweries/
```

**把 YOUR_USERNAME 换成你的GitHub用户名**

示例：
```
https://damengmeng.github.io/mbcb-breweries/
```

---

## 🔄 后续更新教程

当我新增酒厂信息后，你需要更新网页：

### 每次更新的步骤：

1. **我会通知你**："网页已更新，请重新上传"
2. 你打开 GitHub 仓库页面
3. 点击 `index.html` 文件名
4. 点击右上角 **"Edit"**（铅笔图标 ✏️）
5. 删除全部内容，把我给你的新代码粘贴进去
6. 页面往下拉，在 **"Commit changes"** 处：
   - 第一个框写：`update brewery data`
   - 点击 **"Commit changes"**
7. 等待 1-2 分钟，刷新链接即可看到更新

---

## ❓ 常见问题

### Q1: 链接打不开/显示404？
- 检查仓库名和链接是否一致
- 确认 Settings → Pages 里 Branch 设置正确
- 等待 3-5 分钟再试（GitHub部署需要时间）

### Q2: 页面样式错乱？
- 确认上传的是 `index.html` 不是其他文件
- 检查文件名是否大小写正确（GitHub区分大小写）

### Q3: 想换仓库名字怎么办？
- Settings → General → Repository name 修改
- 但链接会变，需要重新分享给朋友

### Q4: 可以绑定自己的域名吗？
- 可以！Settings → Pages → Custom domain
- 需要购买域名并配置DNS，教程可以另发

### Q5: 手机能打开吗？
- 能！GitHub Pages 链接在任何设备都能访问
- 网页本身也是响应式设计，手机体验很好

---

## 📱 快速检查清单

- [ ] 注册了 GitHub 账号
- [ ] 创建了 Public 仓库
- [ ] 上传了 `index.html`
- [ ] Settings → Pages 开启了 main branch
- [ ] 拿到了 `https://用户名.github.io/仓库名/` 链接
- [ ] 链接能正常打开
- [ ] 发给朋友测试成功

---

## 🆘 卡住了怎么办？

把截图发给我，告诉我：
1. 你在哪一步卡住了？
2. 页面显示了什么错误信息？
3. 你的GitHub用户名是什么？

我会一步步帮你解决！

---

*教程版本：v1.0 | 适用：GitHub Pages 免费版*
