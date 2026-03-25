# 游戏积分计算器

计算器相关文件已经统一放在 `integral/` 目录中：

- `index.html`
- `积分计算器.html`
- `.nojekyll`

## 本地打开

直接打开 `integral/index.html` 即可，它会跳转到实际页面 `integral/积分计算器.html`。

## GitHub Pages 发布

这个项目已经改成适合 `integral/` 子目录发布的结构，并新增了工作流：

- `.github/workflows/deploy-integral-pages.yml`

工作流会在你推送到 `main` 分支时，把 `integral/` 目录作为 GitHub Pages 的站点内容发布。

### 首次启用

1. 把整个仓库推到 GitHub。
2. 打开仓库 `Settings`。
3. 进入 `Pages`。
4. 在 `Build and deployment` 里把 `Source` 选成 `GitHub Actions`。
5. 提交或再次推送代码，等待工作流运行完成。

### 访问地址

- 项目页通常是：`https://你的用户名.github.io/仓库名/`

### 说明

- 站点根目录会直接对应 `integral/` 里的文件
- 所以线上首页会是 `integral/index.html`
- `index.html` 会继续跳转到 `积分计算器.html`

## 说明

- `index.html` 是入口页
- `积分计算器.html` 是实际功能页面
- 页面当前使用 `localStorage` 保存数据，不同设备之间不会自动同步
