# anti-ai-order

status: DONE

inputs:
  - archives/vol-1-ch-2-hangong-zhengyan-2.draft.md     # writer 稿；`---` 之后是 writer 的字数与新增细节清单，不算正文
  - prompts/vol-1-ch-2-prompt.md                         # 同源提示词（验收依据；末尾「待作者回答的问题」按暂行验收）
  - .claude/knowledge/anti-ai.md                         # 顶部「WUXIAN 作者覆盖」优先于下文所有条目
  - .claude/memory/
  - settings/writing-style.md
  - CLAUDE.md                                            # 第三节第 7 条（2026-10-01 放宽）

outputs:
  - archives/vol-1-ch-2-hangong-zhengyan-2.anti-ai.md   # 正文部分原样复制 writer 稿正文（一字不改）；`---` 之后：修改建议清单 + 验收违反报告节（verdict PASS/FAIL）+ writer 新增细节清单原样转录 + 待作者回答的问题

round: 1

---

## 说明

- **只列问题、不直接改稿**（作者 2026-10-01 定）：`.anti-ai.md` 的正文部分与 writer 草稿正文逐字一致；所有修改意见写成编号建议清单（每条：原句 → 建议改法 → 理由），交作者逐条 OK/NG。
- 以 anti-ai.md 顶部作者覆盖为准：拟声词、口语化重复描写、「倒吸/吸了一口凉气」（不频繁）、像/仿佛/如同**都不当 AI 味**；情绪标签、心理说明、动作来由解释、比喻、总结句**不列为问题**。拿不准的只列、标「存疑」。
- 仍可列出的：设定复述、回指上一章的解释、精确数字、冗余头衔、技术/临床词、解释性句子、单独成段的强调句（拟声词单独成段可以）、机制解释、T1 句式、相邻段重复、前后对不上。
- verdict 只按提示词红线判：照录文本（进剧情世界提示两行、白雪反应三句、系统任务四行、三条遗言、【本源核心：4/5】、何贵人台词）逐字在场；禁用词（时肆、诡异、诡币、等价交换、契约、何莲、王荣、规则怪谈、主神在死亡之后、叙述里的「副本」、本钱、厘米、公斤、岁——白雪那句「三岁小孩」为照录例外）；吐槽不加引号；只跟林叁玖视角；不写乳斗过程；宴席两笔；侍女不进门无对话；不提毒；不评遗言；章末停在吐槽。
- 非性斗章：文风卡句长 / 感叹句比例偏离**只记录、不判 FAIL**。字数低于 2000 不补、不判 FAIL。
- writer 列出的新增细节（草稿 `---` 之后）由作者删留，你不删不改；在报告里原样转录。
- skill 文件在 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`，允许只读。禁止读 `sexfight-database/`、`start/`。不使用 Bash，不访问项目外路径（skill 目录除外）。
- 不向作者提问；需要作者判断的点写在 .anti-ai.md 末尾「## 待作者回答的问题」（每条附建议）。
- 完成后把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容）。
