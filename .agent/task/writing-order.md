# writing-order

status: DONE

inputs:
  - prompts/vol-1-ch-3-prompt.md        # 唯一输入（纯净上下文，2026-10-04 纯性斗版重写）

outputs:
  - archives/vol-1-ch-3-hangong-zhengyan-3.draft.md   # 整份新写，覆盖任何旧稿（旧稿作废）

partial_path:
resume_from:
rewrite_of:
round: 1
violations:

---

## 说明

- 第 1 卷第 3 章正文（纯性斗版）。第 3 条宫女比胸按提示词的性斗段写法（fight：两步走——先照底本抄句子只换人物/场景/称呼，再按示范润色，只加描写、不改攻防流程）；其余按非性斗写法（nonfight：一句一段为主，吐槽不加引号，只跟林叁玖视角）。
- 只读上方提示词；不读 chapters/、volumes/、notes/、settings/、start/、sexfight-database/、novel-samples/、archives/ 其他文件、.agent/drafts/。底本与示范段已原样贴在提示词里。
- skill 文件在 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`（writing-execution.md 等），允许只读。不使用 Bash，不访问项目外路径（skill 目录除外）。
- 照录台词一字不改（R3 必须是：“掉一颗本源核心罢了，人还在。除非本源核心耗尽，那才是要命。”）；章末单独一行：记忆里，下一个被何贵人当众邀战的，是宋皇后。
- 禁用词一律不出现：规则怪谈、守则、遗言、魔镜真言、毒、契约、时肆、诡异、诡币、何莲、王荣、副本（叙述里）、本钱、厘米、公斤、岁。
- 作者去 AI 味口味：台词越短越像人话，删把话说满的限定语和凑词尾巴；一件事只说一遍。
- **不规定字数**：不写字数统计、不写 quality_gap。
- 不新增章纲以外的情节；正文后 `---`，其下逐条列出「章纲外新增的细节」（含自拟台词）。
- 不向作者提问。
- 完成后把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容）。
