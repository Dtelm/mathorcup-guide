# mathorcup-guide

MathorCup 大数据竞赛参赛向导（报名截止 10.23 12:00；初赛 10.23 18:00 – 10.30 20:00；复赛 12.4 – 12.11）

给已报名选手的向导：先走分岔口确定你的路线（按基础 × 人数分 A1/A2/B1/B2 四条），再按天陪跑完赛前扫盲 → 读题选题 → 建模 → 编程 → 论文 → 调优 → 提交的全程。论文环节附历年获奖论文精华与 40 篇逐篇亮点加分项提炼。

---

## 快速开始（复制即用）

### 方式一：技能版（推荐）——和 AI 对话走完全程

需要准备：Node.js 18 以上（[下载](https://nodejs.org/zh-cn)）、Claude Code、Anthropic 账号。

```bash
# 1. 安装 Claude Code（国内网络慢时，先跑下一行换淘宝镜像再装）
#    npm config set registry https://registry.npmmirror.com
npm install -g @anthropic-ai/claude-code

# 2. 克隆本仓库
git clone https://github.com/Dtelm/mathorcup-guide.git

# 3. 进入仓库目录，启动 Claude Code
cd mathorcup-guide
claude

# 4. 在对话里输入
/mathorcup
```

然后按弹窗问答走即可（首次运行 `claude` 会提示登录 Anthropic 账号）。

没有 git / 不会命令行？在 GitHub 仓库页面点绿色 **Code** 按钮 → **Download ZIP** 下载解压，在解压后的文件夹里打开终端（Windows：文件夹地址栏输入 `cmd` 回车），执行上面的第 3、4 步。

安装说明详见 [Claude Code 官方文档](https://docs.claude.com/en/docs/claude-code/quickstart)。

### 方式二：手动版——零依赖，直接读文档

1. 第一步（约 10 分钟）：[00-分岔口：确定你的路线](https://github.com/Dtelm/mathorcup-guide/blob/main/00-%E5%88%86%E5%B2%94%E5%8F%A3-%E7%A1%AE%E5%AE%9A%E4%BD%A0%E7%9A%84%E8%B7%AF%E7%BA%BF.md)（点开直接读，不用下载）
2. 选定路线后进对应文档：

| 路线 | 适合谁 | 链接 |
|---|---|---|
| A1 有基础 + 三人分工 | 打过比赛、队友靠谱 | [进入](https://github.com/Dtelm/mathorcup-guide/blob/main/A-%E6%9C%89%E5%9F%BA%E7%A1%80/A1-%E4%B8%89%E4%BA%BA%E5%88%86%E5%B7%A5/%E8%B7%AF%E7%BA%BF.md) |
| A2 有基础 + 独立完成 | 打过比赛、自己扛 | [进入](https://github.com/Dtelm/mathorcup-guide/blob/main/A-%E6%9C%89%E5%9F%BA%E7%A1%80/A2-%E7%8B%AC%E7%AB%8B%E5%AE%8C%E6%88%90/%E8%B7%AF%E7%BA%BF.md) |
| B1 无基础 + 三人分工 | 第一次参赛、有队友 | [进入](https://github.com/Dtelm/mathorcup-guide/blob/main/B-%E6%97%A0%E5%9F%BA%E7%A1%80/B1-%E4%B8%89%E4%BA%BA%E5%88%86%E5%B7%A5/%E8%B7%AF%E7%BA%BF.md) |
| B2 无基础 + 独立完成 | 第一次参赛、一个人 | [进入](https://github.com/Dtelm/mathorcup-guide/blob/main/B-%E6%97%A0%E5%9F%BA%E7%A1%80/B2-%E7%8B%AC%E7%AB%8B%E5%AE%8C%E6%88%90/%E8%B7%AF%E7%BA%BF.md) |

3. 论文环节的两份参考：

| 参考 | 内容 | 链接 |
|---|---|---|
| 历年优秀论文精华 | 获奖论文共性：骨架、摘要写法、图表清单、模型选择、创新点套路 | [进入](https://github.com/Dtelm/mathorcup-guide/blob/main/%E5%8F%82%E8%80%83-%E5%8E%86%E5%B9%B4%E4%BC%98%E7%A7%80%E8%AE%BA%E6%96%87%E7%B2%BE%E5%8D%8E.md) |
| 论文亮点加分项 | 2021–2025 全部 40 篇逐篇亮点卡（带出处）+ 17 条加分项清单 + 对照三步法 | [进入](https://github.com/Dtelm/mathorcup-guide/blob/main/%E5%8F%82%E8%80%83-%E8%AE%BA%E6%96%87%E4%BA%AE%E7%82%B9%E5%8A%A0%E5%88%86%E9%A1%B9.md) |

## 里面有什么

- **分岔口**：四步问答判定路线（有基础三问 → 队友投入 → 画像确认 → 摇摆处理）
- **四条路线**：A1/A2/B1/B2 按天陪跑，含决策卡、止损线、AI 工具使用红线（防取消评奖资格）
- **论文三件套**：历年精华 + 40 篇亮点加分项 + 对照三步法（赛题发布后由向导带选手现场对照）
- **技能版**：Claude Code 技能，弹窗问答、一次一问，自包含（只复制 `SKILL.md` 一个文件到任意目录也能用）

## 常见问题

- **没有 Anthropic 账号？** 用方式二（手动版），文档内容完整，效果一样。
- **克隆/下载慢？** 用 GitHub 页面 Code → Download ZIP；npm 安装慢换淘宝镜像（见上面注释）。
- **技能里提到的"Codex"？** A2 路线（有基础单人）的强制挑错机制，可选装，不装也能走完路线。

## 状态

分岔口 + 四条路线第一版完成；论文参考已入库。向导不替选手写论文，也不给现成的示例论文——只教写法、讲亮点、守红线。
