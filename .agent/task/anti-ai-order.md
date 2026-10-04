# anti-ai-order

status: DONE

inputs:
  - archives/vol-1-ch-3-hangong-zhengyan-3.draft.md     # writer 稿（2026-10-04 纯性斗版新稿）；`---` 之后是新增细节，不算正文
  - prompts/vol-1-ch-3-prompt.md                         # 同源提示词（验收依据）
  - .claude/knowledge/anti-ai.md                         # 顶部「WUXIAN 作者覆盖」优先于下文所有条目
  - .claude/memory/
  - settings/writing-style.md
  - settings/style-profiles/nonfight.md                  # 非性斗段（含「原作不会出现的写法」反例表）
  - settings/style-profiles/fight.md                     # 只管宫女比胸段
  - CLAUDE.md                                            # 第三节第 7 条（2026-10-01 放宽）

outputs:
  - archives/vol-1-ch-3-hangong-zhengyan-3.anti-ai.md   # 正文部分原样复制 writer 稿正文（一字不改）；`---` 之后：问题清单 + 验收违反报告节（verdict PASS/FAIL）+ writer 稿 `---` 后各节原样转录

round: 1

---

## 说明

- **只列问题、不改稿**（以 anti-ai.md 顶部作者覆盖为准）：`.anti-ai.md` 正文与 writer 稿正文逐字一致；意见写成编号清单（每条：原句 → 问题类型 → 建议改法 → 理由）。
- 不当 AI 味：拟声词、口语化重复描写、倒吸凉气、像/仿佛/如同；情绪标签、心理说明、动作来由、比喻、总结句不列为问题。拿不准的标「存疑」。
- **比胸段是照底本抄取的原文句子**（金瓶梅 L242–L244 改写：「酥胸对碰，针尖对麦芒」「一阵电流传遍全身」「如流星锤一般势大力沉，夹带风声」「对碰不过三个回合……败下阵来」等）——底本句子与骂词不列改动；只看润色加的部分。性斗段叫声、拟声不当 AI 味。
- **重点找**：碎句定格、动作三连拍、机械套句式、自造对称俏皮句、藏关键词的句子、把话说满的限定语与凑词尾巴、同一件事说两遍、相邻段重复、前后对不上（如侍女随行后在掖庭的去向）。对照 nonfight.md 反例表。
- 其他可列：设定复述、精确数字、冗余头衔、技术/临床词、机制解释、解释性台词。
- **照录不列改动**：R1a、R1b、R2、R3（“掉一颗本源核心罢了，人还在。除非本源核心耗尽，那才是要命。”）、T1/T2/T2b/T4/T5、R4、R5、起哄中间三句、宫女起因与对骂台词、「听明白了吗？」「诺。」、章末钩子「记忆里，下一个被何贵人当众邀战的，是宋皇后。」。若有问题只标「存疑·照录」。
- verdict 只按提示词红线判：照录逐字在场；禁用词（规则怪谈、守则、遗言、魔镜真言、毒、契约、时肆、诡异、诡币、何莲、王荣、叙述里的副本、本钱、厘米、公斤、岁）；非性斗段只跟林叁玖视角；不出系统提示；无遗言/魔镜真言/「怕」/「信不过」；不写第 4 章过程；不取 L245 第二挑战者；比胸隔衣、不加底本没有的招式；林叁玖观战不写情欲与羞耻；章末钩子单独一行。
- 不规定字数：不评字数；文风卡数值偏离只记录、不判 FAIL。
- writer 列出的新增细节原样转录，不删不改。
- skill 文件在 `C:\Users\sb257\.claude\skills\awesome-novel\skills\`，允许只读。禁止读 `sexfight-database/`、`start/`、`novel-samples/`、`.agent/drafts/`。不使用 Bash，不访问项目外路径（skill 目录除外）。
- 不向作者提问；问题要少。
- 完成后把本 order 的 `status: pending` 覆盖为 `status: DONE`（保留其余内容）。
