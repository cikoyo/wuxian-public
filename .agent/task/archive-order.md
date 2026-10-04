# archive-order

status: DONE

chapter: vol-1-ch-2
slug: hangong-zhengyan-2

inputs:
  - archives/vol-1-ch-2-hangong-zhengyan-2.md          # 作者亲自微调的定稿（2026-10-04），已在正确位置。只读：一个字都不许改，包括编辑器留下的 `\~` 写法；不重新生成、不覆盖
  - .agent/drafts/vol-1-ch-2-hangong-zhengyan-2.draft.md     # AI 原版（快照来源，只读）
  - .agent/drafts/vol-1-ch-2-hangong-zhengyan-2.anti-ai.md   # 只读
  - .agent/drafts/vol-1-ch-2-hangong-zhengyan-2.review.md    # 只读
  - .agent/review/vol-1-ch-2.md                              # 只读
  - chapters/vol-1-ch-2.md
  - volumes/volume-1.md（只读）
  - notes/00-决策记录.md 中 2026-10-01、2026-10-02 各节（只读；.claude/memory/ 如规范需要记录，只能用这两处已有内容）
  - settings/character-setting/lin-sanjiu.md
  - settings/character-setting/wang-meiren.md
  - settings/character-setting/he-huanghou.md
  - settings/foreshadowing.md
  - settings/timeline.md
  - .claude/memory/
  - .agent/status.md
  - SOP（只读）：C:\Users\sb257\.claude\skills\awesome-novel\skills\ 下的 updater-archive.md、memory-format-spec.md 等 updater 引用的 skills/*.md

outputs:
  - .agent/vol-1-ch-2-draft-ai.md               # AI 原版快照（按规范，从 .agent/drafts/ 的 .draft.md 复制）
  - .agent/archiving/vol-1-ch-2.done
  - chapters/vol-1-ch-2.md                      # 只把 status 字段改为 archived，其他一个字不动
  - settings/character-setting/lin-sanjiu.md    # 状态历史追加本章结束时：在王美人身体里，醒在永巷乳斗刚结束时；带着王美人到毒发为止的记忆；本源核心 4/5；魔镜真言已生效一次；接到王美人怨魂托付「替我杀了她……杀了何贵人……」与三条遗言
  - settings/character-setting/wang-meiren.md   # 如规范要求则追加本章状态，只写已发生事实：永巷乳斗何贵人胜、踩爆王美人一颗本源核心；王美人怨魂现身托付报仇后散成血字
  - settings/character-setting/he-huanghou.md   # 如规范要求则追加本章状态，只写已发生事实：永巷乳斗胜王美人、踩爆其一颗本源核心
  - settings/foreshadowing.md                   # 只更新跨卷钩子：白雪一条「最近提及」改为 vol-1-ch-2；本卷内钩子不登记（作者定）
  - settings/timeline.md                        # 如需
  - .agent/status.md                            # last_archived: vol-1-ch-2；current_chapter: 3；phase: outline；current_step: chapter-planning；章节：vol-1-ch-3，章节状态重置为空；next_task: 第 3 章章纲，待作者开始

resume_from:

constraints:
  - 定稿文件 archives/vol-1-ch-2-hangong-zhengyan-2.md 不重新生成、不覆盖、不改一个字；规范若要求从 anti-ai 稿复制定稿，跳过这一步，以现有 archives 文件为准
  - 中间稿（.agent/drafts/ 下 .draft.md / .anti-ai.md / .review.md 等）一律不删除、不改动
  - .claude/memory/：本次不追加作者微调的规律（主会话先与作者逐条确认后再写）；其他按规范需要记的，只用 notes/00 2026-10-01、10-02 各节已有内容
  - 不读 sexfight-database/ 和 start/
  - 不改 CLAUDE.md、notes/、volumes/ 的内容；chapters/ 只改第 2 章 status 字段
  - 只写已发生的事实，不推测后续剧情
  - 与规范冲突时以本 order 为准，并在完成说明中列出冲突点
  - 完成后把本 order 的 status 改为 DONE
  - 完成后回报：每个改动文件改了什么（逐条）；任何冲突或失败原文
