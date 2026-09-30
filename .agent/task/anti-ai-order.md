# anti-ai-order

status: DONE

inputs:
  - archives/vol-1-ch-1-hangong-zhengyan-1.draft.md     # writer 草稿
  - prompts/vol-1-ch-1-prompt.md                         # 同源提示词（验收依据）
  - .claude/knowledge/anti-ai.md
  - .claude/memory/
  - settings/writing-style.md
  - CLAUDE.md                                            # 项目规则：第三节第 7 条「正文做减法」、第四节称呼

outputs:
  - archives/vol-1-ch-1-hangong-zhengyan-1.anti-ai.md   # 去 AI 味正文 + 验收违反报告节（verdict PASS/FAIL）

round: 1

---

## 说明

- **不改剧情，只改表达**；不新增情节、细节、台词。字数低于 2500 不补。
- 同时按 CLAUDE.md 第三节第 7 条做减法：删设定复述、精确数字（身高/体重/厘米；时长可写）、具体年龄、情绪标签、冗余头衔修饰、技术/临床词、回指解释、资料卡与履历段、单独成行的强调句、解释性台词、心理说明、动作来由解释。**比喻、总结句不删**（交作者判断）。
- 照录文本一字不改：系统提示两行、天赋文本四行、【剧情世界：汉宫争艳，载入中。】、「小玖快回村里，你奶奶咽气了！」、「愿神勇的波塞冬大人庇佑你」。
- 禁用词（正文不得出现）：规则怪谈、主神在死亡之后、副本、诡异、诡币、时肆、等价交换、契约、本源核心、清海村、白雪、厘米、公斤、岁。
- skill 文件在 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`，允许只读。禁止读 `sexfight-database/`、`start/`。不使用 Bash 访问项目外路径。
- 不向作者提问；需要作者判断的点写在 .anti-ai.md 末尾「## 待作者回答的问题」（正文之外）。
- 完成后把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容）。
