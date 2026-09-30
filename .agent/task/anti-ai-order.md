# anti-ai-order

status: DONE

inputs:
  - archives/vol-1-ch-1-hangong-zhengyan-1.draft.md     # writer 重跑稿（2026-10-01）；`---` 之后是 writer 的字数与新增细节清单，不算正文
  - prompts/vol-1-ch-1-prompt.md                         # 同源提示词（验收依据；末尾「待作者回答的问题」是暂行处理，照暂行验收）
  - .claude/knowledge/anti-ai.md
  - .claude/memory/
  - settings/writing-style.md
  - CLAUDE.md                                            # 第三节第 7 条已于 2026-10-01 放宽

outputs:
  - archives/vol-1-ch-1-hangong-zhengyan-1.anti-ai.md   # 整份重新生成并覆盖（旧版作废，不读旧版）：去 AI 味正文 + 验收违反报告节（verdict PASS/FAIL）

round: 1

---

## 说明

- **不改剧情，只改表达**；不新增情节、细节、道具、台词。字数低于 2500 不补。
- 减法按放宽后的 CLAUDE.md：**不删**情绪标签、心理说明、动作来由解释、比喻、总结句。仍删：设定复述、旁白复述身份、精确数字（身高/体重/厘米/年龄；时长可写）、冗余头衔、技术/临床词、解释性台词、单独成段的强调句（拟声词单独成段可以）、机制解释。
- writer 列出的新增细节（草稿 `---` 之后）由作者删留，**你不删也不改写其内容**；在报告里原样转录该清单。正文里不保留 `---` 附录。
- 文风卡的句长 / 感叹句比例是从性斗样本学来的，非性斗章偏离这组数值**只记录、不判 FAIL**，列为待作者回答的问题。
- 照录文本一字不改：系统提示 11 行（双天赋 6 行 + 魔镜真言 4 行 + 【剧情世界：汉宫争艳，载入中。】）、「小玖快回村里，你奶奶咽气了！」、「愿神勇的波塞冬大人庇佑你」。
- 禁用词（正文不得出现）：规则怪谈、主神在死亡之后、副本、诡异、诡币、时肆、等价交换、契约、本源核心、清海村、白雪、厘米、公斤、岁。帖子标题与回帖不得用【】。
- skill 文件在 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`，允许只读。禁止读 `sexfight-database/`、`start/`。不使用 Bash 访问项目外路径。
- 不向作者提问；需要作者判断的点写在 .anti-ai.md 末尾「## 待作者回答的问题」（正文之外）。
- 完成后把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容）。
