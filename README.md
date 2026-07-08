# 汇率数据看板（公开网页版）

仅包含汇率看板，不含资金看板数据。

## 在线访问

发布到 GitHub Pages 后，访问地址为：

```
https://你的用户名.github.io/exchange-dashboard/
```

## 本地预览

直接用浏览器打开 `index.html`，或：

```bash
cd ~/Desktop/exchange-dashboard
python3 -m http.server 8080
# 打开 http://127.0.0.1:8080
```

## 实时更新

网页版已内置**浏览器实时刷新**（无需本地 Python 服务）：

- 打开页面自动拉取新浪财经最新汇率
- 每 **5 分钟**自动刷新
- 可手动点 **「刷新实时汇率」**

访问地址：

```
https://jianqiuni7-ui.github.io/exchange-dashboard/
```

## 更新历史数据后重新发布

在 `~/Desktop/汇率` 目录运行：

```bash
bash 同步发布网页.sh
```

然后在 GitHub Desktop 里 Commit + Push `data.js` 即可。


## GitHub Pages 开启步骤

1. 把本仓库 Push 到 GitHub（建议仓库名 `exchange-dashboard`）
2. 打开 GitHub 仓库 → **Settings** → **Pages**
3. **Source** 选 **Deploy from a branch**
4. **Branch** 选 `main`，文件夹选 **/ (root)**
5. 点 **Save**，等 1～2 分钟

> 免费 GitHub Pages 需要仓库为 **Public（公开）**。若必须私有，可用 Netlify 免费托管。
