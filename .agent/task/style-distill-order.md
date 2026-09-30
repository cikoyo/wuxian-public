# style-distill-order

status: DONE

inputs:
  - settings/writing-style.md
  - settings/style-profiles/fight.md
  - settings/style-profiles/analysis/general.md
  - settings/style-profiles/analysis/fight.md
  - novel-samples/间谍过家家：新.txt

outputs:
  - settings/writing-style.md
  - settings/style-profiles/fight.md
  - settings/style-profiles/analysis/general.md
  - settings/.style-versions/

resume_from:

---

## 说明（novel-agent → style-distiller）：作者对画像的反馈，按此修订，不重新全量蒸馏

作者 2026-09-28 对「作者画像」三个问题的回答：

1. **精确数字尽量不写**：身高厘米、体重斤数、罩杯字母、「几厘米」「几分钟」之类的精确数值，新书里尽量不用。请在主卡和性斗卡的硬约束里写明这一条（用对比、动作、反应代替数字）。量化层里原先照实记录的「样本爱用数字」要标注为「不继承」。
2. **身体细节向《间谍过家家：新》靠**：作者认为这篇「身体细节写得更实，值得学习」。只学这一点——身体部位的具体描写（部位、动作、反应写得实、写得具体）。**句法（句长、短句比例、省略号用法）仍按六篇平均，不向这篇靠**。请从这篇里补充几条身体细节写法的例句到性斗卡的声音层（原文摘录，删节处标「……」）。
3. **只学写法，不学剧情套路**：情敌争夫、正宫与小三等母题不带进新书。在分析稿里把第 3 个问题标为已确认。

其他：
- 修订前先把当前两张卡备份到 `settings/.style-versions/`（文件名带 2026-09-28）。
- **不要读 `novel-samples/sexfight-database/` 目录**，那是另外的素材库，不是文风样本。
- 画像中「有三件事想请你拍板」一节，改写为「作者已确认」的结论。
- 完成后把本 order 覆盖为 `status: DONE`，回报改了哪些条目。
