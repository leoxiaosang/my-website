# 苏衡测控 - 官方网站

## 公司信息

- **公司名称**：苏衡测控技术有限公司
- **联系电话**：18811906890
- **电子邮件**：info@suhengck.cn
- **公司地址**：江苏徐州泉山区工业园
- **主营产品**：皮带秤、电子皮带秤、称重传感器、皮带秤仪表、校验装置

## 部署说明

### 方法一：通过网页操作（推荐新手）

#### 第一步：创建 GitHub 账号
1. 访问 https://github.com
2. 点击 Sign up 注册账号（如果已有账号直接登录）

#### 第二步：创建新仓库
1. 点击右上角 **+** → **New repository**
2. 填写信息：
   - **Repository name**：`suheng-website`（或其他名称）
   - **Description**：苏衡测控官方网站
   - 选择 **Public**（GitHub Pages 需要 Public 仓库）
   - **不要**勾选 "Add a README file"（保持干净）
3. 点击 **Create repository**

#### 第三步：上传网站文件
1. 进入刚创建的仓库
2. 点击 **uploading an existing file**
3. 将以下 3 个文件拖拽上传：
   - `index.html`
   - `style.css`
   - `script.js`
4. 点击 **Commit changes**

#### 第四步：开启 GitHub Pages
1. 在仓库页面点击 **Settings**（设置）
2. 左侧菜单找到 **Pages**
3. 配置如下：
   - **Source**：选择 **Deploy from a branch**
   - **Branch**：选择 **main**，文件夹选 **/ (root)**
   - 点击 **Save**
4. 等待 1~2 分钟，页面会显示：
   > Your site is published at **https://你的用户名.github.io/suheng-website/**

---

### 方法二：通过 Git 命令行

```bash
# 1. 进入网站文件夹
cd /path/to/suheng-website

# 2. 初始化 Git 仓库
git init

# 3. 添加所有文件
git add .

# 4. 提交
git commit -m "first commit"

# 5. 关联 GitHub 仓库（替换为你的仓库地址）
git remote add origin https://github.com/你的用户名/suheng-website.git

# 6. 推送到 GitHub
git push -u origin main
```

然后在 GitHub 仓库 Settings → Pages 中开启即可。

---

## 自定义域名（可选）

如果已有域名（如 `www.suhengck.cn`），可以绑定：

1. 在仓库 Settings → Pages → **Custom domain** 填写你的域名
2. 在域名 DNS 处添加 CNAME 记录指向 `你的用户名.github.io`
3. 勾选 **Enforce HTTPS**（强制 HTTPS）
4. 中国域名需完成 ICP 备案

---

## 后续更新网站

修改 `index.html`、`style.css`、`script.js` 后：
1. 重新上传覆盖原文件，或用 `git push`
2. GitHub Pages 会自动重新部署（约 1~2 分钟生效）

---

## 访问地址格式

| 配置 | 访问地址 |
|------|---------|
| 用户名: `zhangsan` | `zhangsan.github.io/suheng-website/` |
| 自定义域名 | `www.suhengck.cn` |
