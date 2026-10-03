[Carbon-check_README.md](https://github.com/user-attachments/files/33000866/Carbon-check_README.md)
# Carbon Check

> **Does it really reduce emissions?**

Carbon Check 是一个面向课堂展示的交互式低碳经济可视化网页，通过四个互动实验，从**系统边界、反弹效应、指标选择、时间尺度**四个角度重新审视“低碳”。

## 四个实验

### 01 · System Boundary｜系统边界
**你到底算了哪些碳？**

通过逐步扩大核算范围，展示生命周期评价（LCA）的系统边界思想：

```text
使用阶段 → 能源供应 → 制造 → 材料与完整生命周期
```

本模块部分数字为课堂演示用的归一化示意数据，不代表具体产品的真实生命周期排放比例。

### 02 · Rebound Effect｜反弹效应
**效率提高以后，使用量会不会增加？**

通过“效率提升”和“使用量增加”两个变量，观察单位排放与总排放的变化。

模块还加入真实研究案例：

Munyon, V. V., Bowen, W. M., & Holcombe, J. (2018).  
*Vehicle Fuel Economy and Vehicle Miles Traveled: An Empirical Investigation of Jevons’ Paradox*.  
*Energy Research & Social Science*, 38, 19–27.

DOI: https://doi.org/10.1016/j.erss.2018.01.007

网页中的案例互动用于教学演示，不应视为对所有情景的精确预测。

### 03 · Indicator Trap｜指标陷阱
**一个指标变好，是否意味着整个系统都变好？**

通过“需求活动量”和“单位碳强度”观察：

- 单位碳强度变化
- 需求活动量变化
- 绝对排放变化

核心思想：

> 单位指标改善与绝对总量下降并不是同一件事。

### 04 · Transition Carbon Debt｜转型碳债
**今天的高碳投入，需要多久才能换回未来的减排？**

通过：

- 建设阶段新增碳排放
- 每年避免的碳排放

观察累计减排与碳回本时间。

简化关系：

```text
碳回本时间
=
建设阶段新增碳排放
÷
年均避免碳排放
```

真实项目需要结合具体材料、能源结构、设备寿命和生命周期数据进行测算。

## Core Logic

四个实验最终回答四个问题：

```text
边界：我到底算了什么？
   ↓
行为：人们会怎么反应？
   ↓
指标：我到底看到了什么？
   ↓
时间：减排什么时候兑现？
```

核心观点：

> **低碳，不只是让一个数字变小，而是让整个系统的净碳排放真正下降。**

## Methodology

实验一的理论框架参考：

- ISO 14040:2006 — *Environmental management — Life cycle assessment — Principles and framework*
- ISO 14044:2006 — *Environmental management — Life cycle assessment — Requirements and guidelines*

注意：ISO 14040/14044规定的是LCA的原则、框架、要求和指南，并不规定本项目网页中的具体排放数字。

## Data Note

本项目包含两类数据：

1. **机制演示数据**：为课堂互动构造，用于说明变量关系，不代表真实项目测算结果。
2. **文献案例数据**：实验二包含基于公开研究文献的案例，用于说明效率提升与使用量变化之间的统计关系。

因此，Carbon Check 是一个**课堂交互演示原型**，不是完整的碳排放核算工具。

## Tech Stack

纯静态网页：

- HTML
- CSS
- JavaScript
- SVG

不需要后端、数据库或 API，可直接部署到 GitHub Pages。

## Project Structure

```text
Carbon-check/
├── index.html
└── README.md
```

## Run Locally

直接打开 `index.html` 即可。

或者运行：

```bash
python -m http.server
```

然后访问：

```text
http://localhost:8000
```

## GitHub Pages

1. 新建 GitHub Repository。
2. 上传 `index.html` 和 `README.md`。
3. 进入 `Settings → Pages`。
4. 选择 `Deploy from a branch`。
5. 选择 `main / root`。
6. 保存并等待部署完成。

## Online Demo

https://jackliudesca.github.io/Carbon-check/

## Classroom Presentation

推荐流程：

```text
提出问题
   ↓
实验一：系统边界
   ↓
实验二：反弹效应
   ↓
实验三：指标陷阱
   ↓
实验四：转型碳债
   ↓
结论：什么才叫真正的低碳？
```

展示方式：

> **PPT提出问题 → 手机扫码 → 现场操作网页 → 观察结果 → 回到PPT总结**

## Design Philosophy

Carbon Check 不直接回答：

> “某项技术是不是绿色？”

而是提出：

> **“我们看到的‘低碳’，究竟是真实的系统性减排，还是某一个边界、某一个指标、某一个时间段里看起来更低碳？”**

**Boundary · Behavior · Indicator · Time**

---

Made for educational and classroom presentation.
