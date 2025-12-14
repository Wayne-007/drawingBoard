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

## 代码逻辑详解

### HTML 结构
项目使用简单的 HTML 结构，包含以下主要元素：
- `<canvas>` 元素作为绘图区域
- 重置和保存功能的按钮

### CSS 样式设计
采用现代化 UI 设计理念：
- 使用渐变背景和阴影效果增强视觉层次感
- 按钮具有悬停和点击状态的交互动效
- 画布具有圆角和阴影，提升整体质感
- 响应式布局适配不同设备

### JavaScript 核心逻辑

#### 初始化和变量定义
```javascript
const canvas = document.getElementById('canvas');  // 获取画布元素
const ctx = canvas.getContext('2d');               // 获取2D绘图上下文
const resetBtn = document.getElementById('reset'); // 获取重置按钮
const saveBtn = document.getElementById('save');   // 获取保存按钮

// 绘图状态变量
let isDrawing = false;  // 是否正在绘制
let lastX = 0;          // 上一个绘制点的X坐标
let lastY = 0;          // 上一个绘制点的Y坐标
```

#### 事件监听
为画布添加鼠标事件监听器：
- `mousedown`: 开始绘制
- `mousemove`: 绘制过程
- `mouseup`: 停止绘制
- `mouseout`: 鼠标离开画布时停止绘制

#### 绘制函数
1. `startDrawing(e)`: 鼠标按下时触发，标记开始绘制并将当前位置设为起始点
2. `draw(e)`: 鼠标移动时触发，如果正在绘制则绘制从上一点到当前点的线条
3. `stopDrawing()`: 鼠标松开或离开画布时触发，标记停止绘制

#### 功能按钮
- 重置按钮：清空整个画布
- 保存按钮：将画布内容导出为PNG图片并下载

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
python -m SimpleHTTP.Server 8000
```

使用 Node.js:
```bash
npx http-server
```

或者使用其他本地服务器工具如 XAMPP、WAMP 等。

## 浏览器兼容性

- Chrome 52+
- Firefox 31+
- Safari 10+
- Edge 79+

## 许可证

MIT License

## 开发者

人工智障 waynehu2014@163.com