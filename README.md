# Statistical Mechanics

统计力学可视化专题库。结构与 [pde-visualization](https://github.com/FelixJiashengFu/pde-visualization) 相同：根目录的 [专题目录](index.html)负责分类和导航，每个专题放在 `topics/<slug>/` 下，专题的 `index.html` 是可独立打开的单文件网页。

在线阅读：<https://felixjiashengfu.github.io/statistical-mechanics/>

## 专题

| 分类 | 专题 | 内容 | 入口 |
| --- | --- | --- | --- |
| 系综与配分函数 | 重力场中的理想气体 | 巨正则配分函数、`μ → μ − mgz`、气压公式 `p(z) = p(0)·e^{−βmgz}`；水墨风格交互图；需联网加载字体 | [打开交互页](topics/gravity-ideal-gas/index.html) · [说明](topics/gravity-ideal-gas/README.md) |
| 热与功 · 第一定律 | 热与功 · 测验讲解 | CHMB23 第 1–3 章，26 道选择题 + 27 道判断题，中英对照；2 份 PDF | [打开目录页](topics/heat-work-quizzes/index.html) · [说明](topics/heat-work-quizzes/README.md) |
| 熵 · 第二与第三定律 | 熵、第二定律与自由能 · 测验讲解 | 26 道选择题；26 道判断题的中文版与英文版；3 份 PDF | [打开目录页](topics/entropy-quizzes/index.html) · [说明](topics/entropy-quizzes/README.md) |
| 熵 · 第二与第三定律 | 熵、第三定律与吉布斯能 · 习题精讲 | 四道经典习题中英分步讲解：等温膨胀可逆/不可逆、冰→过热蒸汽熵变、液态汞第三定律熵、等温膨胀 ΔG；1 份 PDF | [打开目录页](topics/entropy-gibbs-worked-problems/index.html) · [说明](topics/entropy-gibbs-worked-problems/README.md) |
| 相平衡 · 相变 | 相平衡与单组分相变 · 精讲讲义 | Focus 4 课堂讲义：dG = V dP − S dT、G–T/G–P 曲线、克拉佩龙方程、水的相图与超临界流体，附 4 道典型考题；1 份 PDF | [打开目录页](topics/phase-equilibria-lecture/index.html) · [说明](topics/phase-equilibria-lecture/README.md) |
| 复习速查 | CHMB23 第 1–3 章 · 复习速查 | 一页 Cheat Sheet + 两版公式表；3 份 PDF | [打开目录页](topics/chmb23-review-sheets/index.html) · [说明](topics/chmb23-review-sheets/README.md) |

目前收录 6 个专题。

## 仓库结构

```text
statistical-mechanics/
├── index.html                  # 全部专题的分类入口
├── README.md                   # 专题索引与新增规则
└── topics/
    ├── gravity-ideal-gas/
    │   ├── index.html          # 水墨风格单文件页；需联网加载字体
    │   └── README.md           # 模型、推导、交互参数与适用范围
    ├── heat-work-quizzes/      # 热与功测验讲义（PDF）
    ├── entropy-quizzes/        # 熵与第二定律测验讲义（PDF）
    ├── entropy-gibbs-worked-problems/ # 熵、第三定律与吉布斯能习题精讲（PDF）
    ├── phase-equilibria-lecture/ # 相平衡与单组分相变精讲讲义（PDF）
    └── chmb23-review-sheets/   # Cheat Sheet 与两版公式表（PDF）
        ├── index.html          # 每个 PDF 专题：目录页 + 原始 PDF + README
        └── README.md
```

## 今后新增专题

1. 在 `topics/` 下建立简短、稳定、全小写的目录。
2. 将可独立打开的单文件网页放在该目录的 `index.html`；源码和验证材料放在本专题的 `source/`。若需联网加载外部资源，在目录卡片和说明中标注。
3. 在专题 `README.md` 写明模型、假设、交互参数、适用范围和验证方式，区分精确结论、数值近似与教学示意。
4. 讲义类专题（PDF）同样放进 `topics/<slug>/`，保留原文件名，配一个列出各 PDF 的 `index.html` 和 `README.md`；内容重复的文件不收。
5. 在根目录 `index.html` 的相应分类加入专题卡片，同时更新上面的专题表和数量。
