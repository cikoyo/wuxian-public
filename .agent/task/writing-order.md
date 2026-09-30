# writing-order

status: DONE
quality_gap: 正文约 1950 字（手工估算），略低于 2000 软下限；四个场景与全部逐字照录行已覆盖，按指示未为凑字数加内容。

inputs:
  - prompts/vol-1-ch-2-prompt.md        # 唯一输入（纯净上下文）；文件末尾「待作者回答的问题」一节 writer 忽略

outputs:
  - archives/vol-1-ch-2-hangong-zhengyan-2.draft.md

partial_path:
resume_from:
rewrite_of:
round: 1
violations:

---

## 说明

- 只读上方提示词；不读 chapters/、volumes/、notes/、start/、sexfight-database/ 及 archives/ 下任何文件。
- skill 文件在 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`（writing-execution.md 等），允许只读。
- 林叁玖的吐槽不加引号，直接写进叙述；提示词里「逐字照录」的各行一字不改。
- 不新增章纲以外的情节、道具或暗示性悬念；贴着视角的感官细节可以写，按提示词「产出格式」在正文后 `---` 下逐条列出。
- 字数 2000–2500 为软指标，不为凑字数加内容；短了在本 order 写 `quality_gap:` 行如实说明。
- 不向作者提问；需要作者判断的点写在草稿 `---` 之后「待作者回答的问题」（每条附建议），不写进正文。
- 完成后把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容）。
