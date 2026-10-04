# archive-order

status: DONE

chapter: vol-1-ch-4
slug: hangong-zhengyan-4

skills_path: C:\Users\sb257\.claude\skills\awesome-novel\skills\   # updater-archive.md、memory-format-spec.md 等 SOP 在此全局目录（只读）

背景：本书 2026-10-04 起为纯性斗文；「本源核心」已全书改名「阴珠」，「本源精华」改名「阳精」。新写入的任何文字一律用「阴珠」「阳精」。本章招式名为十字点樱、火烧连营、泰山压顶、巨灵开山；何皇后名乳「赤焰乳」、名穴「缠丝锁」（已在卡中）。

inputs:
  - archives/vol-1-ch-4-hangong-zhengyan-4.md          # 作者确认的定稿，已在正确位置。只读：一个字都不许改；不重新生成、不覆盖
  - .agent/drafts/vol-1-ch-4-hangong-zhengyan-4.draft.md     # AI 原版（快照来源，只读）
  - .agent/drafts/vol-1-ch-4-hangong-zhengyan-4.anti-ai.md   # 只读
  - .agent/drafts/vol-1-ch-4-hangong-zhengyan-4.review.md    # 只读
  - chapters/vol-1-ch-4.md
  - volumes/volume-1.md（只读）
  - settings/character-setting/lin-sanjiu.md
  - settings/character-setting/he-huanghou.md
  - settings/foreshadowing.md
  - settings/timeline.md
  - .agent/status.md
  - SOP（只读）：C:\Users\sb257\.claude\skills\awesome-novel\skills\ 下 updater 引用的 skills/*.md

outputs:
  - .agent/vol-1-ch-4-draft-ai.md               # AI 原版快照（按规范，从 .agent/drafts/ 的 .draft.md 复制）
  - .agent/archiving/vol-1-ch-4.done
  - chapters/vol-1-ch-4.md                      # 只把 status 字段改为 archived，其他一个字不动
  - settings/character-setting/he-huanghou.md   # 状态历史追加本章（只写已发生事实）：长秋宫请安时当众邀战宋皇后、以后位作赌；比斗中翻盘获胜；当场踩碎宋皇后一颗阴珠。赤焰乳、缠丝锁已在卡中，不重复添加
  - settings/character-setting/lin-sanjiu.md    # 状态历史追加本章：在场观战
  - settings/timeline.md                        # 第 4 章一行按定稿更新（只写已发生事实）
  - settings/foreshadowing.md                   # 只更新跨卷钩子；本章无跨卷钩子则不动
  - .agent/status.md                            # last_archived: vol-1-ch-4；current_chapter: 5；phase: outline；current_step: chapter-planning；章节：vol-1-ch-5，章节状态重置为空；next_task: 第 5 章章纲（作者在另一个对话进行）

resume_from:

constraints:
  - 定稿文件 archives/vol-1-ch-4-hangong-zhengyan-4.md 不重新生成、不覆盖、不改一个字；规范若要求从 anti-ai 稿复制定稿，跳过这一步，以现有 archives 文件为准
  - 中间稿（.agent/drafts/ 下 .draft.md / .anti-ai.md / .review.md）一律不删除、不改动
  - 宋皇后不建角色卡（只在本章出场）；wang-meiren.md 不改
  - .claude/memory/：本次不追加任何内容
  - 不读 sexfight-database/、start/、notes/
  - 不改 CLAUDE.md、notes/、volumes/；chapters/ 只改第 4 章 status 字段
  - 只写已发生的事实，不推测后续剧情；不写精确数字、不用「本钱」
  - 不写 last_volume_completed（由 novel-agent 判定）
  - 与规范冲突时以本 order 为准，并在完成说明中列出冲突点
  - 完成后把本 order 的 status 改为 DONE
  - 完成后回报：每个改动文件改了什么（逐条，每个一行）；任何冲突或失败原文
