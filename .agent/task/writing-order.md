# writing-order

status: DONE

inputs:
  - prompts/vol-1-ch-1-prompt.md        # 唯一输入（纯净上下文，2026-10-01 重新生成）；文件末尾「待作者回答的问题」一节 writer 忽略

outputs:
  - archives/vol-1-ch-1-hangong-zhengyan-1.draft.md   # 整份重新写并覆盖；旧稿作废，不读、不在旧稿上修补

partial_path:
resume_from:
rewrite_of:
round: 1
violations:
quality_gap: 实际约 2250 字（含标点，人工估算），低于 2500；按软指标处理，未为凑字数加内容

---

## 说明

- 只读上方提示词；不读 chapters/、volumes/、notes/、start/、sexfight-database/ 及 archives/ 下任何旧文件。
- skill 文件在 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`（writing-execution.md 等），允许只读。
- 不新增章纲以外的细节道具或暗示性悬念；确需加的感官细节，按提示词「产出格式」在正文后 `---` 下逐条列出。
- 字数 2500–3000 为软指标，不为凑字数加内容；短了如实写 `quality_gap:` 行。
- 不向作者提问；需要作者判断的点写在草稿 `---` 之后，不写进正文。
- 完成后把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容）。
