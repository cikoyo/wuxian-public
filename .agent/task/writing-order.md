# writing-order

status: DONE

inputs:
  - prompts/vol-1-ch-2-prompt.md        # 唯一输入（纯净上下文）；文件末尾「待作者回答的问题」一节 writer 忽略，上文已按默认写好

outputs:
  - archives/vol-1-ch-2-hangong-zhengyan-2.draft.md   # 覆盖同名旧文件（若有）

partial_path:
resume_from:
rewrite_of:
round: 1
violations:

---

## 说明

- 本轮是第 2 章正文**全新重写**（章纲第三版）。上一版正文作废；`.agent/drafts/` 下旧稿**不读**。
- 只读上方提示词；不读 chapters/、volumes/、notes/、settings/、start/、sexfight-database/、novel-samples/ 及 archives/、.agent/drafts/ 下任何文件。底本原文与示范段已原样贴在提示词里。
- skill 文件在 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`（writing-execution.md 等），允许只读。不使用 Bash，不访问项目外路径（skill 目录除外）。
- 两种写法：第 2 条乳斗记忆按提示词「写作规范 A」（性斗段，两步走：先照底本抄句子、只换人物/场景/称呼并执行【改】，再按示范手法润色，不改招式与攻防流程、不加回合）；其余按「写作规范 B」（非性斗段，一句一段为主，吐槽不加引号）。
- 提示词「约束红线·照录」各行一字不改；禁用词一律不出现。
- **不规定字数**：不写字数统计、不写 quality_gap。永远不为凑字数加内容。
- 不新增章纲以外的情节；贴着视角的感官细节可以写，按提示词「产出格式」在正文后 `---` 下逐条列出「章纲外新增的细节」，再列「底本抄取对照」（5 句以上，标行号），最后「待作者回答的问题」（每条附建议）。
- 不向作者提问。
- 完成后把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容）。
