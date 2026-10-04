# reader-review-order

status: DONE

inputs:
  - archives/vol-1-ch-4-hangong-zhengyan-4.draft.md     # round 2 修改后稿（`---` 后有「round 2 改动」逐条对照）
  - .agent/task/vol-1-ch-4-violations.md                 # 上轮你给出的修改点 + anti-ai 同意项
  - archives/vol-1-ch-4-hangong-zhengyan-4.review.md     # 你上一轮的评审（原地覆盖为复审结论，保留上轮主要意见）
  - prompts/vol-1-ch-4-prompt.md                         # 红线参照
  - archives/vol-1-ch-3-hangong-zhengyan-3.md            # 掉阴珠段对照
  - archives/vol-1-ch-2-hangong-zhengyan-2.md            # 掉阴珠段对照

outputs:
  - archives/vol-1-ch-4-hangong-zhengyan-4.review.md     # 复审：通过 / 不通过；只核上轮不通过项与改动是否引入新硬伤

---

## 说明

- round 2 复审：核对修改清单 A（掉阴珠段近同句）、B（盘坐接不上、「自己」指代、边走边脱）是否解决；改动处是否引入新的读感硬伤；禁用词与红线是否仍全过。
- 不重新全面评审，不提新表达层建议（除非是新引入的硬伤）。
- skill 文件在 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`，允许只读。禁止读 `sexfight-database/`、`start/`、`novel-samples/`、`.agent/drafts/`。不使用 Bash，不访问项目外路径。不向作者提问。
- 完成后把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容）。
