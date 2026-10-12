# Statistical Mechanics

统计力学可视化专题库。结构与 [pde-visualization](https://github.com/Uugyfgyb/pde-visualization) 相同：根目录的 [专题目录](index.html)负责分类和导航，每个专题放在 `topics/<slug>/` 下，专题的 `index.html` 是可独立打开的单文件网页。

## 专题

| 分类 | 专题 | 内容 | 入口 |
| --- | --- | --- | --- |
| 系综与配分函数 | 重力场中的理想气体 | 巨正则配分函数、`μ → μ − mgz`、气压公式 `p(z) = p(0)·e^{−βmgz}`；水墨风格交互图；需联网加载字体 | [打开交互页](topics/gravity-ideal-gas/index.html) · [说明](topics/gravity-ideal-gas/README.md) |

目前收录 1 个专题。

## 仓库结构

```text
statistical-mechanics/
├── index.html                  # 全部专题的分类入口
├── README.md                   # 专题索引与新增规则
└── topics/
    └── gravity-ideal-gas/
        ├── index.html          # 水墨风格单文件页；需联网加载字体
        └── README.md           # 模型、推导、交互参数与适用范围
```

## 今后新增专题

1. 在 `topics/` 下建立简短、稳定、全小写的目录。
2. 将可独立打开的单文件网页放在该目录的 `index.html`；源码和验证材料放在本专题的 `source/`。若需联网加载外部资源，在目录卡片和说明中标注。
3. 在专题 `README.md` 写明模型、假设、交互参数、适用范围和验证方式，区分精确结论、数值近似与教学示意。
4. 在根目录 `index.html` 的相应分类加入专题卡片，同时更新上面的专题表和数量。
