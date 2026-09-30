# reader-review-order

status: DONE

inputs:
  - archives/vol-1-ch-1-hangong-zhengyan-1.anti-ai.md   # 正文（只评正文部分，文件后半的修改报告/验收节不算正文）
  - chapters/vol-1-ch-1.md                               # 章纲（对照用）
  - CLAUDE.md                                            # 项目规则：第三节第 7 条「正文做减法」、第四节称呼

outputs:
  - archives/vol-1-ch-1-hangong-zhengyan-1.review.md     # 评审报告（结论：通过 / 不通过 + 主要意见；若不通过写明应回到哪个环节修）

---

## 说明

- 苛刻读者验收：先沉浸阅读再逐项评价。
- 评价时遵守项目规则：作者偏好做减法、宁可留白；**比喻、总结句由作者判断，不以此为不通过理由**；字数 2500–3000 是软指标，不为凑字数建议加内容（可以指出篇幅，但不作为单独不通过理由）；不建议新增章纲以外的情节。
- skill 文件在 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`，允许只读。禁止读 `sexfight-database/`、`start/`。
- 不向作者提问；需要作者判断的点写在评审报告末尾「## 待作者回答的问题」。
- 完成后把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容）。
