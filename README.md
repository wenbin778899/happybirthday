# 🎉 兄弟生日快乐 - Interactive Birthday Webpage

一个充满创意和温情的生日祝福网页，结合了动画爱心树、烟花特效、照片轮播等多种互动元素，为特殊的人送上最真挚的生日祝福。

[![GitHub Pages](https://img.shields.io/badge/demo-GitHub%20Pages-brightgreen)](https://wenbin778899.github.io/happybirthday)
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://www.w3.org/html/)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://www.w3.org/CSS/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

## ✨ 项目特色

### 🌳 动画爱心树
- 基于HTML5 Canvas的精美爱心树动画
- 使用Jscex异步框架实现流畅的生长动画
- 包含种子、生长、开花、移动等多个动画阶段
- 点击种子开始动画序列

### 🎆 高性能烟花系统
- **智能性能优化**：FPS监控与自适应质量调节
- **流畅体验**：支持1.0/0.75/0.6三档画质自动切换
- **双击激活**：防误触设计，双击释放绚烂烟花
- **粒子系统**：最多320个粒子，15个同屏烟花限制
- **视觉效果**：HSL色彩系统，渐变轨迹，发光特效

### 📸 智能照片轮播
- **多模式显示**：底部内联 + 悬浮窗口双模式
- **拖拽功能**：悬浮模式支持自由拖拽定位
- **自动播放**：3.8秒间隔，带进度条显示
- **完整控制**：上一张/下一张/暂停/播放/关闭
- **记忆按钮**：FAB风格按钮，一键开启照片回忆

### 🎨 精美UI设计
- **响应式布局**：适配不同屏幕尺寸
- **暗色主题**：支持明暗主题切换
- **平滑动画**：CSS3过渡效果和transform动画
- **毛玻璃效果**：backdrop-filter模糊背景
- **滚动进度**：页面滚动进度可视化

## 🚀 在线演示

[查看在线演示](https://wenbin778899.github.io/happybirthday)

## 📁 项目结构

```
happybirthday/
├── index.html              # 主页面文件
├── LICENSE                 # 开源许可证
├── README.md              # 项目说明文档
├── css/                   # 样式和脚本目录
│   ├── default.css        # 主样式文件
│   ├── functions.js       # 工具函数
│   ├── love.js           # 爱心树动画逻辑
│   ├── jquery.min.js     # jQuery库
│   ├── jscex*.js         # Jscex异步框架
│   └── love.jpg          # 背景图片
├── music/                 # 背景音乐
│   └── love.mp3          # 背景音乐文件
└── photo/                 # 照片素材
    ├── fig1.jpg          # 照片1-13
    ├── ...
    └── fig13.jpg
```

## 🛠️ 本地开发

### 环境要求
- 现代浏览器（支持HTML5 Canvas, CSS3, ES6+）
- 本地HTTP服务器（推荐Python或Node.js）

### 快速开始

1. **克隆项目**
```bash
git clone https://github.com/wenbin778899/happybirthday.git
cd happybirthday
```

2. **启动本地服务器**

使用Python（推荐）：
```bash
# Python 3.x
python -m http.server 8000

# Python 2.x  
python -m SimpleHTTPServer 8000
```

使用Node.js：
```bash
npx serve .
# 或
npm install -g live-server
live-server
```

3. **访问页面**
```
http://localhost:8000
```

## 🌐 GitHub Pages部署

### 自动部署
1. Fork本项目到你的GitHub账户
2. 进入项目设置 Settings → Pages
3. 选择Source为 "Deploy from a branch"
4. 选择Branch为 "main" 或 "master"
5. 点击Save，等待部署完成
6. 访问 `https://wenbin778899.github.io/happybirthday`

### 手动部署
1. 将项目上传到GitHub仓库的gh-pages分支
2. 在仓库设置中启用GitHub Pages
3. 选择gh-pages分支作为发布源

## 🎯 使用说明

### 基础交互
- **启动动画**：点击页面中心的爱心种子
- **烟花特效**：双击右下角烟花按钮释放烟花
- **照片回忆**：点击记忆按钮开启照片轮播
- **主题切换**：点击月亮图标切换明暗主题

### 照片轮播操作
- **打开/关闭**：点击记忆按钮（🖼）
- **播放控制**：使用底部控制按钮
- **拖拽窗口**：切换到悬浮模式后可拖拽
- **快捷键**：ESC键关闭轮播窗口

### 性能优化
- 烟花系统会根据设备性能自动调节画质
- 支持帧率监控和自适应降级
- 闲置时自动停止动画循环节省资源

## 🎨 自定义指南

### 替换照片
1. 将新照片放入 `photo/` 目录
2. 命名为 `fig1.jpg` 到 `fig13.jpg`
3. 修改 `index.html` 中的照片描述文字

### 修改文字内容
编辑 `index.html` 中的以下部分：
```html
<span class="say"><h1>致最好的Duck：</h1></span>
<span class="say">你的祝福文字...</span>
```

### 更换背景音乐
1. 将音乐文件放入 `music/` 目录
2. 修改 `index.html` 中的音频源路径：
```html
<source src="music/your-music.mp3" type="audio/mp3" />
```

### 调整烟花参数
在 `index.html` 的FW对象中修改：
```javascript
const FW = {
    minFPS: 48,           // 最低FPS阈值
    maxParticles: 320,    // 最大粒子数
    baseBurst: 10,        // 每次发射烟花数
    cooldown: 250,        // 冷却时间(ms)
};
```

## 🔧 技术栈

- **前端框架**：原生HTML5 + CSS3 + JavaScript ES6+
- **动画引擎**：HTML5 Canvas + Jscex异步框架
- **UI库**：jQuery (DOM操作)
- **样式预处理**：原生CSS3 (Grid, Flexbox, Animations)
- **性能优化**：requestAnimationFrame + 自适应质量控制

## 📱 浏览器兼容性

| 浏览器 | 版本要求 | 支持程度 |
|--------|----------|----------|
| Chrome | 60+ | ✅ 完全支持 |
| Firefox | 55+ | ✅ 完全支持 |
| Safari | 12+ | ✅ 完全支持 |
| Edge | 79+ | ✅ 完全支持 |
| IE | ❌ | 不支持 |

## 🤝 贡献指南

欢迎提交Issue和Pull Request！

1. Fork本项目
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启Pull Request

## 📄 开源协议

本项目采用MIT协议开源 - 查看 [LICENSE](LICENSE) 文件了解详情

## 🙏 致谢

- [Jscex](https://github.com/JeffreyZhao/jscex) - 异步编程框架
- [jQuery](https://jquery.com/) - DOM操作库
- 所有为这个项目提供建议和支持的朋友们

## ⭐ Star History

如果这个项目对你有帮助，请给它一个Star！

[![Star History Chart](https://api.star-history.com/svg?repos=wenbin778899/happybirthday&type=Date)](https://github.com/wenbin778899/happybirthday/stargazers)

---

<div align="center">

**用代码传递温暖，用技术承载友情** ❤️

Made with ❤️ by [wenbin778899](https://github.com/wenbin778899)

[🔝 返回顶部](#-兄弟生日快乐---interactive-birthday-webpage)

</div>