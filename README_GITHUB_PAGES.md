# GitHub Pages 部署文件清单

## ✅ 需要上传的文件

### 根目录文件：
1. `index.html` - 主页面文件（已修复路径）
2. `vite.svg` - 网站图标文件（已创建）

### 资源文件夹 assets/：
3. `index-GOkqsi8G.js` - 主JavaScript文件
4. `index-D3MXnc_n.css` - 主样式文件
5. `DashboardView-pJGY76wz.js` - 仪表板视图
6. `SettingsView-1mZpWaQV.js` - 设置视图
7. `ComparisonView-DjwIgruy.js` - 对比视图
8. `EnvBenefitsView-aq89EeSH.js` - 环境效益视图
9. `CostCalculatorView-F7Zzb_eb.js` - 成本计算器视图
10. `calcStore-CuhoDHwg.js` - 状态管理
11. `DashboardView-C85tewNm.css` - 仪表板样式
12. `SettingsView-BU4lV5Nj.css` - 设置样式
13. `ComparisonView-DbV7n1ES.css` - 对比样式
14. `EnvBenefitsView-Cl2Kc8Ti.css` - 环境效益样式
15. `CostCalculatorView-Brqob_qF.css` - 成本计算器样式

## 🔧 修复说明

### 主要修复内容：
1. **图标路径修复**：`/vite.svg` → `./vite.svg`
2. **所有资源使用相对路径**：确保在 GitHub Pages 上正确加载
3. **添加了缺失的 vite.svg 文件**

### 修复后的 index.html：
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <link rel="icon" type="image/svg+xml" href="./vite.svg" />  <!-- 修复路径 -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>版材成本对比专业版</title>
    <script src="https://cdn.jsdelivr.net/npm/echarts@5.5.0/dist/echarts.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/jspdf@2.5.1/dist/jspdf.umd.min.js"></script>
    <script type="module" crossorigin src="./assets/index-GOkqsi8G.js"></script>
    <link rel="stylesheet" crossorigin href="./assets/index-D3MXnc_n.css">
  </head>
  <body>
    <div id="app"></div>
  </body>
</html>
```

## 📤 上传步骤

1. **下载所有文件**：从 dist 文件夹中复制上述所有文件
2. **上传到 GitHub**：创建新的仓库或上传到现有仓库
3. **启用 GitHub Pages**：Settings → Pages → 选择 main 分支
4. **等待部署**：通常需要几分钟时间

## 🌐 访问地址

部署成功后，您的应用将可以通过以下地址访问：
```
https://[您的用户名].github.io/[仓库名称]/
```

## ⚠️ 常见问题

### 如果仍然空白：
1. 检查浏览器控制台错误
2. 确认所有文件都已上传
3. 检查文件路径是否正确
4. 等待 GitHub Pages 部署完成（可能需要几分钟）

### 文件路径检查：
- ✅ `./vite.svg`（正确）
- ❌ `/vite.svg`（错误，GitHub Pages 不支持）
- ✅ `./assets/`（正确）
- ❌ `/assets/`（错误）

## 📞 技术支持

如果上传后仍然有问题，请：
1. 检查浏览器开发者工具控制台
2. 确认所有文件都已正确上传
3. 等待 GitHub Pages 完全部署