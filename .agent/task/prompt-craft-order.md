# prompt-craft-order

status: DONE

inputs:
  - chapters/vol-1-ch-1.md                      # 章纲（作者已确认 2026-09-30），含末尾「作者答复」
  - volumes/volume-1.md                          # 卷纲 1-1 条（辅助）
  - settings/writing-style.md                    # 文风主卡（本章非性斗章，不用 style-profiles/fight.md）
  - settings/character-setting/lin-sanjiu.md
  - settings/world-setting.md
  - .claude/memory/                              # prompt-memory.md 等动态记忆
  - .claude/knowledge/anti-ai.md
  - .claude/knowledge/prompt-setting-style.md
  - .claude/knowledge/chapter-quality-checklist.md
  - .claude/knowledge/permanent-memory.md
  - .claude/knowledge/genre-example.md
  - .claude/knowledge/memory-format-spec.md
  - start/yuan/1.txt  只读 L1–L73               # 作者特许；本书改编底本第 1 章

outputs:
  - prompts/vol-1-ch-1-prompt.md

---

## 任务

组装**第 1 卷第 1 章「汉宫争艳（1）」**的 6 元素提示词。上一章：无（ch-1，前情上下文标注无前置章节）。

## 读取权限

- 允许读：上方 inputs；项目根 `CLAUDE.md`（项目规则全程生效，尤其第三节第 7 条「正文做减法」、第四节称呼）。
- skill 文件不在项目里，在 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`（prompt-crafting.md、prompt-audit.md、memory-recording.md 等），允许只读。
- `start/yuan/1.txt` **只读 L1–L73**。
- **禁止读** `sexfight-database/`；禁止读 `start/` 下除 1.txt L1–L73 以外的任何内容。

## 1.txt 素材处理（writer 不读原文，素材必须进提示词）

把章纲要求的节拍素材从 1.txt L1–L73 提炼**改写后**放进提示词：回帖三层意思、倒计时（二十分钟 → 十分钟 → 两分钟）、村长电话、同事台词、原书男女主天赋名与等级、吐槽比喻串（上战场不让带枪、进考场忘带笔、刮刮乐没中还倒扣十块；有人一出生就在罗马、她的起点是贫民窟）等。
- 1.txt 措辞必须改写，不大段照抄。以下三处**照录**：天赋文本 L55–58 四行；「愿神勇的波塞冬大人庇佑你」；村长那句「小玖快回村里，你奶奶咽气了！」。
- 「一切只能靠自己」删去。

## 必须写进提示词的硬约束

- 不出现：书名《规则怪谈：主神在死亡之后》、「规则怪谈」「副本」「诡异」「诡币」「时肆」「等价交换」「契约」「本源核心」「清海村」「白雪」。
- 系统提示照章纲：【叮！首次进入的试炼者，可以获得一次抽取天赋的机会。】【系统正在为您抽取……】；天赋文本四行（照录 L55–58）；章末【剧情世界：汉宫争艳，载入中。】，章末停在这行，后面什么都不写。
- 只跟林叁玖视角，不进同事、村长、网友内心。
- 做减法：不写设定复述、精确数字（身高、体重、厘米；「七年」「二十分钟」等时长可以）、具体年龄、情绪标签、技术/临床词、资料卡与履历段、单独成行的强调句、解释性台词、心理说明、动作来由解释。**比喻和总结句不主动删**（作者自己判断）。
- 章纲「设定依据（严禁写进正文）」区块的任何解释都不得进入给 writer 的正文要求里。
- 字数 2500–3000，软指标，不为凑字数加内容；不新增章纲以外的情节。

## 不向作者提问

需要作者判断的点写进提示词文件末尾「## 待作者回答的问题」（逐条编号；这一节写在提示词正文之外，注明 writer 忽略），不自行补、不自行取舍。

## 完成

写完后用 Write 把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容，不删除本文件）。
