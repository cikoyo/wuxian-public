# archive-order

status: DONE

chapter: vol-1-ch-1
slug: hangong-zhengyan-1

inputs:
  - archives/vol-1-ch-1-hangong-zhengyan-1.anti-ai.md   # 作者逐条审定的定稿（2026-10-01）。正文 = 第 1 行至第 89 行（「【剧情世界：汉宫争艳，载入中。】」），即第一个 `\n---` 分隔线之前；分隔线之后的修改报告、writer 字数与新增细节清单、验收节、待答问题全部不属于正文
  - archives/vol-1-ch-1-hangong-zhengyan-1.draft.md     # AI 原版（快照 / diff 基线来源）
  - archives/vol-1-ch-1-hangong-zhengyan-1.review.md
  - chapters/ 下第 1 章章纲（只读）
  - volumes/volume-1.md（只读）
  - notes/00-决策记录.md 的「第 1 章正文的回复（2026-10-01）」一节   # 本章作者反馈要点，按 memory-format-spec 记入 .claude/memory/ 对应文件（本项只读此节）
  - settings/character-setting/lin-sanjiu.md
  - settings/foreshadowing.md
  - settings/timeline.md
  - .claude/memory/
  - .agent/status.md
  - SOP（只读）：C:\Users\sb257\.claude\skills\awesome-novel\skills\ 下的 updater-archive.md、memory-format-spec.md 等 updater 引用的 skills/*.md

outputs:
  - archives/vol-1-ch-1-hangong-zhengyan-1.md   # 定稿正文：原样复制上述第 1–89 行，一个字不改；不加标题行（作者定：正文首行不写章名）；不含报告、验收节、字数与新增细节清单
  - .agent/vol-1-ch-1-draft-ai.md               # AI 原版快照（按规范）
  - .agent/archiving/vol-1-ch-1.done
  - settings/character-setting/lin-sanjiu.md    # 状态历史追加本章结束时：已抽到 D 级「初级魅魔血脉」、D 级「魔镜真言」一级；被载入【剧情世界：汉宫争艳】
  - settings/foreshadowing.md                   # 只更新跨卷钩子的「最近提及」等状态；作者定：本卷内钩子不登记
  - settings/timeline.md                        # 如需
  - .claude/memory/ 对应记忆文件
  - .agent/status.md                            # last_archived: vol-1-ch-1；章节状态：全部完成（archiving）；current_chapter: 2；phase: outline；current_step: chapter-planning；next_task: 第 2 章章纲，待作者开始

resume_from:

constraints:
  - 中间文件（.draft.md / .anti-ai.md / .review.md 等）一律不删除、不改动
  - 不读 sexfight-database/ 和 start/
  - 不改 CLAUDE.md、notes/、volumes/、chapters/ 的内容
  - 只写已发生的事实，不推测后续剧情
  - 与规范冲突时以本 order 为准，并在完成说明中列出冲突点
  - 完成后回报：定稿文件字数；每个改动文件改了什么（逐条）；任何冲突或失败原文
