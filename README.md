# 五月天粉丝站 · Mayday Fan Site

> 🎸 一个专为五月天歌迷打造的个人记录与社区互动平台
>
> **这个项目从需求构思到功能上线，全程通过自然语言对话驱动 AI 完成，零手写代码。**

🌐 **在线访问：** [genuine-truffle-61ae61.netlify.app](https://genuine-truffle-61ae61.netlify.app)

---

## 项目亮点

这是一个典型的 **Vibe Coding** 实践案例：

- ✅ 产品需求、UI 设计、功能迭代全部通过自然语言描述
- ✅ 数据库设计、SQL 建表、RLS 权限策略由 AI 生成
- ✅ 从零到上线，开发者**没有手写过一行代码**
- ✅ 完整的用户系统、云数据库、生产环境部署

---

## 功能列表

| 功能模块 | 说明 |
|---|---|
| 🏠 首页 | 成名历程时间轴、演唱会倒计时、今日冷知识 |
| 💿 专辑 & 成员 | 9张专辑展示、5位成员介绍、歌曲库收藏 |
| 🎤 演唱会 | 8大巡演卡片、世界巡演地图 |
| 📔 我的 | 五迷等级系统、演唱会日记（三级联动打卡）、回忆相册轮播、年度报告 PDF |
| 💬 留言墙 | 歌迷排行榜、昵称设置、便签留言、点赞 |

---

## 技术栈

- **前端：** 原生 HTML / CSS / JavaScript（单文件）
- **数据库：** Supabase（PostgreSQL + Row Level Security）
- **存储：** Supabase Storage（演唱会照片）
- **部署：** Netlify（静态托管）
- **AI 工具：** Kiro IDE

---

## 数据库结构

```
fan_messages      - 留言墙（内容、昵称、点赞数、颜色）
concert_diary     - 演唱会打卡记录（用户 × 场次）
concert_photos    - 演唱会回忆照片（文件路径、巡演名）
favorite_songs    - 歌曲收藏（用户 × 歌曲 key）
user_profiles     - 用户昵称
```

---

## Vibe Coding 过程

整个项目的开发流程：

1. 用一句话描述想法：「我想做一个五月天粉丝网站」
2. AI 生成初版 UI 原型（HTML）
3. 通过对话迭代功能：「加登录」「加演唱会日记」「改成轮播」...
4. AI 生成 Supabase 建表 SQL，手动在控制台执行
5. AI 处理跨域、RLS 权限、部署配置等问题
6. 拖拽文件夹到 Netlify 完成部署

**整个过程没有打开过代码编辑器，没有手写过任何代码。**

---

## 本地运行

```bash
git clone <repo-url>
cd project/public
npx serve .
# 浏览器打开 http://localhost:3000
```

> 需要配置 Supabase 环境变量，详见 `public/index.html` 中的连接配置。

---

## License

MIT
