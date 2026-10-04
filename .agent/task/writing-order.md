# writing-order

status: DONE

inputs:
  - archives/vol-1-ch-4-hangong-zhengyan-4.draft.md   # 上一轮稿（在此基础上小改）
  - .agent/task/vol-1-ch-4-violations.md               # 修改清单（逐条执行）
  - prompts/vol-1-ch-4-prompt.md                      # 红线参照（不重写）

outputs:
  - archives/vol-1-ch-4-hangong-zhengyan-4.draft.md   # 原地覆盖为修改后稿

partial_path:
resume_from:
rewrite_of: archives/vol-1-ch-4-hangong-zhengyan-4.draft.md
round: 2
violations: .agent/task/vol-1-ch-4-violations.md

---

## 说明

- **只按修改清单逐处小改，其余一字不动**；不重写全章，不加新情节，不动招式名、攻防流程、照录台词、章末两句。
- 改完同步更新正文后 `---` 下的「章纲外新增的细节」清单（删去随改动消失的条目），并在清单后加一节「round 2 改动」逐条对应清单编号列出（原句 → 新句）。
- 对白保持接近现代的白话；禁用词一律不出现（见提示词）。
- 不读 chapters/、volumes/、notes/、settings/、start/、sexfight-database/、novel-samples/、.agent/drafts/、archives/ 其他文件。不使用 Bash，不访问项目外路径（skill 目录 `C:\Users\sb257\.claude\skills\awesome-novel\skills\` 只读除外）。
- 不规定字数；不写 quality_gap；不向作者提问。
- 完成后把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容）。
