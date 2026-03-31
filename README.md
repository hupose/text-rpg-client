# Text RPG Frontend

文字 RPG 放置游戏 - 前端部分

## 技术栈

- HTML5 + CSS3
- Vanilla JavaScript (无框架)
- Socket.IO Client (实时通信)

## 文件结构

```
frontend/
├── index.html    # 主页面
├── styles.css    # 样式
├── ui.js         # UI 渲染与交互
├── api.js        # 后端 API 调用封装
└── README.md     # 本文件
```

## 功能

- 双职业选择（物理/魔法）
- 属性加点系统
- 自动战斗
- 药品购买与使用
- 离线挂机战斗
- 实时状态同步 (WebSocket)

## 运行

需要配合后端服务：

```bash
# 启动后端 (在 server 目录)
cd ../server && node server.js

# 访问
http://localhost:3000
```

## 配置

在 `api.js` 中修改后端地址：

```javascript
const API_BASE = 'http://localhost:3000';
const SOCKET_URL = 'http://localhost:3000';
```

## 相关仓库

- [text-rpg-server](https://github.com/hupose/text-rpg-server) - 后端代码
- [text-rpg-client](https://github.com/hupose/text-rpg-client) - 本仓库（前端）