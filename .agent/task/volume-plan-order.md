# volume-plan-order

status: DONE

inputs:
  - story.md
  - notes/15-汉宫争艳大纲.md
  - notes/00-决策记录.md
  - settings/world-setting.md
  - settings/genre-setting.md
  - settings/foreshadowing.md
  - settings/timeline.md
  - settings/character-setting/lin-sanjiu.md
  - settings/character-setting/wang-meiren.md
  - settings/character-setting/he-huanghou.md
  - .claude/knowledge/volume-setting-style.md
  - .claude/knowledge/plot-craft/

outputs:
  - volumes/volume-1.md

resume_from:

---

## 任务

规划第 1 卷《汉宫争艳》卷纲，输出 `volumes/volume-1.md`。current_volume: 1。

## 权限例外（作者特许）

1. **notes/ 读取**：作者特许读取 `notes/15-汉宫争艳大纲.md` 与 `notes/00-决策记录.md`（仅这两份；notes/ 其余文件不读）。
2. **skill 文件**：你引用的 `skills/volume-arc.md`、`skills/volume-direction.md`、`skills/volume-writing.md`、`skills/memory-recording.md` 不在项目内，位于 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`。**只允许只读这四个文件**，该目录其他文件不读，项目外其他路径一律不访问。
3. **禁读**：`sexfight-database/`、`start/` 不读（取材出处已在大纲 15 注明，照抄标注即可，不需要去核对原文）。

## 流程要求

- **STEP 0 主线拆纲：跳过。** 作者类型 B（只知道开头），story.md 已写好（全书终点、卷间断点待定）。**不改 story.md。**
- **STEP 1 不向作者提问**（你无法与作者对话）：大纲 15 已回答剧情方向。
- **只把大纲 15 整理成卷纲格式**：
  - 不重新设计剧情、不增删情节、不改章数（**10 章**）。
  - 不改性斗取材出处、回合顺序与【改】标注。
  - 不改本源核心数字：王美人 4（开局）→ 3（第 5 章后）→ 2（第 9 章后）；何贵人/何皇后 5 → 0（第 9 章）；女官 4。
  - 若发现剧情缺口或冲突，写在 volume-1.md 末尾「待作者回答的问题」一节，**逐条编号**，不自行补。
- **剧情以 notes/15 为准**；notes/00 与 notes/15 冲突时以 notes/00 较晚条目为准，仍不确定就列入「待作者回答的问题」。
- **题材卡节奏规则**（genre-setting 的 max_consecutive_* 等）已标为未经作者确认、不作约束；验收时**不得**以它为由要求改大纲。

## 卷纲必须写清

1. **四幕结构**：每幕覆盖哪几章、这一幕做什么。
2. **情绪走向**：附对应章节。
3. **核心冲突**：一句话。
4. **章数与每章一句话事件**：章名为「汉宫争艳（1）」～「汉宫争艳（10）」（大纲里括号后的工作标签不是章名）。
5. **每章的钩子/伏笔操作**：对照 `settings/foreshadowing.md`（埋/推/收）。

## 项目规则（CLAUDE.md，全程生效）

- 章节方向**只写看得见的动作和事件**；机制、动机、「这意味着什么」放每章的「设定依据（严禁写进正文）」区块。
- **精确数字不写**（身高、体重、厘米等）；罩杯字母、时长可以写。本源核心计数（【本源核心 -1】、4/5 等）是系统提示，照大纲保留。
- 称呼：「王美人」「何贵人 / 何皇后」；**不用参考文里的本名**（不用「何莲」、不用王美人本名）。玩家「试炼者」、原著角色「剧情人物」、卵子称「本源核心」。
- 原创内容标【原创提案】：**大纲 15 已有的标注照留，不新增原创情节。**
- **天赋是「魔镜真言」**（被问话必须说真话）。**「等价交换」/「契约」已全部作废，不要写回**（notes/00 骨架 G1–G13 条目里「以等价交换缔结性斗生死约」已被后续 M1–M13 推翻；第 8 章生死局按 J6 由双方约定成立，不靠系统强制）。
- 所有角色都是成年人；删去一切与孩子相关内容（大纲已删，不要补回）。

## 完成

写完 `volumes/volume-1.md` 后，用 Write 把本文件的 `status: pending` 覆盖为 `status: DONE`（不删除本文件）。
