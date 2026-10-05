# 你好，我是 summmmerz

应届毕业生，方向是 **LLM 应用与知识图谱**。习惯把踩过的坑做成能直接用的工具——所以这里的仓库大多有明确的使用场景、能跑起来，README 讲的是"为什么这么做"而不只是复述代码。

*English: CS graduate working on LLM applications and knowledge graphs. I like turning debugging pain into small tools that actually run.*

## 代表作

### research-topic-assistant · 智能科研选题助手（毕业设计）
基于大模型 + 知识图谱的科研选题推荐平台：Neo4j 存图谱、Redis 管会话、多特征融合排序产出推荐、Vue 3 + Element Plus 做前端。

`Python` `Flask` `Vue 3` `Neo4j` `Redis` · [仓库](https://github.com/summmmerz/research-topic-assistant)

### BiliMusicTool · 把歌单处理成能直接用的音频
输入歌名 → B 站搜索下载 → 提取曲绘 → 检测 BPM → 在歌曲开头补一个"它自己 BPM 的一小节"纯静音 → 输出 44.1kHz / 320kbps MP3。网页界面零构建：后端只用 Python 标准库，前端原生 HTML/CSS/JS，不装 npm 依赖。

`Python` `yt-dlp` `numpy` · [仓库](https://github.com/summmmerz/BiliMusicTool)

### dsh-spend-guard · 滚动窗口花费熔断
DeepSeek Harness 宿主插件：滚动 10 分钟窗口内花费到 ¥1 弹窗提醒、到 ¥2 直接结束当前轮。起因是 dsh 核心没有花费上限，而官方成本插件的"预算"只做展示、不会暂停任务。

`Node.js` `DSH plugin` · [仓库](https://github.com/summmmerz/dsh-spend-guard)

### dsh-notes · DSH 折腾笔记
环境体检、升级排障、token 花费诊断（直接用本机账本反解成本结构，定位到"输出 token"是主要成本项），另附三个可复用的 PowerShell 修复脚本。

`PowerShell` `Markdown` · [仓库](https://github.com/summmmerz/dsh-notes)

## 技术栈

Python · Flask · Vue 3 · Neo4j · Redis · SQLite · Node.js · PowerShell

## 一些做事的习惯

- **能免安装、免构建就免**——"装不上"是对用户最好的劝退
- **改完必须真跑一遍**，测试没过不算完成
- **踩过的坑写成文档**，而不是留在脑子里
- **密钥不进仓库**：只留 `.example` 占位符，真实值走环境变量

---

有问题或想聊，欢迎在对应仓库开 issue。
