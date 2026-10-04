# writing-order

status: DONE

inputs:
  - prompts/vol-1-ch-3-prompt.md        # 唯一输入（纯净上下文）；文件末尾「待作者回答的问题」一节 writer 忽略，上文已按默认写好

outputs:
  - archives/vol-1-ch-3-hangong-zhengyan-3.draft.md

partial_path:
resume_from:
rewrite_of:
round: 1
violations:

---

## 说明

- 第 1 卷第 3 章正文，**非性斗章**，全章按提示词的非性斗写法（nonfight：一句一段为主，叙述写完整长句，吐槽不加引号，只跟林叁玖视角）。
- 只读上方提示词；不读 chapters/、volumes/、notes/、settings/、start/、sexfight-database/、novel-samples/ 及 archives/、.agent/drafts/ 下任何文件。示范段已原样贴在提示词里。
- skill 文件在 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`（writing-execution.md 等），允许只读。不使用 Bash，不访问项目外路径（skill 目录除外）。
- 提示词「约束红线·照录」各行一字不改（R3 必须是：“掉一颗本源核心罢了，人还在。除非本源核心耗尽，那才是要命。”）；遗言用「遗言第几条。」单起一行 + 下一行「」原文；【】只给系统提示；章末单独一行结论句。禁用词一律不出现。
- 作者的去 AI 味口味：台词越短越像人话，删把话说满的限定语和凑词尾巴；一件事只说一遍；不写碎句定格、动作三连拍、机械套句式、自造对称俏皮句、谜语句。
- **不规定字数**：不写字数统计、不写 quality_gap。永远不为凑字数加内容。
- 不新增章纲以外的情节；正文后 `---`，其下逐条列出「章纲外新增的细节」（含你自拟的台词），最后「待作者回答的问题」（每条附建议）。
- 不向作者提问。
- 完成后把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容）。
