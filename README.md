# Drawing Board 画板

一个简单易用的在线画板应用，使用 HTML5 Canvas 技术实现。

## 功能特性

- 🎨 简洁直观的绘图界面
- ✏️ 平滑的线条绘制体验
- 🔄 一键清空画布
- 💾 保存作品为 PNG 图片
- 📱 响应式设计，适配不同屏幕尺寸
- 🎨 精美的 UI 设计，带有渐变按钮和阴影效果

## 技术栈

- HTML5 Canvas API
- Vanilla JavaScript (无框架依赖)
- CSS3 样式设计

## 项目结构

```
drawingBoard/
├── index.html       # 主页面
├── style/
│   └── index.css    # 样式文件
└── js/
    └── index.js     # 核心功能逻辑
```

## 快速开始

### 在线预览

直接打开 `index.html` 文件即可使用本应用。

### 本地运行

由于浏览器安全策略限制，建议通过本地服务器运行：

使用 Python:
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

使用 Node.js:
```bash
# 安装 http-server
npm install -g http-server

# 启动服务
http-server
```

然后在浏览器中访问 `http://localhost:8000` 或相应端口。

## 使用说明

1. 打开应用后即可在画布上自由绘制
2. 点击"重置"按钮清空画布
3. 点击"保存"按钮将当前画作下载为 PNG 图片

## 设计亮点

- 采用现代化 UI 设计，包含圆角、阴影和渐变效果
- 按钮具有悬停和点击反馈效果
- Canvas 画布带有圆角和阴影，提升视觉层次感
- 响应式布局，适配不同设备屏幕

## 浏览器兼容性

- Chrome 5+
- Firefox 4+
- Safari 5+
- Edge 12+

## 许可证

MIT License

## 开发者

人工智障 waynehu2014@163.com