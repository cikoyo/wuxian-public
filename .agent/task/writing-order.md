# writing-order

status: DONE

inputs:
  - prompts/vol-1-ch-1-prompt.md        # 唯一输入（纯净上下文）；文件末尾「待作者回答的问题」一节 writer 忽略

outputs:
  - archives/vol-1-ch-1-hangong-zhengyan-1.draft.md

partial_path:
resume_from:
rewrite_of:
round: 1
violations:
quality_gap: 正文约 2100 字，低于 2500 软下限；按提示词「写不到不补内容」未补写

---

## 说明

- 只读上方提示词；不读 chapters/、volumes/、notes/、start/、sexfight-database/ 及其他 archives/ 文件。
- skill 文件在 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`（writing-execution.md 等），允许只读。
- 不向作者提问；需要作者判断的点写在草稿文件之外（回报里说明），不写进正文。
- 完成后把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容）；如有字数降级，写 `quality_gap:` 行。
