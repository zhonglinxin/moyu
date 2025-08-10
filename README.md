# 摸鱼特工 - Goof Off Agent

一款基于 Next.js 和 Phaser 3 开发的休闲策略游戏。

## 技术栈

- **框架**: Next.js 15.4.6
- **游戏引擎**: Phaser 3.90.0
- **语言**: TypeScript
- **样式**: Tailwind CSS

## 快速开始

### 安装依赖
```bash
npm install
```

### 启动开发服务器
```bash
npm run dev
```

然后访问 [http://localhost:3000](http://localhost:3000)

### 构建生产版本
```bash
npm run build
npm run start
```

## 项目结构

```
├── app/                 # Next.js App Router
├── src/
│   ├── components/      # React组件
│   │   └── PhaserGame.tsx
│   └── game/           # Phaser游戏代码
│       ├── config/     # 游戏配置
│       └── scenes/     # 游戏场景
│           ├── PreloadScene.ts
│           ├── MainMenuScene.ts
│           └── GameScene.ts
├── doc/                # 文档
│   └── moyu.md        # 游戏需求文档
└── todo.md            # 开发任务清单
```

## 游戏玩法

- **目标**: 在5分钟内尽可能多地"摸鱼"，同时避免被巡查员发现
- **操作**: 
  - 点击"工作"按钮切换到工作状态
  - 点击"摸鱼"按钮进入摸鱼状态
  - 摸鱼时快速点击屏幕积累金币
- **失败条件**:
  - 工作时间超过30秒（过劳）
  - 摸鱼时被巡查员发现
  - 时间结束时金币不足

## 当前实现功能

- ✅ Phaser 3集成到Next.js
- ✅ 基础场景管理（加载、主菜单、游戏场景）
- ✅ 核心游戏循环
- ✅ 工作/摸鱼状态切换
- ✅ 工作进度条系统
- ✅ 摸鱼点击积分系统
- ✅ 金币奖励机制
- ✅ 游戏计时系统
- ✅ 失败判定逻辑

## 待开发功能

详见 [todo.md](./todo.md)