# Claude Code 简历技能集

一套专注于简历优化、求职申请和职业发展的 AI 智能体技能。面向求职者、转行人士，以及希望借助 Claude Code 完成简历撰写、ATS 优化、面试准备和制定求职策略的职场人士。

## 什么是 Skills？

Skills（技能）是为 AI 智能体提供特定任务所需专业知识和工作流程的 Markdown 文件。将这些文件添加到项目后，Claude Code 就能在你处理简历和求职任务时识别相关场景，并应用合适的方法框架和最佳实践。

## 可用技能

| 技能 | 说明 |
|-------|-------------|
| [resume-ats-optimizer](/skills/resume-ats-optimizer) | 针对应聘者跟踪系统（ATS）优化简历，检查 ATS 兼容性，分析关键词匹配情况 |
| [resume-bullet-writer](/skills/resume-bullet-writer) | 将平淡的经历描述改写为突出成果的要点，体现量化指标和实际影响 |
| [job-description-analyzer](/skills/job-description-analyzer) | 分析职位描述，计算匹配分数，识别差距，制定求职申请策略 |
| [resume-tailor](/skills/resume-tailor) | 在保持真实性的前提下，针对具体职位定制简历 |
| [cover-letter-generator](/skills/cover-letter-generator) | 根据简历和职位描述，生成个性化、有说服力的求职信 |
| [linkedin-profile-optimizer](/skills/linkedin-profile-optimizer) | 让 LinkedIn 个人资料与简历保持一致，提高被搜索到的机会和互动效果 |
| [interview-prep-generator](/skills/interview-prep-generator) | 根据简历生成 STAR 法则故事、模拟面试题和表达要点 |
| [salary-negotiation-prep](/skills/salary-negotiation-prep) | 调研市场薪资水平，制定谈薪策略，准备还价话术 |
| [tech-resume-optimizer](/skills/tech-resume-optimizer) | 优化软件工程、产品经理及其他技术岗位的简历 |
| [executive-resume-writer](/skills/executive-resume-writer) | 撰写突出战略领导力的企业高管及副总裁级别简历 |
| [career-changer-translator](/skills/career-changer-translator) | 将一个行业中的技能转化为另一个行业易于理解的表述，识别可迁移技能 |
| [resume-quantifier](/skills/resume-quantifier) | 发掘可补充量化指标的内容，在缺少具体数字时进行估算 |
| [resume-formatter](/skills/resume-formatter) | 确保排版对 ATS 友好，生成整洁、便于快速浏览的版式 |
| [portfolio-case-study-writer](/skills/portfolio-case-study-writer) | 将简历要点扩展为作品集中的详细案例分析 |
| [academic-cv-builder](/skills/academic-cv-builder) | 为学术岗位整理履历，涵盖论文发表、科研资助和教学经历 |
| [reference-list-builder](/skills/reference-list-builder) | 规范整理职业推荐人名单，准备推荐所需材料 |
| [offer-comparison-analyzer](/skills/offer-comparison-analyzer) | 并排比较多个工作 Offer，分析整体薪酬待遇 |
| [resume-version-manager](/skills/resume-version-manager) | 跟踪不同简历版本，维护主简历，管理各岗位的定制版本 |
| [creative-portfolio-resume](/skills/creative-portfolio-resume) | 为创意类岗位平衡视觉设计与 ATS 兼容性 |
| [resume-section-builder](/skills/resume-section-builder) | 针对不同经验水平和岗位，创建并优化相应的简历板块 |

## 安装

### 方式一：通过命令行安装（推荐）

```bash
# 全局安装全部 20 个技能（适用于所有项目）
npx skills add Paramchoudhary/ResumeSkills -g -y

# 仅安装到当前项目
npx skills add Paramchoudhary/ResumeSkills -y

# 查看已安装的技能
npx skills list

# 查看全局安装的技能
npx skills list --global
```

### 方式二：手动安装

```bash
# 克隆仓库并复制到技能目录
git clone https://github.com/Paramchoudhary/ResumeSkills.git
mkdir -p ~/.cursor/skills
cp -r ResumeSkills/skills/* ~/.cursor/skills/
```

### 方式三：直接下载

从 `/skills` 目录下载所需的单个技能文件，并将其添加到你的 AI 智能体的技能目录。

### 卸载

```bash
# 按名称移除单个技能
npx skills remove resume-ats-optimizer
npx skills remove resume-bullet-writer

# 或从目录中移除所有技能
rm -rf ~/.agents/skills/resume-*
rm -rf ~/.cursor/skills/resume-*
```

## 支持的 AI 智能体

这些技能可用于多种 AI 编程助手：

- **Cursor**（IDE）
- **Claude Code**（CLI）
- **Windsurf**
- **Codex**
- **Gemini CLI**
- **Amp、Antigravity、Augment** 等 30 多种工具

## 使用方法

安装完成后，直接向 AI 助手提出简历相关需求即可：

```
“帮我优化简历，提高 ATS 兼容性”
→ 使用 resume-ats-optimizer 技能

“帮我改进简历中的经历要点”
→ 使用 resume-bullet-writer 技能

“我应该申请这个岗位吗？”＋粘贴职位描述
→ 使用 job-description-analyzer 技能

“帮我为这个岗位写一封求职信”
→ 使用 cover-letter-generator 技能

“帮我准备 Google 的面试”
→ 使用 interview-prep-generator 技能
```

## 技能分类

### 简历优化

- `resume-ats-optimizer` - 帮助简历通过 ATS 筛选
- `resume-bullet-writer` - 撰写突出成果的经历要点
- `resume-quantifier` - 补充量化指标和数字
- `resume-formatter` - 提供整洁、便于快速浏览的排版
- `resume-section-builder` - 创建有针对性的简历板块

### 求职策略

- `job-description-analyzer` - 分析岗位匹配度并制定策略
- `resume-tailor` - 针对具体岗位定制简历
- `resume-version-manager` - 管理多个简历版本
- `offer-comparison-analyzer` - 比较不同的工作 Offer

### 配套材料

- `cover-letter-generator` - 撰写个性化求职信
- `linkedin-profile-optimizer` - 优化 LinkedIn 个人资料
- `portfolio-case-study-writer` - 撰写作品集内容
- `reference-list-builder` - 整理职业推荐人名单

### 面试与谈薪

- `interview-prep-generator` - 准备 STAR 法则故事和模拟面试题
- `salary-negotiation-prep` - 制定薪资谈判策略

### 特定岗位与职业场景

- `tech-resume-optimizer` - 软件工程、产品经理及其他技术岗位
- `executive-resume-writer` - 企业高管及副总裁级别岗位
- `academic-cv-builder` - 学术岗位
- `creative-portfolio-resume` - 设计及创意类岗位
- `career-changer-translator` - 职业转型与跨行业求职

## 为什么需要这些技能？

**常见问题：**

- 75% 的简历在被人工查看之前，就已被 ATS 淘汰
- 每个岗位平均收到 250 份申请
- 大多数简历的经历描述缺乏说服力，也没有量化指标
- 求职者将时间浪费在不适合自己的岗位上

**解决方案：**

- 通过优化格式和关键词，提高 ATS 筛选通过率
- 用突出成果的经历要点脱颖而出
- 有策略地申请与自身匹配的岗位
- 通过定制申请材料，更快获得面试机会

**带来的效果：**

- 每次投递获得的面试机会增至原来的 2–3 倍
- 获得更高质量的回复
- 加快求职进程（平均节省 2 个月）
- 提升谈薪效果（获得薪资高出 10,000 美元以上的 Offer）

## 快速上手示例

### 示例一：全面优化简历

```
用户：这是我的简历［粘贴简历］。我正在申请数据科学家岗位，请帮我优化一下。

Claude 将会：
1. 检查 ATS 兼容性
2. 对照数据科学家岗位的常见要求进行分析
3. 补充量化指标，改进经历要点
4. 建议添加合适的关键词
5. 调整排版，确保 ATS 兼容性
```

### 示例二：针对具体岗位定制简历

```
用户：这是职位描述［粘贴职位描述］和我的简历［粘贴简历］。我应该申请这个岗位吗？

Claude 将会：
1. 计算匹配分数
2. 识别优势与差距
3. 标出招聘信息中的潜在风险
4. 提供简历定制策略
5. 生成求职信的表达要点
```

### 示例三：准备面试

```
用户：我即将参加［公司名称］的［岗位名称］面试。这是我的简历，请帮我做准备。

Claude 将会：
1. 根据你的经历整理 STAR 法则故事
2. 预测可能出现的面试问题
3. 为每条简历要点准备讲述思路
4. 调研该公司的面试特点，提供针对性准备
5. 准备适合向面试官提问的问题
```

## 参与贡献

发现了改进技能的方法？有新技能的建议？欢迎提交 Pull Request 和 Issue！

贡献指南请参阅 [CONTRIBUTING.md](CONTRIBUTING.md)。

### 你可以如何参与

- 改进现有技能的说明
- 补充特定行业的示例
- 为特定场景创建新技能
- 修正错别字，或让表述更清晰
- 添加其他语言的翻译

## 许可证

本项目采用 MIT 许可证，你可以按需使用这些技能。

详情请参阅 [LICENSE](LICENSE)。

## 关于本项目

适用于 Claude Code 的简历技能集，涵盖 ATS 优化、经历要点撰写、岗位匹配、面试准备和职业发展。

**关键词：** 简历、CV、ATS、求职、职业发展、面试、求职信、LinkedIn、薪资谈判、求职申请

---

*为每一位求职者用心打造。祝你求职顺利！*
