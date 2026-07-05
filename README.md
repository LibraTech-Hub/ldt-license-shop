# LDT Editor License Shop

LDT Editor 标准版激活页面

## 本地预览

```bash
# 方式 1: Python
python -m http.server 8000
# 访问 http://localhost:8000

# 方式 2: Node.js
npx serve .
```

## 部署到 GitHub Pages

1. 在 GitHub 创建仓库 `ldt-license-shop`
2. 推送代码：
   ```bash
   git init
   git add index.html README.md
   git commit -m "Initial commit"
   git remote add origin https://github.com/你的用户名/ldt-license-shop.git
   git push -u origin main
   ```
3. 仓库 Settings → Pages → Source: main → Save
4. 修改 `index.html` 中的 `API_URL` 为你的 Worker URL

## 配置

编辑 `index.html` 第 109 行，替换为你的 Worker URL：

```javascript
const API_URL = 'https://ldt-license-worker.你的子域名.workers.dev/api/generate-license';
```
