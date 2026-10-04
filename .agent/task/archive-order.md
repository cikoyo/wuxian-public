# archive-order

status: DONE

chapter: vol-1-ch-3
slug: hangong-zhengyan-3

skills_path: C:\Users\sb257\.claude\skills\awesome-novel\skills\   # updater-archive.md、memory-format-spec.md 等 SOP 在此全局目录（只读）

背景：本书 2026-10-04 起为纯性斗文；「本源核心」已全书改名「阴珠」，「本源精华」改名「阳精」。新写入的任何文字一律用「阴珠」「阳精」。

inputs:
  - archives/vol-1-ch-3-hangong-zhengyan-3.md          # 作者亲自微调的定稿，已在正确位置。只读：一个字都不许改；不重新生成、不覆盖
  - .agent/drafts/vol-1-ch-3-hangong-zhengyan-3.draft.md     # AI 原版（快照来源，只读）
  - .agent/drafts/vol-1-ch-3-hangong-zhengyan-3.anti-ai.md   # 只读
  - .agent/drafts/vol-1-ch-3-hangong-zhengyan-3.review.md    # 只读
  - chapters/vol-1-ch-3.md
  - volumes/volume-1.md（只读）
  - settings/character-setting/lin-sanjiu.md
  - settings/character-setting/wang-meiren.md
  - settings/character-setting/he-huanghou.md
  - settings/foreshadowing.md
  - settings/timeline.md
  - .agent/status.md
  - SOP（只读）：C:\Users\sb257\.claude\skills\awesome-novel\skills\ 下 updater 引用的 skills/*.md

outputs:
  - .agent/vol-1-ch-3-draft-ai.md               # AI 原版快照（按规范，从 .agent/drafts/ 的 .draft.md 复制）
  - .agent/archiving/vol-1-ch-3.done
  - chapters/vol-1-ch-3.md                      # 只把 status 字段改为 archived，其他一个字不动
  - settings/character-setting/lin-sanjiu.md    # 状态历史追加本章（只写已发生事实）：女医讲宫中规矩；在掖庭旁观宫女比胸，输家的阴珠被赢家当场踩碎；用金簪差遣侍女跑腿传话
  - settings/foreshadowing.md                   # 只更新跨卷钩子；本章无跨卷钩子则不动
  - settings/timeline.md                        # 按需
  - .agent/status.md                            # last_archived: vol-1-ch-3；current_chapter: 4；phase: outline；current_step: chapter-planning；章节：vol-1-ch-4，章节状态重置为空；next_task: 第 4 章章纲

resume_from:

constraints:
  - 定稿文件 archives/vol-1-ch-3-hangong-zhengyan-3.md 不重新生成、不覆盖、不改一个字；规范若要求从 anti-ai 稿复制定稿，跳过这一步，以现有 archives 文件为准
  - 中间稿（.agent/drafts/ 下 .draft.md / .anti-ai.md / .review.md）一律不删除、不改动
  - .claude/memory/：本次不追加任何内容（作者这次只删了重复的约定台词，不另记）
  - wang-meiren.md、he-huanghou.md：本章两人未出场交手，不追加（规范若强制要求，只写一句已发生事实）
  - 不读 sexfight-database/、start/、notes/
  - 不改 CLAUDE.md、notes/、volumes/；chapters/ 只改第 3 章 status 字段
  - 只写已发生的事实，不推测后续剧情；不写精确数字、不用「本钱」
  - 与规范冲突时以本 order 为准，并在完成说明中列出冲突点
  - 完成后把本 order 的 status 改为 DONE
  - 完成后回报：每个改动文件改了什么（逐条，每个一行）；任何冲突或失败原文
