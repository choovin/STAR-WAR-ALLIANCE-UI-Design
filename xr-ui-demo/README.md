# MR星战大联盟 - 3D UI设计项目

🚀 **基于WebXR技术的沉浸式混合现实射击游戏界面设计**

[![WebXR](https://img.shields.io/badge/WebXR-Compatible-blue)](https://webxr.org/)
[![A-Frame](https://img.shields.io/badge/A--Frame-1.4.0-red)](https://aframe.io/)
[![PICO](https://img.shields.io/badge/PICO-4UE%20Optimized-green)](https://www.picoxr.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## 📖 项目简介

MR星战大联盟是一款专为混合现实设备设计的多人在线射击游戏的3D用户界面原型。项目采用WebXR技术栈，特别针对PICO 4UE头显设备进行了深度优化，提供沉浸式的3D空间交互体验。

## ✨ 核心特色

### 🎮 游戏功能
- **多人在线对战** - 支持最多8人同时游戏
- **丰富武器系统** - 包含突击步枪、狙击枪、霰弹枪等多种武器
- **战队协作** - 团队模式，强调策略配合
- **实时语音** - 内置语音聊天系统
- **成就系统** - 完整的等级和成就体系

### 🥽 XR体验
- **3D空间界面** - 立体化的用户界面设计
- **手势交互** - 支持手部追踪和手势操作
- **头部追踪** - 6DOF头部位置追踪
- **空间音频** - 3D立体声音效
- **触觉反馈** - 震动反馈增强沉浸感

### 🎨 视觉设计
- **科幻风格** - 星战主题的视觉设计
- **全息效果** - 发光材质和全息投影效果
- **动态UI** - 流畅的界面切换动画
- **响应式布局** - 适配不同设备分辨率

## 🛠️ 技术栈

| 技术 | 版本 | 用途 |
|------|------|------|
| **A-Frame** | 1.4.0 | WebXR框架，3D场景渲染 |
| **WebXR** | Latest | VR/AR设备兼容性 |
| **JavaScript** | ES6+ | 交互逻辑和事件处理 |
| **HTML5** | Latest | 页面结构 |
| **CSS3** | Latest | 样式和动画 |
| **Three.js** | (via A-Frame) | 底层3D图形渲染 |

## 📁 项目结构

```
xr-ui-demo/
├── 📄 README.md                 # 项目说明文档
├── 📄 产品设计文档.md            # 详细的产品设计规范
├── 📄 task.md                   # 项目任务清单
├── 🌐 3D-UI.html               # 统一的3D界面演示平台
├── 🎮 01-主菜单界面.html        # 游戏主菜单
├── 🏠 02-房间大厅界面.html       # 多人房间大厅
├── ⚔️ 03-武器装备界面.html       # 武器装备系统
├── 🎯 04-游戏内HUD界面.html      # 游戏内抬头显示
├── 📊 05-战绩统计界面.html       # 战绩和数据统计
├── 👥 06-社交好友界面.html       # 社交和好友系统
├── ⚙️ 07-设置配置界面.html       # 游戏设置配置
├── 🎓 08-教学引导界面.html       # 新手教学引导
├── 📝 XR-3D-UI-Design-Prompt.md # 设计提示文档
└── 📝 demo.md                   # 演示说明
```

## 🚀 快速开始

### 环境要求

- **浏览器**: Chrome 90+, Firefox 90+, Edge 90+ (支持WebXR)
- **设备**: PICO 4UE, Quest 2/3, HoloLens 2 或其他WebXR兼容设备
- **网络**: 本地HTTP服务器或HTTPS环境

### 安装步骤

1. **克隆项目**
   ```bash
   git clone https://github.com/your-username/mr-starwar-alliance.git
   cd mr-starwar-alliance
   ```

2. **启动本地服务器**
   ```bash
   # 使用Python
   python -m http.server 8000
   
   # 或使用Node.js
   npx http-server -p 8000
   
   # 或使用PHP
   php -S localhost:8000
   ```

3. **访问演示**
   - 在浏览器中打开: `http://localhost:8000/3D-UI.html`
   - 或访问单独界面: `http://localhost:8000/01-主菜单界面.html`

### VR设备使用

1. **PICO 4UE**
   - 确保设备连接WiFi
   - 打开浏览器访问本地IP地址
   - 点击VR图标进入沉浸模式

2. **Meta Quest**
   - 启用开发者模式
   - 使用Oculus Browser访问
   - 允许WebXR权限

## 🎮 界面说明

### 主要界面

| 界面 | 功能描述 | 特色功能 |
|------|----------|----------|
| **主菜单** | 游戏入口，用户登录 | 微信登录、星空背景 |
| **房间大厅** | 多人房间管理 | 实时玩家状态、地图预览 |
| **武器装备** | 武器选择和配置 | 3D武器展示、配件系统 |
| **游戏HUD** | 游戏内信息显示 | 准星、血量、小地图 |
| **战绩统计** | 数据分析展示 | 3D图表、排行榜 |
| **社交好友** | 好友和战队管理 | 在线状态、团队聊天 |
| **设置配置** | 游戏参数设置 | 音量、画质、控制 |
| **教学引导** | 新手训练教程 | 互动式教学、虚拟训练场 |

### 交互方式

- **鼠标/触摸**: 点击按钮和界面元素
- **键盘**: 数字键1-8切换界面，空格键总览模式
- **VR控制器**: 射线指向和触发器点击
- **手势追踪**: 直接用手指点击(支持的设备)
- **语音命令**: "返回主菜单"、"切换界面"等

## 🔧 开发指南

### 自定义界面

1. **创建新界面**
   ```html
   <!DOCTYPE html>
   <html>
   <head>
       <script src="https://aframe.io/releases/1.4.0/aframe.min.js"></script>
   </head>
   <body>
       <a-scene>
           <!-- 你的3D界面元素 -->
       </a-scene>
   </body>
   </html>
   ```

2. **添加交互逻辑**
   ```javascript
   // 注册自定义组件
   AFRAME.registerComponent('custom-interaction', {
       init: function () {
           this.el.addEventListener('click', function () {
               // 处理点击事件
           });
       }
   });
   ```

### 性能优化建议

- **减少多边形数量**: 使用低模型和LOD技术
- **优化材质**: 避免过多的透明和发光效果
- **控制动画**: 限制同时播放的动画数量
- **合理使用光照**: 减少动态光源数量
- **纹理压缩**: 使用适当的纹理分辨率

## 📱 设备兼容性

### 完全支持
- ✅ PICO 4UE (推荐)
- ✅ Meta Quest 2/3
- ✅ HTC Vive
- ✅ Valve Index

### 部分支持
- ⚠️ HoloLens 2 (AR模式)
- ⚠️ Magic Leap 2
- ⚠️ 移动设备 (有限功能)

### 浏览器支持
- ✅ Chrome 90+ (推荐)
- ✅ Firefox 90+
- ✅ Edge 90+
- ❌ Safari (WebXR支持有限)

## 🐛 常见问题

### Q: 界面显示模糊或性能差？
A: 检查设备性能设置，降低渲染质量或关闭部分视觉效果。

### Q: VR模式无法进入？
A: 确保使用HTTPS或localhost，检查浏览器WebXR权限。

### Q: 手势追踪不工作？
A: 确认设备支持手势追踪，检查浏览器权限设置。

### Q: 音频没有3D效果？
A: 检查音频权限，确保使用耳机或立体声扬声器。

## 🤝 贡献指南

我们欢迎社区贡献！请遵循以下步骤：

1. Fork 项目
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

### 代码规范
- 使用ES6+语法
- 遵循A-Frame最佳实践
- 添加适当的注释
- 确保跨设备兼容性

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情。

## 🙏 致谢

- [A-Frame](https://aframe.io/) - 优秀的WebXR框架
- [Three.js](https://threejs.org/) - 强大的3D图形库
- [WebXR](https://webxr.org/) - 开放的XR标准
- [PICO](https://www.picoxr.com/) - 设备支持和优化

## 📞 联系我们

- **项目主页**: https://github.com/your-username/mr-starwar-alliance
- **问题反馈**: https://github.com/your-username/mr-starwar-alliance/issues
- **邮箱**: contact@mrstarwar.com
- **QQ群**: 123456789

---

⭐ 如果这个项目对你有帮助，请给我们一个星标！

**让我们一起构建未来的XR游戏体验！** 🚀🎮