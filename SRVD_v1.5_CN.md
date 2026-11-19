# 结构递归存续动力学（Structure Recursive Viability Dynamics，SRVD） {.unnumbered .unlisted}

***

**梁瑞峰** | ORCID: [0009-0002-8575-7127](https://orcid.org/0009-0002-8575-7127) | 2026 | v1.5 · 五卷合订（卷Ⅰ / 卷Ⅱ / 卷Ⅲ / 卷Ⅳ / 卷Z） | fineflowerrain@gmail.com

<!-- imprint-begin -->
DOI（概念，始终指向最新版本）：[10.5281/zenodo.20130775](https://doi.org/10.5281/zenodo.20130775)

本版 DOI（v1.5）：[10.5281/zenodo.24365889](https://doi.org/10.5281/zenodo.24365889)

许可：CC BY 4.0（[creativecommons.org/licenses/by/4.0](https://creativecommons.org/licenses/by/4.0/)）

复现包：[10.5281/zenodo.24349831](https://doi.org/10.5281/zenodo.24349831)
<!-- imprint-end -->

***

**声明。** 全部方程与预测均为待检验的假说；已有的数学结果仅限于所声明的简化模型。文中所有数值算例、量级估计与数值表均为**示意性模型演算**，用于演示读数与判据的用法，不对应任何实测系统；标注来源的实证数据不在此列。各卷自成体系：所用变量、方程、判据与适用条件均在卷内给出或就地说明。

| 卷 | 标题 | 卷内特有的补充声明 | 证据标签出处 |
| :---- | :----------------- | :------------------------ | :----------- |
| **卷Ⅰ** | 理论核心 | $V_{\mathrm{obj}}$ 的绝对值**目前**无法精确测量——缺的是标定与观察窗协议，不是定义本身；模型未经临床或实证校准，不产生任何个体层面的预后读数 | 随文标注，本卷不设集中定义表 |
| **卷Ⅱ** | 持久结构的演化：复杂度攀升的热力学框架 | 全部结论按 §2.5 的四级证据标签标注强度，未加标签者属叙述与举例 | §2.5 |
| **卷Ⅲ** | 压缩智能与认知演化：离线编译计算、人类因果增量与物理嵌入的边界 | 结论按 §1.2 的四级证据标签标注强度，未加标签者属叙述与举例 | §1.2 |
| **卷Ⅳ** | 解码器博弈论与对齐工程 | 结论按 §1.2 的四级标签标注强度，未加标签者属叙述与举例 | §1.2 |
| **卷Z** | 现实映射词典：数学式与叙事 | 词典体，可独立阅读：不产生新的数学结论，每条条目的证据等级都不高于它所叙述的形式化条目；凡叙事强于所叙述的条目，以条目为准 | 「第零章　使用说明」 |

***

<!-- VOLUME Ⅰ ｜ 理论核心 -->
## 卷Ⅰ　理论核心

> **本卷＝卷Ⅰ。**

**本卷主张。** 持久结构的存续可以写成一本可核算的账：净有效因果信息 $I_{\mathrm{net}}$ 的累积率与基线折旧率 $\gamma_0$ 相抵，决定存续势 $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ 的平衡位置；同一物理信号经不同解码器可记为 $I^{+}$、$I^{-}$ 或 $I^{0}$，账的记法随解码器而变；主动相实际优化的是 $V^{\mathrm{val}}$——由虚拟信号 $V^{\mathrm{virt}}$ 度量的价值存续势——而不是 $V_{\mathrm{obj}}$。沿这条线索，本卷给出变量宪法与量纲记账、存续势三重分裂、一个平衡点与鞍结分岔阈值均有闭式的约化 $I$–$V$ 子系统、11 条各附反驳条件的框架命题，以及一套可执行的预注册证伪协议。

**使用边界。** 上述各项按四级证据等级（【定理】【命题】【候选推论】【假说】）逐条标注，前提与失效条件写在原处；文中数值与量级一律为示意性模型演算，未经临床或实证校准，不产生任何个体层面的预后读数。完整的使用边界、测量契约与伦理约束见 §10.5。

***

**引言**

进入严格论证之前，先用两个对象直观展示核心概念。

一座荒岛。一人、一条巨蟒、一头野猪。

野猪先遇见人。它从未见过这个物种：个头太大，不像猎物；动作太慢，不像威胁。在它的解码器里，人只是一团无关的噪声——**$I^0$**。它无视这个人，继续悠然觅食。

人同时发现野猪：难以直接捕获，得不到正效信息 $I^+$；獠牙锋利，存在负效信息 $I^-$ 的风险。他选择最安全的做法——爬上树。

树冠深处，早已盘踞着一条巨蟒。它把人和野猪同时收入视野：野猪是一团高价值蛋白质，是优质的 $I^+$；人是陌生物种，正效还是负效并不明朗，非极度饥饿时不列入优先菜单。

野猪最先嗅到蛇的气味，恐惧攫住它：它的 **$T_{\mathrm{pred}}$**，即内生时间视界，急剧收缩，只剩此刻的生死。它狂奔一公里，危机感消散，又低下头拱土觅食。对它而言，威胁一旦离开感知范围，就等于从未存在。

人滑下树逃离。但逃出生天后，他的 **$T_{\mathrm{pred}}$** 没有停在“此刻安全”，而是继续向前延伸——延伸到明天、后天，以及更远的将来。在他预测的未来里，蛇还在，致命威胁还在。

对野猪而言，未来并不存在；而对人而言，未来已经开始影响现在。

于是人行动起来，$I_{\mathrm{net}}$（净有效因果信息）的高阶递归被启动。“陷阱”“长矛”“藤索”——这些尚未存在于物理世界的对象，在他的知识积累与未来预演中成形，随后被他制作出来。他也意识到，短兵相接时逃跑或搏斗都会消耗巨大体力，一旦触及 $E_{\mathrm{thresh}}$（损伤触发阈值）就完了，因此提前用闲时的 $E_{\mathrm{eff}}$ 锻炼身体，换取未来更多可用的体力。

第二天，蛇找到野猪，一场没有悬念的捕食发生了。第三天，人找到蛇窝，偷走蛇蛋。

蛇返回巢穴时，发现人正在享用最后几个蛇蛋。在蛇的解码器里，人从陌生物种骤然升级为直接威胁自身基因 PS 存续的强 $I^-$，它立刻发起攻击。迎接它的是一套远超其认知模型的复杂战术与武器。蛇被砍伤，拖着断尾遁走；人也在搏斗中身受致命伤。

弥留之际，他想到家乡的亲人、未酬的壮志，以及那条让他 **$V_{\mathrm{s}}$** 即将归零的蛇。在剩余的可操作性空间里，他强忍剧痛，在岩石上刻下遗嘱：写下对亲人想说却未说出的话，分配遗产，并请亲友替他杀死那条蛇。

刻完最后一笔，他已经没有力气再挪动半步。伤口继续失血，饥饿与寒冷一并消耗他剩下的资源：当前因果通道对存续的维持贡献 $V_{\mathrm{c}}$ 一路下降，并持续侵蚀尚未耗尽的结构存续资源 $V_{\mathrm{s}}$。当客观存续势 $V_{\mathrm{obj}}$ 跌破可维持阈值，而剩余可操作状态空间中又不存在足以把它拉回的可行方案时，他能做的事情急剧收窄——窄到只剩呼吸。天亮之前，他死于失血与失温。结构损耗先一步走完了它的账：$T_{\mathrm{struct}}$ 在他还没有想清楚之前就已经用尽。

三个月后，另一个人发现了刻着遗嘱的岩石。遗嘱进入法律程序，那带有亲笔署名和特殊笔迹的文字信息开始代替他继续对物理世界施加因果效力 $I_{\mathrm{net}}$，执行未竟之事：化解与亲人的隔阂，让家族 PS 获得财富，为其基因 PS 争取更多未来可达空间。亲友替他猎杀了那条蛇，并在荒岛上为他立碑。他的姓名、肖像、事迹与遗愿被保留下来，个人 PS 化作模因 PS，在物理世界继续存续，并尽可能延长自身的 **$T_{\mathrm{pred}}$**。

同一组条件，在一个非生命的对象上可以看得更清楚。海岸线上有一座灯塔，服役一百四十年。它的价值从来不在砖石本身，而在于那条被它照亮的航线：每晚固定的闪光周期，是它与所有过往船只之间的一份隐性协议。后来航线改道，货运转移到更远的深水码头，照明功能不再对应任何真实的存续需求；盐雾侵蚀使钢筋锈胀、砖石盐析，年度维护预算从“例行修缮”滑向“整体加固”，再滑向“拆除重建”。评估报告给出的重建成本，超出了主管机构在一个财政周期内可动员的全部资源；分年实施又要求灯塔连续停用数年，而停用期间的替代方案同样需要新的资本开支。修复方案于是超出了可操作空间——所有可行方案的成本都落在可用预算之外。灯塔按预先写定的程序停运：熄灯、拆除透镜与旋转机构、封存楼梯，通报海事部门更新航图，把灯志、光学图纸与守塔人日志移交地方档案馆。它被列入遗址名录，夏天有游客上来拍照，讲解牌上写着它的闪光周期与那套协议的由来。砖石仍在，但存续方式换了一种拓扑：从“持续输出光信号的功能结构”，变成“被反复读取的历史结构”。这是结构在给定能量与时间约束下，把剩余的可操作空间从“维持原功能”切换到“以另一种方式继续被读取”。

***

在这个故事里，野猪、巨蟒、人、长矛、遗嘱、金钱、后代，都不是真正的主角。**真正的主角是：在一定能量约束下，维持自身有序拓扑特征的负熵构型——持久结构**（Persistent Structure, PS）。

### 什么是持久结构？

宇宙服从熵增定律，一切最终趋向无序。然而在这不可逆的洪流中，却不断涌现出逆流而上的有序岛屿：晶体、恒星、细胞、神经网络、语言、制度、文明，以及一份承载含义的遗嘱。这些看似风马牛不相及的事物拥有一个共同本质：它们都是在一定能量支撑下、能够从背景噪声中识别出来的特定有序信息结构。SRVD（Structure Recursive Viability Dynamics）认为，当宇宙中任何对象展现出可辨识的有序特征时，其存续与消亡便可纳入同一套跨尺度分析框架：

$$
V \approx \frac{I \cdot T}{E} \tag{I-0.1}
$$

**存续势 = 信息 × 时间 ÷ 能量代价。**

> **$V$ 是存续势的正式记号（单写 $V$ 即 $V_{\mathrm{obj}}$）；$V\approx I\cdot T/E$ 是它的低阶近似，也是对外表述的统一口号。** 分通道核算 $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$（式 (I-3.2)）是**记账分解**：其中的“+”为暂定写法，聚合算子（相加、取大或更复杂的权衡）尚未确定，故不承担定义功能。凡使用 $V\approx I\cdot T/E$，须标为低阶近似并声明校准状态；凡使用 $V_{\mathrm{s}}+V_{\mathrm{c}}$，须声明聚合算子暂定。

其中，$I$（信息处理与因果效力）、$T$（时间视界）与 $E$（热力学代价）均为广义变量，可在不同系统中展开为具体的动力学指标。存续势 $V$ 是对持久结构存续强度的积分度量，是演化过程中持续被优化的核心状态变量。我们以为自己在追求幸福、财富、权力、意义、爱、荣耀或复仇，但在热力学与信息学的统一视角下，这些动机都可以尝试被重新诠释为**存续势**这一共同度量在不同约束下的不同表征；“最大化”只在主动相成立（§3.5、§5.7），不作为对一切结构的驱动性断言。

### 本书的结构

本书由五卷构成，各卷独立成书，互不构成阅读顺序上的依赖。本卷承担理论核心：建立变量体系、核心动力学与可证伪预测——持久结构如何定义，其因果效力相对于谁（即解码器 $D$），为什么只有高阶智慧体才会产生复杂的「爱与恨」（即 $V$ 的三重分裂），智慧为什么会带来短视失控的风险，以及如何早期预警。

### 四层定位

本卷的每一句陈述都落在下面四层之一。读的时候先判断这一句在哪一层，再判断它有多硬。

- **本体层**：持久结构 $P$ 与物理信道——**什么存在**；
- **公理层**：存续势的低阶粗粒化基准 $V\approx I\cdot T/E$——**用什么度量**。它在指定近似下被选定，不是从物理定律推出的，理由与失效条件见 §3.1；
- **驱动层**：$\max V$——**演化的动力**。它在被动相里是筛选结果的描述（无目的），在主动相里是内生驱动的目标（有目的），两层不可混读。（$\max V$ 在书中有两个数学对象：筛选层的不等式 $\mathbb{E}[V_{\text{保留}}]\ge\mathbb{E}[V_{\text{淘汰}}]$，定义见卷Ⅱ §7.5；目标层的 $\max V^{\mathrm{val}}$，见 §3.5 与框架命题 1。二者共用一把尺子，不同层不可混读，也不得互相代换。凡未写“在约束域 (I-5.19) 内”的 $\max V$，都读作后者的简写。）
- **机制层**：解码器 $D$——**如何与世界交换**。

四层之间是依赖关系，不是“谁更底层”的排序：$D\to I\to V$ 是定义依赖链，$\max V$ 是目的论陈述，二者分属不同维度。凡本卷结论强度不足的地方，都注明了它停在哪一层。

### 与相邻框架的分工

本卷与相邻的《相对信息论》（Relational Information Framework，DOI: 10.5281/zenodo.24365795）各自独立成立，也各自可以单独阅读。后者把“信息”严格定义为某个读数相对于某个背景的稀有程度，并把背景构造、读数协议、瑕疵登记、单位记账这一整套测量层问题写清；它不讨论存续，也不给出存续效率的合成式。本卷在概念上沿用它给出的信息定义，在动力学上完全自足，在信息、时间、能量三个量之上讨论存续势的合成与动力学：信息如何被解码器赋予极性，时间视界如何内生化，能量成本如何分摊到两条通道，以及三者耦合时出现哪些相态。

两书在持久结构、解码器、结构信息、因果信息、两类存续时间与两条能量通道这六个概念上同名同义，各自在书内给出完整定义：本卷第一章定义持久结构与解码器，第二章定义信息、时间、能量三族。除这一句说明外，本卷不依赖任何外部文本，记号与判据均由本卷自行给出。

### 为什么需要这个框架

我们正处在硅基 AI 与碳基文明高速共演的时代，模因、算法、制度、生物体相互缠绕，旧的学科边界已不足以描述这种跨尺度混合体。SRVD 的核心创新有两点：提出存续势的双通道定义及其低阶粗粒化基准 $V\approx I\cdot T/E$，作为跨尺度统一的候选**度量语言**；并给出**驱动层元公设**——在给定约束下，被保留下来的结构其存续势不低于被淘汰者（筛选层，无目的，可被统计观测反驳）；对主动相结构，$\max V^{\mathrm{val}}$ 同时是实际优化的方向（目标层，有目的，可被策略漂移的方向反驳）。两层不可混读。“其他机制都是局部策略”一句不成立：局部策略层上走哪条路线是真实的选择，筛选层不改变标准，只筛选这些选择的后果（§3.3.2、卷Ⅱ §7.5）。

SRVD 不违背任何已知物理定律，不改建既有科学理论的地基，只提供另一个有穿透力的透镜：把矿物、生命、机器、文明与模因放在同一张桌子上对话，看清它们有什么共同规律、在哪里有本质区别，从而判断未来有哪些可能，以及我们还有多少可操作空间。

***

## 摘要

结构递归存续动力学（SRVD）是一个跨尺度的宏观粗粒化框架，把晶体、生命系统、AI 模型、文明与模因等一切持久结构统一纳入信息—时间—能量描述。公理：**无解码器，则无信息（作为有效因果信息）。**

核心度量是存续势（Viability Potential）$V$。单通道粗粒化基准形式 $V \approx I \cdot T / E$ 对应 $\alpha=\beta=\gamma=1$ 的特例，不构成 $V$ 的定义；一般粗粒化响应形式为幂律 $V = V_0 (I/I_0)^{\alpha} (T/T_0)^{\beta} (E/E_0)^{-\gamma}$，三个比值无量纲，$V_0$ 与 $V$ 同量纲；以 bit、s、J 计，基准 $V$ 的量纲为 bit·s/J。弹性指数 $\alpha, \beta, \gamma$ 作为待定参数保留，排序 $\alpha/\gamma > 1 > \beta/\gamma$ 是基于资源相对稀缺性的定性猜想，尚待推导或实证。

主要内容有四条。其一，**解码器内生化**：信息的价值不是信号固有属性，而由解码器 $D$ 提取并赋予极性（$I^{+}/I^{-}/I^{0}$）；认知解码器 $D_{\mathrm{cog}}$ 是三轴连续空间加自我指涉第四轴，具身型、在线型、符号型是区域而非离散类别。其二，**存续势三重分裂**：客观存续势按 $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ 作模型级聚合，须先统一核算边界、观察窗、持有者归属、成本分摊与效果去重；低阶式 $V\approx I\cdot T/E$ 是 $V$ 的低阶近似与对外表述；$V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ 是记账分解，聚合算子待定。$T_{\mathrm{pred}}$ 可自我调控后，系统进一步区分 $V_{\mathrm{obj}}$、$V^{\mathrm{virt}}$、$V^{\mathrm{val}}$；分裂本身中性，是高阶认知的必要条件；此后至少有两条路径，取决于脱钩偏差 $\Delta_{\mathrm{VV}}$ 与自指耦合强度 $\chi$——一条把虚拟势用于长期投资与前馈调节，另一条是短视失控态，后者只在符号型区域的高阶系统中可能激活，不是必然命运。对简化的信息—存续势子系统，本文给出平衡点与稳定性的解析分析，含鞍结分岔与临界耦合强度的显式表达式；该结果属于指定子系统，与完整认知系统阈值的对应仍待检验；路径二的 $\Delta_{\mathrm{VV}}$ 源项未给出，故“$\chi>\chi_{\mathrm{c}}$ 导致偏差放大”不是本模型的推论。其三，**五重递归**：$I, V, T, E, D$ 耦合演化，**以 $\max V$ 为框架元公设**（元公设是前提，递归是机制，二者不构成“收敛”关系）；本卷采用快—慢尺度分离下的线性化概念框架，完整双向耦合的 ODE/PDE 系统是开放问题。其四，**可证伪预测族**：涵盖强化学习中的视界先坍缩预警、结构同一性判据失效判定等。

SRVD 把朗道尔原理、热力学第二定律等作为外部物理约束接口；跨尺度动力学并不因此自动获得实验验证，只有在变量映射、系统边界与适用条件均满足时，相关约束才可用于具体模型。本框架可作为 AI 对齐、文明治理与复杂度演化研究的候选宏观语言。

**证据等级约定。** 本卷对每一处形式化陈述标注四级标签之一：**【定理】**前提完整列出、推导闭合、结论在该前提下严格成立；**【命题】**有形式化陈述，但前提部分待标定，或推导某步依赖未证的建模假设；**【候选推论】**由某命题在附加条件下导出、尚未独立检验；**【假说】**经验性或机制性猜测，无形式化推导。凡标【命题】者，正文同时给出前提、结论与失效条件三行。本卷不把任何依赖未标定参数的结论称为定理。

**关键词**：存续势；解码器相对性；持久结构；信息—时间—能量；朗道尔原理；动力系统；可证伪性

**Abstract.** Structure Recursive Viability Dynamics (SRVD) is a cross-scale, macroscopic, coarse-grained framework that brings all persistent structures — crystals, living systems, AI models, civilizations, memes — under one information–time–energy description. Axiom: **without a decoder, there is no information (as effective causal information).**

The core measure is the viability potential $V$. The single-channel coarse-grained baseline form $V \approx I \cdot T / E$ corresponds to the special case $\alpha=\beta=\gamma=1$ and does not constitute the definition of $V$; the general coarse-grained response form is the power law $V = V_0 (I/I_0)^{\alpha} (T/T_0)^{\beta} (E/E_0)^{-\gamma}$, in which the three ratios are dimensionless and $V_0$ has the same dimension as $V$; with bit, s and J as units, the baseline $V$ has dimension bit·s/J. The elasticity exponents $\alpha, \beta, \gamma$ are retained as parameters to be determined; the ordering $\alpha/\gamma > 1 > \beta/\gamma$ is a qualitative conjecture based on relative resource scarcity, awaiting derivation or empirical test.

There are four main contents. First, **endogenization of the decoder**: the value of information is not an intrinsic property of the signal but is extracted by the decoder $D$, which also assigns its polarity ($I^{+}/I^{-}/I^{0}$); the cognitive decoder $D_{\mathrm{cog}}$ is a three-axis continuous space plus a fourth, self-referential axis, and the embodied, online and symbolic types are regions, not discrete classes. Second, **the triple splitting of the viability potential**: the objective viability potential is aggregated at the model level as $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$, which requires first fixing the accounting boundary, observation window, holder attribution, cost apportionment and effect de-duplication; the low-order $V\approx I\cdot T/E$ is the low-order approximation of $V$ and its public statement; $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ is a bookkeeping decomposition whose aggregation operator is yet to be determined. Once $T_{\mathrm{pred}}$ can regulate itself, the system further distinguishes $V_{\mathrm{obj}}$, $V^{\mathrm{virt}}$ and $V^{\mathrm{val}}$; the splitting itself is neutral and is a necessary condition for higher-order cognition; after it there are at least two paths, depending on the decoupling deviation $\Delta_{\mathrm{VV}}$ and the self-referential coupling strength $\chi$ — one puts the virtual potential to use for long-term investment and feedforward regulation, the other is the myopic runaway regime, which can be activated only in higher-order systems in the symbolic region and is not an inevitable fate. For a simplified information–viability-potential subsystem, this text gives an analytic treatment of equilibrium points and stability, including explicit formulas for the saddle-node bifurcation and the critical coupling strength; this result belongs to the specified subsystem, and its correspondence to the thresholds of a full cognitive system remains to be tested; the $\Delta_{\mathrm{VV}}$ source term of path two is not given, so "$\chi>\chi_{\mathrm{c}}$ leads to deviation amplification" is not an inference of this model. Third, **fivefold recursion**: $I, V, T, E, D$ evolve in coupling, **with $\max V$ as the framework's meta-postulate** (the meta-postulate is the premise, the recursion is the mechanism, and the two do not stand in a "convergence" relation); this volume adopts a linearized conceptual framework under fast–slow time-scale separation, and the fully bidirectionally coupled ODE/PDE system is an open problem. Fourth, **a family of falsifiable predictions**: covering early warning of horizon collapse in reinforcement learning, failure determination for the structural identity criterion, and so on.

SRVD takes the Landauer principle, the second law of thermodynamics and the like as interfaces to external physical constraints; cross-scale dynamics does not thereby automatically gain experimental verification, and the relevant constraints can be applied to a concrete model only when the variable mapping, system boundary and applicability conditions are all satisfied. The framework can serve as a candidate macroscopic language for research on AI alignment, civilizational governance and the evolution of complexity.

**Evidence-level convention.** This volume labels every formal statement with one of four level tags: **Theorem**: premises are fully listed, the derivation closes, and the conclusion holds strictly under those premises; **Proposition**: has a formal statement, but the premises are in part to be calibrated, or some step of the derivation depends on an unproven modeling assumption; **Candidate Corollary**: derived from some proposition under additional conditions and not yet independently tested; **Hypothesis**: an empirical or mechanistic conjecture with no formal derivation. Wherever a statement is labeled **Proposition**, the main text also gives three lines — premises, result and failure conditions. This volume calls no conclusion that depends on an uncalibrated parameter a theorem.

**Keywords**: viability potential; decoder relativity; persistent structure; information–time–energy; Landauer principle; dynamical systems; falsifiability

**框架命题一览。** 下列十一条是本卷的框架命题：各有形式化陈述与可讨论的结论，但参数、阈值或函数形式至少有一项尚未标定，因此一律标为【命题】。每条可单独反驳，反驳条件列于右列；正文对应章节给出完整的前提、推导与适用域。

| 编号 | 框架命题 | 反驳条件（摘要） |
| :--------- | :----------------------- | :------------------------- |
| 1 | $\max V$ 是负熵结构的长期宏观目标；主动相实际执行的是 $V^{\mathrm{val}}$ | 策略漂移方向与 $V_{\mathrm{obj}}$ 排序无关，或速率与其差无单调关系 |
| 2 | 低阶粗粒化基准 $V \approx I\cdot T/E$ 及幂律推广 | 秩相关不显著，或域内校准后残差呈系统性结构 |
| 3 | 四类载体与三阶认知 | 既无法归类也无法标为混合，或三阶归并互相矛盾 |
| 4 | 被动—主动—认知连续；$V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ 为条件性模型聚合 | $V_{\mathrm{c}}$ 的可操作代理被稳定测为零而非极小正数 |
| 5 | 解码器第一性：$D \to I \to V$ | 存在不指定解码器即可稳定测量并独立预测 $V$ 的信息量 |
| 6 | 弹性指数为 log–log 斜率、无量纲；排序属假说 | 预注册检验通过后，同域重复测量稳定给出 $\alpha/\gamma \le 1$ |
| 7 | 内生时间视界受 $T_{\mathrm{min}}<T_{\mathrm{pred}}\le\min(T_{\mathrm{struct}}^{\max},T_{\mathrm{env}})$ 约束 | 加入 $T_{\mathrm{pred}}$ 不提高任何预测力 |
| 8 | 三重分裂与分裂后的两条路径 | $V^{\mathrm{val}}$ 可完全由 $V_{\mathrm{obj}}$ 当期值解释 |
| 9 | 信息极性三分 $I^{+}/I^{-}/I^{0}$ | 同一输入同时表现为 $I^{+}$ 与 $I^{-}$ 且不可按时段或尺度拆分 |
| 10 | 五重递归 $I\to V\to T\to E\to D$ | 加入反向耦合后定性行为改变，则单向链只保留为局部近似 |
| 11 | 三资源筛选：$I,T,E$ 互不可替代，$D$ 非第四类资源 | 必须引入第四个独立资源维度才能恢复预测力 |

## 第一章　本体层：持久结构与解码器

本章确定框架的最小本体：什么算一个持久结构，谁有资格作为解码器读取它，以及二者所处的物理背景。此后的全部变量都定义在这三样东西之上。

### 1.1 持久结构

**定义：持久结构（Persistent Structure，PS）是在能量约束下形成、可从背景中区分，并能在有限时间窗口内维持其可识别拓扑组织的有序负熵构型。** 这里的“拓扑组织”指其关键关系的组织形式，不要求物质载体保持不变。其成立需满足三个条件：存在可区分于背景的有序负熵组织；该组织能在有限时间窗口内保持连续性；存在足够的能量条件支撑其存续。

“有限”指非无限：任何持久结构都受制于热力学终极边界、宇宙演化边界或物理常数设定的极限，并不意味着时间尺度狭小。花岗岩可存续十亿年量级，仍属有限时间，“有限”与“持久”并不矛盾。因此一个结构是否“持久”，不取决于绝对寿命的长短，而取决于它能否在给定能量条件下使自身拓扑特征在相应时间窗口内保持可识别。量子态、晶体、恒星、基因组、神经网络、语言、制度与文明，尺度、成分与介质相差悬殊，但在动力学意义上属于同一类对象：在能量约束下形成并维持的、有序且可区分的拓扑构型。框架不预设“物理的”与“抽象的”之间存在本体论断裂，后续核心变量都定义在持久结构之上，并通过其载体、维持成本与因果执行方式加以区分。

#### 1.1.1 载体分层

| 载体类型 | 主导能量项 | $E_{\mathrm{causal}}$ 角色 | 存续核心 | 典型实例 |
| :--------- | :---------- | :---------- | :---------- | :---------------- |
| **势垒冻结型** | $E_{\mathrm{barrier}}$ | 近乎无主动因果调用 | 结构不散 | 晶体、岩石；指定窗口内主要靠结构约束维持组织的尸体、纸质书、断电硬盘 |
| **物理耗散型** | $E_{\mathrm{survival}}$ | 无认知，持续物理耗散 | 断能即散 | 恒星、火焰、台风、洋流、贝纳德对流 |
| **主动耗散型·具身型** | $E_{\mathrm{survival}} + E_{\mathrm{barrier}} + E_{\mathrm{causal}}$（因果处理成本通常较低） | 低功耗生化积分、物理试探 | 代谢加遗传模板 | 植物、真菌、细菌、水熊虫等低级动物 |
| **主动耗散型·在线型** | $E_{\mathrm{survival}} + E_{\mathrm{causal}}$ | 联想学习与在线模拟 | 代谢加神经认知 | 乌鸦、狗、大部分动物 |
| **主动耗散型·符号型** | $E_{\mathrm{survival}} + E_{\mathrm{causal}}$ | 离线多路径反事实推演 | 代谢加符号认知 | 人类、具身 AI |
| **外部载体依赖型·病毒型** | 宿主复制机器的能耗（宿主支付） | 无自身因果调用，借宿主机制复制 | 宿主复制机器持续可得 | 病毒谱系 |
| **外部载体依赖型·形式数学型** | 外部调用时由承载者支付相应 $E_{\mathrm{causal}}$ | 形式推演与关系调用 | 数学／逻辑关系被正确实例化或调用 | 数学结构、逻辑关系、几何结构 |
| **外部载体依赖型·模因虚拟型** | $E_{\mathrm{causal}}$（宿主支付） | 传播扩散 | 共识维持 | 货币、宗教、语言 |
| **外部载体依赖型·软件型** | 运行硬件能耗（运行环境支付） | 由计算硬件执行 | 代码、参数与存储状态被保存并运行 | 软件、模型参数 |

主动耗散型内部按 $D_{\mathrm{cog}}$ 三轴位置细分：具身型区域（三轴低值）、在线型区域（三轴中高）、符号型区域（三轴高值）；在线型区域是符号型区域的下端过渡带。框架内不存在零物理维持成本的“纯抽象”结构：外部载体依赖型总要由外部承载系统支付 $E_{\mathrm{causal}}$ 或运行能耗。

**外部载体依赖型的界定。** 外部载体不仅包括物质存储介质，也包括提供计算实现、生物复制、认知调用、社会传播或制度维持等功能的外部系统。普通的能源需求、代谢依赖、生态位依赖或一般环境影响本身不足以构成判据；关键在于外部系统是否承担了特征性信息组织得以实现、复制或延续的必要功能，且该功能不能由 PS 内部机制等价替代。四个子类的处理要点：病毒型以谱系的复制延续为分析对象，单个颗粒的物理存续另行分析；模因虚拟型中符号记录的保存不必然意味着相应结构仍然有效，单一载体消失也不必然意味着结构无法延续；形式数学型须区分结构本身与其表达载体：数学、逻辑及几何关系属于本类；物理规律作为客观物理关系纳入物理信道，不以人类表述为存在条件。符号、公式、证明文本、教科书及通信协议是这些结构的表示或记录，不因承载了数学内容就自动等同于数学结构。调用形式数学结构时，外部认知或计算系统承担相应能耗；日常数学推理也可以只是主体内部的认知活动。**本卷所称数学形式持久结构包括逻辑关系、数学关系与物理规律。** 其中物理规律作为客观结构关系归入物理信道，不以人类表述为存在条件；证明、符号、公式的具体文字记录、教科书及通信协议属于表达、记录或传播载体，不因承载数学内容就自动等同于数学结构本身。软件型须区分代码、参数、存储状态与某次运行实例，某个实例停止不必然意味着软件结构消失。

**与解码器的关系。** 分类描述主要存续条件，不直接决定 $D$ 是否存在或属何种类型。外部系统提供承载条件，不意味着其全部功能属于目标 PS 自身的解码器，解码器资格仍按判据独立判断。**计量边界**：复杂对象可含不同层次的子结构，混合表示同一对象在不同边界或时间窗下归属不同，不构成第五类；测量 $I$、$T$、$E$ 时须先确定目标 PS 的边界、尺度与时间窗，外部承载系统的信息、时间与资源代价不得未经论证直接计入，共享载体或多个 PS 协同运行时须先声明代价分配规则，避免重复计量。

**三阶认知归并。** 全框架在认知层级上统一归并为三阶，不因载体细分而增加阶数：

1. **第一阶：严格零认知（$D = \varnothing$）。** 势垒冻结型与物理耗散型，如岩石、晶体、火焰、台风、恒温器。特征：$V_{\mathrm{c}} \equiv 0$，$T_{\mathrm{pred}} \equiv 0$，自身无解码器，其结构信息可被外部读数协议（如 $D_{\mathrm{macro}}$）读取。
2. **第二阶：极低生命认知（具身型区域）。** 植物、真菌、细菌。特征：$V_{\mathrm{c}} \to 0^{+}$，三轴低值，可塑时间尺度偏跨代。
3. **第三阶：高阶符号认知（在线型及以上区域）。** 人类、具身 AI；乌鸦、章鱼等在线型认知作为该阶下端的过渡带归入此类，不单列一级。特征：$V_{\mathrm{c}} \gg 0$，三轴中高至高值。

![图 Ⅰ-2　持久结构的载体分类](figures/release/G1_持久结构的载体分类.pdf)

**图 Ⅰ-2　持久结构的载体分类。** 四类顶层分类（势垒冻结型、物理耗散型、主动耗散型、外部载体依赖型）与各自的主导维持机制、典型实例、解码器位置。认知位置（具身型／在线型／符号型区域）是主动耗散型内部的连续区域，不是与载体类型并列的分类轴。概念图，不含数值。

### 1.2 解码器

#### 1.2.1 解码器的定义

**无解码器，则无信息（作为有效因果信息）。** 公共读数协议（如 $D_{\mathrm{macro}}$）可读出结构信息，但不是解码器持有者，不产生有效因果信息。解码器（decoder，$D$）是持久结构从潜在构型中提取有效因果信息、用以维持自身存续的物理机制；它是结构与物理信道之间的界面，决定能量流入、转化与分配的方式。

从操作化角度看，解码过程的本质是**物理态耦合与信息映射**：$D$ 以效率 $\eta_D \in [0,1]$ 从潜在信息 $I_{\mathrm{latent}}$ 中提取当前被激活的子集 $I_{\mathrm{active}} \equiv \eta_D \cdot I_{\mathrm{latent}}$。低效解码（$\eta_D \to 0$）普遍存在于被动结构中，高效递归解码是主动相的高阶特征。净有效因果信息 $I_{\mathrm{net}} = \varphi_{\mathrm{s}} I_{\mathrm{struct}} + \varphi_{\mathrm{c}} I_{\mathrm{causal}}$ 是由两条通道按能量分配权重合成的粗粒化基准量。$I_{\mathrm{active}}$ 由 $I_{\mathrm{latent}}$ 定义，$I_{\mathrm{net}}$ 是 $I_{\mathrm{struct}}$ 与 $I_{\mathrm{causal}}$ 的加权合成；当前定义推不出二者之间存在普遍包含关系或 $I_{\mathrm{active}} \le I_{\mathrm{net}}$ 的上界，本卷不将该关系预设为已确立结论。

解码器本身也是持久结构，同样服从存续动力学：$V(D) \approx I_{\mathrm{net}}(D)\cdot T(D)/E_{\mathrm{eff}}(D)$（低阶近似，$T$ 取结构存续时间），观察者与被观察对象由此形成自洽闭环。依赖链为 **$D \to I \to V$**（无解码器的被动结构，$D$ 取公共读数协议）：任何讨论“信息处理”“信息流”“信息价值”的理论，若未先定义其解码器，在 SRVD 框架下视为未完成定义。

#### 1.2.2 物理解码器 $D_{\mathrm{phys}}$

物理解码器是**有自维持边界**的选择性提取机制：它具备一层哪怕最简陋的自我维持边界，对环境差异的选择性提取服务于这层边界背后那套结构自身的存续。内部再分两层：**静态**——选择规则被长期历史进程固定，运作期间不因环境细节改写，如离子通道只对钠离子开放、水熊虫脱水到某个程度触发休眠；**动态**——结构自身存在实时反馈，比较“现在”与“刚才”并据此调整响应，如细菌趋化性、植物向光性。

**不含自维持边界的结构不在此列。** 石头、晶体、恒星都没有“自己”在被守护，归入 $D = \varnothing$。恒温器也不属于 $D_{\mathrm{phys}}$：它维持的是房间里人的舒适，不是它自己的边界，其效果算在使用者名下。有反馈、有阈值、有状态切换，都不足以让结构自动进入 $D_{\mathrm{phys}}$；关键是这种选择性提取是否在维持提取者自己的那套边界。具身型认知解码器（植物、真菌、细菌的生化积分与物理试探）以 $D_{\mathrm{phys}}$ 为基础，不另立独立层级。

#### 1.2.3 认知解码器 $D_{\mathrm{cog}}$

认知解码器是一个**连续谱系**，不是二值开关，由三根连续轴刻画：**历史依赖程度**（内部状态有多少由过去经历决定，而非完全由当前输入决定）、**存续耦合程度**（这层历史依赖与自身存续核算绑得多紧）、**可塑发生的时间尺度**（可塑性是跨代焊死，还是个体一生内可改写）。三轴大致划出三片区域：

| 区域 | 三轴位置 | 典型实例 |
| :------------ | :----------------------- | :---------------------- |
| 具身型区域 | 三轴低值，可塑时间尺度偏跨代 | 细菌适应性调节、含羞草习惯化、植物向性 |
| 在线型区域 | 三轴中高，可塑时间尺度偏个体一生 | 乌鸦、章鱼、大多数哺乳动物 |
| 符号型区域 | 三轴高值，出现离线推演、反事实、符号操作 | 人类、部分 AI |

三轴的具体测量协议尚待建立，第四轴“自我指涉程度”目前只有概念定义。三片区域是三轴空间的粗粒化表述，与三阶归并一一对应；恒温器、岩石、火焰等系统只有 $D = \varnothing$，完全不进入 $D_{\mathrm{cog}}$ 谱系。

#### 1.2.4 解码器的主动性判据

一个系统是“主动存续”的解码器，当且仅当同时满足三个最小条件：**内部状态可控**（能依据内部模型改变自身行为，而非仅被外部驱动）；**能量流可调**（能主动增减 $E_{\mathrm{flow}}$ 以响应环境变化）；**时间视界可预测**（$T_{\mathrm{pred}} > 0$，并能据此调节当前行为）。

这三条是**主动相判据**，只判断“主动存续”属性，不替代解码器的**四项一般资格条件**。四项条件由卷Ⅳ §2.2 定义 2.2 给出，与本处逐字一致、缺一不可：① **自身维持可识别边界**；② **选择性提取环境差异**；③ **由提取引发状态更新**；④ **该更新对自身存续具有因果意义**。只有先满足这四项的系统，才继续接受本节的主动性分类。据此：岩石、行星、恒星、火焰、恒温器不满足全部条件，归入 $D = \varnothing$；细菌、植物、真菌满足主动性条件，归入 $D_{\mathrm{phys}}$；乌鸦、章鱼、哺乳动物、人类、具身 AI 满足主动性条件且三轴位置达到在线型及以上，归入 $D_{\mathrm{phys}} + D_{\mathrm{cog}}$。判据的判定对象是作为整体的系统（细胞、个体、机器人）；静态选择规则（离子通道、休眠开关）属于持有者内部的组成部分，不单独接受本判据，其归属随持有者。

> **恒星的归类。** 恒星内部确有反馈（如核心温度与聚变速率的负反馈），但不依赖内部预测模型、也无自维持边界，故 $D=\varnothing$：其有效视界等同于燃料储量决定的 $T_{\mathrm{struct}}^{\max}$，不能被内部状态主动延长或压缩。这才是它属被动存续的原因，而非“是否存在能量流调节”。

#### 1.2.5 解码器符号汇总

| 符号 | 名称 | 定义 | 适用范围 |
| :------ | :------------ | :----------------------- | :--------------- |
| $D = \varnothing$ | 无解码器 | 无自维持边界的纯物理结构 | 岩石、晶体、恒星、火焰、恒温器 |
| $D_{\mathrm{phys}}$ | 物理解码器 | 有自维持边界的选择性提取，分静态与动态 | 细菌、植物、真菌、低级动物 |
| $D_{\mathrm{cog}}$ | 认知解码器 | 在 $D_{\mathrm{phys}}$ 基础上叠加的功能复杂度，三轴连续空间 | 乌鸦、章鱼、哺乳动物、人类、具身 AI |
| $\eta_D$ | 解码效率 | $\eta_D \in [0,1]$，$I_{\mathrm{active}} \equiv \eta_D \cdot I_{\mathrm{latent}}$ | 所有 PS |
| $\mathcal{T}$ | 拓扑跃迁算子 | 拓扑跃迁发生时打开新因果维度的操作 | 仅主动相 |
| $D_{\mathrm{depth}}$ | 规则深度（静态定义） | 解码器 $D$ 在容差内还原 $P$ 所需的最少独立规则数（无短于逐点记录的规则时为 0） | 所有 PS；完美晶体为 1 |
| $D_{\mathrm{depth}}^{\mathrm{dyn}}$ | 深度指数（动力学定义） | $1 + \#\{\mathcal{T}\}$，即跃迁计数加一；仅对静态深度不小于 1 的对象定义 | 有跃迁史的主动相；被动相恒为 1 |

**$D_{\mathrm{depth}}$ 的双层含义。** 必须把两件事分开，否则会把一个标定假设读成数学等式。

**静态层面是定义**：$D_{\mathrm{depth}}$ 为解码器 $D$ 在指定容差内还原一个对象所需的最少独立规则数；完全随机、找不到短于逐点记录的规则时取 0。完美晶体只有一条规则（“全白”），$D_{\mathrm{depth}} = 1$；手表有齿轮传动、发条储能、指针指示等多条独立规则，深度更高；雪花枝晶是同一条规则在不同尺度重复，重复展开不增加深度。这是本卷对“规则深度”的正式定义，也是唯一作为定义使用的写法。

**动力学层面是深度指数**：把跃迁次数作为深度的演化代理，写作 $D_{\mathrm{depth}}^{\mathrm{dyn}} \equiv 1 + \#\{\mathcal{T}\}$，$\#\{\mathcal{T}\}$ 为到观测时刻为止的拓扑跃迁次数。带 $\mathrm{dyn}$ 上标的量不是“实际规则数”，它与静态定义共享同一直觉（规则越多越深），数值上不必相等。

两者不能当成同一个量：一次跃迁可能同时引入多条独立规则（从牛顿力学到相对论，一次跃迁同时改写时空、质量、能量三组关系），也可能只改变既有规则的组织方式而不新增规则（同一套方程换一种等价表述）。因此“每次跃迁恰好增加一条独立规则”是一个**标定假设**，不由静态定义推出。写下 $D_{\mathrm{depth}}^{\mathrm{dyn}} = 1 + \#\{\mathcal{T}\}$ 时，本卷同时声明该假设，并在下面的标定方法中给出检验它的办法；假设不成立时深度指数仍可用，但它只是跃迁计数，不再是深度估计。

**标定方法。** 取一组可比对象（同一域、同一观察尺度、同一容差），对每个对象独立测出静态深度 $D_{\mathrm{depth}}$（按容差内的最小编码长度或最小规则集计数），同时从历史记录中数出跃迁次数 $\#\{\mathcal{T}\}$，做回归

$$
D_{\mathrm{depth}} = a + b\cdot \#\{\mathcal{T}\} + \varepsilon_{\mathrm{res}} \tag{I-1.1}
$$

母命题 $D_{\mathrm{depth}}=1+\#\{\mathcal{T}\}$ **同时预测 $a=1$ 与 $b=1$**，故须同时检验两者：预先设定截距与斜率的等效容差，并分别进行等效性检验（例如 TOST）；仅仅未能拒绝 $a=1$ 或 $b=1$ 的普通差异检验，不足以证明二者等于 1。残差中还不得存在随对象类型系统变化的趋势（同质性检验）。只检 $b$ 会削弱可证伪性——若作者认为 $a$ 受测量零点影响不宜强制，须在此写明理由，并把卷Ⅱ §2.4 的 $a=1$ 标为“可选”。两条同时通过时，“每次跃迁增加一条独立规则”在该域内可作工作假设；斜率显著大于 1，说明一次跃迁平均引入多条规则，深度指数应改写为 $1 + b\cdot\#\{\mathcal{T}\}$ 并重标定；斜率显著小于 1 或接近 0，说明跃迁主要改变规则组织而非数量，此时深度指数只能作为“范式变更次数”的代理，不能用于深度比较。回归的容差、编码方式、跃迁计数规则须在测前锁定，事后调参不算通过。

**符号说明**：$D_{\mathrm{depth}}$ 中的 $D$ 取自 depth（深度），不是解码器归属符号。

### 1.3 物理信道

**定义**：物理信道（$C_{\mathrm{phys}}$）是持久结构及其解码器所处的环境底座，包含基本相互作用及其所有涌现出的底层规则；在已知物理学框架内，它为能量流动提供管道，为信息交互提供协议。任何解码器的运作都受制于三个嵌套约束层：

- **底层法则约束**：电磁力、引力、强核力、弱核力为能量转移与信号传递提供底层约束，是解码器不可逾越的物理基底。
- **介质结构约束**：基本相互作用在特定时空聚集形成的中观介质（空气、水、真空、神经纤维）对信号施加带宽限制、延迟与衰减，决定解码器可提取的有效信号量。
- **热力学下界约束**：热涨落与耗散引入信道噪声；只有在逻辑不可逆擦除与 SRVD 信息变量之间建立可检验映射之后，朗道尔原理才为对应的 $E_{\mathrm{compute}}$ 提供条件性能量下界，它不直接给出一般 $E_{\mathrm{causal}}$ 或任意有效因果信息量的下界。

$C_{\mathrm{phys}}$ 在本框架中被视为固定背景而非动力学变量，它决定微观势垒高度 $\Delta U_{\mathrm{barrier}}$、$E_{\mathrm{causal}}$ 的效率极限，以及 $I_{\mathrm{net}}$ 的最大可能值。它是所有解码器共同受制的约束背景：热力学第二定律与光速因果限制之所以具有跨文化、跨物种的普遍客观性，正是因为任何解码器违反它们都会遭遇不可逆的实践惩罚。这是 $C_{\mathrm{phys}}$ 区别于文化共识的根本标准。

![图 Ⅰ-3　SRVD 的最小理论架构](figures/release/G2_SRVD最小理论架构.pdf)

**图 Ⅰ-3　SRVD 的最小理论架构。** 从持久结构 PS 的可辨识组织，经解码器 $D$ 读取，形成 $I$、$T$、$E$ 三元读数，并在相容配对下形成存续势读数 $V$（$D \to (I,T,E) \to V$）；物理信道 $C_{\mathrm{phys}}$（底层法则、介质结构、热力学下界）是所有解码器共同受制的约束背景。图示为概念架构，不表示完整动力学闭环。概念图，不含数值。

***

## 第二章　变量宪法

本章定义贯穿全卷的核心变量，分信息、能量、时间、存续势、解码器五个家族，外加弹性指数与少量动力学参数。每个符号在此给一次完整定义（含单位与适用域），后文再用时只作一句复述。

### 2.1 $I$ 家族（信息家族）

**用语约定。** 裸称“信息”时指上位概念，不指单一可测量。可测量的信息变量是结构信息 $I_{\mathrm{struct}}$ 与因果信息 $I_{\mathrm{causal}}$；公式中的裸符号 $I$ 默认指 $I_{\mathrm{net}}$（显式声明除外），它是由二者合成的模型量，不是直接测量量。凡讨论「有效信息」，一律写全为「净有效因果信息」（合成量 $I_{\mathrm{net}}$）或「有效因果信息」（满足因果效果三项入门条件的 $I_{\mathrm{causal}}$）。

**时间口径。** 存续势公式里的 $I\cdot T$，只有当 $I$ 在 $T$ 内恒定时才等于 $\int I\,\mathrm{d}t$。本卷的处理是：凡出现 $I$ 与 $T$ 相乘，$I$ 一律指 **$T$ 内的读数均值** $\bar I$，即 $\bar I:=\frac{1}{T}\int_{S}I(t)\,\mathrm{d}t$，其中 $T=\mu(S)$，$S$ 是使读数成立的那个时间集合（结构通道取可辨识时段，因果通道取效果可识别时段）。$I$ 在窗内恒定时 $\bar I=I$，原式不变；$T=0$ 时 $\bar I$ 不定义，不出现零除零。报告读数必须同时写明三件事：采样时点或窗口、取的是均值还是单点、以及窗口内是否检出背景漂移。只有单点读数时标「$I(t_0)$ 单点读数」，此时 $V$ 对单调衰减的 $I$ 只作上界。跨对象比较一律固定同一窗口。

**双通道。** 低阶核心方程以 $I_{\mathrm{net}}$ 为输入；精细核算用两通道形式，输入为 $I_{\mathrm{struct}}$ 与 $I_{\mathrm{causal}}$：

$$
I_{\mathrm{net}} = \varphi_{\mathrm{s}} I_{\mathrm{struct}} + \varphi_{\mathrm{c}} I_{\mathrm{causal}}, \qquad \varphi_{\mathrm{s}} = \frac{E_{\mathrm{struct}}}{E_{\mathrm{eff}}}, \quad \varphi_{\mathrm{c}} = \frac{E_{\mathrm{causal}}}{E_{\mathrm{eff}}}, \quad \varphi_{\mathrm{s}} + \varphi_{\mathrm{c}} = 1 \tag{I-2.1}
$$

通道权重直接取能量读数之比，不是待拟合参数；权重取能量比是模型约定，不是从 $E$ 推出 $I$ 的独立推导，$E_{\mathrm{eff}}$ 的核算范围（含持有者）须先于权重声明。纯结构型退化为 $I_{\mathrm{net}}\approx I_{\mathrm{struct}}$，纯认知型退化为 $I_{\mathrm{net}}\approx I_{\mathrm{causal}}$。两种 bit 按此加权未经域内标定时，$I_{\mathrm{net}}$ 只作量级指标，不替代两个子通道的读数。

**加性与数值可比性是建模约定，不是单位自动保证的结论。** $I_{\mathrm{struct}}$ 与 $I_{\mathrm{causal}}$ 使用不同的读数协议、背景和对照物；二者都以 bit 计，不足以证明它们处于同一语义尺度。能量份额 $\varphi_{\mathrm{s}}$、$\varphi_{\mathrm{c}}$ 只提供可核算的折算权重，不证明两类 bit 可以互换。因此 $I_{\mathrm{net}}$ 是粗粒化合成指数，不是直接测量量，也不是由热力学第一性原理推出的量。其数值只有在同时满足四项条件时才可作定量使用：（i）两条通道使用**同一读数协议**（同一度量方式、同一分辨率、同一极端方向）；（ii）**同一背景**与同一对照物构造规则；（iii）**同一观察窗**，且窗口内两条通道的采样密度可比；（iv）已完成**域内校准**，即在同一批对象上验证过加权和与某个独立可观测量（存活时间、产出、恢复力等）的关系单调且稳定。四项缺一，$I_{\mathrm{net}}$ 只作**序关系指标**：可以说“甲的 $I_{\mathrm{net}}$ 高于乙”，不可以说“甲是乙的 1.7 倍”，更不可以跨域比较其数值。任何加权和都隐含一个折算率，折算率本身必须有独立的经验依据；在未校准的域里，加权和的绝对数值没有意义，只有符号与序有意义。

**测量契约。** 任何信息读数须声明五项：读数对象、背景或对照、度量方式、分辨率与极端方向、观察窗与不确定度。更换任一项后须重新标定，不与旧读数直接比较。信息只相对于读数者（解码器及其持有者，或公共读数协议）成立，换用对象、持有者或对照后不得沿用读数。为行文简洁，以下在不引起歧义时把 $I_{\mathrm{struct},D}(P)$、$I_{\mathrm{causal},D}(P)$ 简写为 $I_{\mathrm{struct}}$、$I_{\mathrm{causal}}$，$P$ 与 $D$ 默认取当前讨论的结构及其持有者；比较不同对象或持有者时恢复完整写法。

**结构信息 $I_{\mathrm{struct},D}(P)$。** 默认度量为相对背景的稀有度：离散读数 $r=D(P)$ 取 $-\log_2\Pr_B(r)$；有序读数按事先声明的方向取尾概率；分布读数取相对熵并说明估计与平滑。背景默认取持有者栖息环境中该读数的自然频率分布；无持有者的被动结构由公共读数协议指定参照总体；无法构造时须明示为建模者指定的背景。描述长度、有效维度、构型熵等口径可替代默认度量，但须同样声明五项。

**因果信息 $I_{\mathrm{causal},D}(P)$。** 度量 $P$ 相对于对照物 $P_0$ 所产生的可观察效果有多稀有。先声明 $D$、$P$、$P_0$、效果读数 $e$ 与观察窗，再在 $P_0$ 下测得效果分布 $B_0$：

$$
I_{\mathrm{causal},D}(P)=-\log_2\Pr_{B_0}\big(s(e')\ge s(e_{\mathrm{obs}})\big)
$$

$s$ 是事先声明的效果统计量，小值更极端时反向使用 $\le$；离散效果可取 $-\log_2\Pr_{B_0}(e=e_{\mathrm{obs}})$。效果须同时满足反事实差异、可观察性与持有者付出可测代价三项入门条件；仅有稀有读数而没有可观察因果效果，不计入。

**代入本卷方程的条件。** 信息变量须满足：非负；控制 $T$、$E$ 后仍能独立预测 $V$ 的变化（因果效力，这是对模型解释力的检验要求，不是 $I$ 的定义）；不能被 $T$、$E$ 的函数归约（否则乘积形式退化为冗余）。物理界只对满足相应定义的量适用：朗道尔下界约束逻辑不可逆擦除量，贝肯斯坦界（Bekenstein, 1981）与全息界（Bousso, 2002）约束物理熵或可区分状态数，建立了到这些量的映射才可代入。

| 符号 | 单位 | 定义 | 适用范围 |
| :------- | :------ | :----------------------------- | :------------- |
| $I$ | bit | 广义结构差异：持久结构相对于背景的可区分有序差异总量 | 所有 PS |
| $I_{\mathrm{struct}}$ | bit | 结构信息：按测量契约定义的结构通道信息量 | 所有 PS |
| $I_{\mathrm{causal}}$ | bit | 因果信息：$P$ 相对于持有者 $D$ 的对照基线所产生效果的稀有度；效果须满足反事实差异、可观察性与可测代价三项条件 | 存在合格效果与持有者时 |
| $I_{\mathrm{net}}$ | bit | 净有效因果信息：$\varphi_{\mathrm{s}} I_{\mathrm{struct}} + \varphi_{\mathrm{c}} I_{\mathrm{causal}}$；加性为建模约定，四项条件齐备才可作数值使用；合成模型量，非直接测量量 | 所有 PS |
| $I_{\mathrm{latent}}$ | bit | 潜在因果信息：当前未激活但可恢复的因果能力存量 | 仅主动相 |
| $I_{\mathrm{active}}$ | bit | 激活因果信息：$\eta_D \cdot I_{\mathrm{latent}}$ | 仅主动相 |
| $I_{\mathrm{max}}(D)$ | bit | 解码器 $D$ 能提取的最大信息容量 | 所有 PS |
| $I_{\mathrm{min}}$ | bit | 维持同一性所需的最低信息量 | 所有 PS |
| $I^{+}$ / $I^{-}$ / $I^{0}$ | bit | 正效／负效／中性：扩大／压缩未来可达状态空间的输入，或无存续极性的物理因果输入 | $I^{+}$、$I^{-}$ 仅主动相 |
| $\tilde I_{\mathrm{orig}}$ | bit | 候选范式突破信号：$D_n$ 在目标上的预测残差相对其历史残差分布的稀有度，$-\log_2\Pr_{B_n}(\varepsilon_{\mathrm{res}}\ge\varepsilon_{\mathrm{obs}})$；跃迁前唯一门控变量，可观测代理 | 仅主动相 |
| $I_{\mathrm{orig}}$ | bit | 经验证的新增信息：跃迁成功并独立复现后追认的新增有效因果信息；事后量，不作事前门控 | 仅主动相 |
| $I_{\mathrm{interp}}$ | bit | 范式解释信息：现有范式内的优化，边际效能快速衰减 | 仅主动相 |
| $I_{\mathrm{type}}$ / $I_{\mathrm{token}}$ | bit | 信息类型（可继承的模板）／信息实例 | 所有 PS |
| $I_{\mathrm{total}}$ | bit | 结构信息与因果信息的并列记录标签；语义基底与校准未建立前，不视为可直接相加的实测总量 | 概念量 |

**范式突破信息的三层拆分。** 上表把过去混写成一个符号的三个对象拆开，三层的时间位置、可观测性与用途都不同，混用会导致循环论证。

**第一层，候选范式突破信号 $\tilde I_{\mathrm{orig}}$。** 定义为现有解码器 $D_n$ 在目标上的预测残差 $\varepsilon_{\mathrm{res}}$ 相对于该解码器历史残差分布 $B_n$ 的稀有度：$\tilde I_{\mathrm{orig}}\equiv-\log_2\Pr_{B_n}(\varepsilon_{\mathrm{res}}\ge\varepsilon_{\mathrm{obs}})$。它是**事前**量，只用 $D_n$ 自己的历史行为就能算出，不需要先知道跃迁是否成功。使用前须做四件事：预注册显著性水平 $\alpha_0$（例如 $\alpha_0=10^{-3}$，对应 $\tilde I_{\mathrm{orig}}\ge 9.97$ bit 的门槛）；预注册残差分布 $B_n$ 的构造方式（滑动窗口长度、是否剔除异常段、是否分层）；预注册**误报率规则**——在 $N$ 次独立门控中容许的误报次数上限 $N\alpha_0$，并规定连续 $k$ 次超过门槛才判定为候选信号（$k$ 亦预注册），以抑制单次噪声触发的假阳性；预注册**分辨率条件**——参考分布 $B_n$ 的样本量 $N_B$ 须满足 $N_B\alpha_0\gtrsim10$（$\alpha_0=10^{-3}$ 时 $N_B\gtrsim10^4$），否则该门槛不可分辨（经验分布把可报读数封顶在 $\log_2N_B$，小计数处另有同量级偏差），须改用参数化尾模型，或按实际可分辨上限下调 $\alpha_0$；每次读数旁须标注 $N_B$ 与尾估计方式。四项锁定之后，$\tilde I_{\mathrm{orig}}$ 才是可复核的门控读数；未锁定的稀有度读数只是描述性统计。

**第二层，经验证的新增信息 $I_{\mathrm{orig}}$。** 只有跃迁已经发生、且新增能力被独立复现之后才追认：它记录“这次跃迁究竟带来了多少此前不存在、且可被独立检验的有效因果信息”。这是**事后**量，用于记账、比较与理论校准，不能反过来当作跃迁的输入条件。

**第三层，拓扑跃迁事件 $\mathcal{T}$。** 这是事件本身而非信息量：新因果维度被打开、$I_{\mathrm{max}}(D_{n+1})>I_{\mathrm{max}}(D_n)$、深度指数加一，由跃迁前后的解码器状态比对判定。

**只有第一层能进门控。** 因为只有 $\tilde I_{\mathrm{orig}}$ 在跃迁之前就有定义且可算。用 $I_{\mathrm{orig}}$ 门控会形成循环（要先知道跃迁成功才能算出信号），用 $\mathcal{T}$ 门控等于用结果预测结果。同时须写明一条限制：**代理读数超过门槛，不等于跃迁必然发生**。残差稀有只说明现有解码器在该目标上明显失灵，失灵可能来自噪声、分布漂移、测量故障，也可能来自真正的新维度；门控只筛出“值得投入试错成本”的候选集，跃迁是否发生仍取决于后续的构造、验证与资源条件。其用途是把有限的 $E_{\mathrm{build}}$ 集中到少数候选上，而不是宣布突破已经到来。

#### 2.1.1 信息是关系量，不是绝对量

$I$ 在 SRVD 中是持久结构通过解码器 $D$ 所能提取的有效差异量。$I_{\mathrm{net}}$ 的大小不仅取决于环境中存在的潜在信息 $I_{\mathrm{latent}}$，更取决于 $D$ 的结构特征。

同一物理构型对不同解码器呈现完全不同的信息价值：氧气对人类是 $I^{+}$，对厌氧菌可能是 $I^{-}$，可见光电磁波对先天失明者接近 $I^{0}$。因果效力是拓扑构型与解码器结构之间匹配程度的度量。由此得到一条推论：在当前的认知与测量框架下，跨解码器的 $I$ 绝对数值不可直接比较——“石头有多少 bit，人有多少 bit”不是有意义的同域提问，除非未来建立起跨解码器的统一参照系。“信息量更大”的陈述必须附带“在何种解码器下”，否则不完整；$I$ 的边界随解码器升级而扩展，打开此前不可达的信息维度。

#### 2.1.2 存续势的比较规则

传统信息论试图以 $I = \log_2 \Omega$ 对所有结构作一维绝对排名，原则上不可行，因为不同系统的状态空间不在同一坐标系内。这一限制精确化为关于 $V$ 的比较规则。

**存续势不是脱离解码器就有的量。** $V$ 的任何取值本质上都是 $V_D(P)$：某个持久结构 $P$ 相对于某个读数者 $D$ 的存续势。正文未特别注明参照解码器时，$V_{\mathrm{obj}}$ 指相对于宏观读数协议 $D_{\mathrm{macro}}$ 的存续势，不是脱离一切解码器、独立存在的绝对理论量。比较只能在明确参照解码器之后进行，其合法性由解码器、测量协议与环境三者的固定状态共同决定。

| 比较类型 | 条件 | 合法性 | 语义 |
| :------- | :--------------------- | :----------- | :------------------ |
| $V_D(P_1)$ 对 $V_D(P_2)$ | 同一解码器、协议、环境、观察窗与分析尺度；信息定义及能量归属一致 | 条件合法 | 还须能量构成可比或已独立校准，否则不作定量排序 |
| $V_{D_A}(P_A)$ 对 $V_{D_B}(P_B)$ | $D_A \ne D_B$，未做解码器映射 | 未定义 | 不同测量系统的数值不可比 |
| $V_D(P_A)$ 对 $V_D(P_B)$ | 已映射至共同参照解码器 $D$ | $V_{\mathrm{s}}$ 合法；$V_{\mathrm{c}}$ 未定义 | $V_{\mathrm{s}}$ 可在统一物理测量下排序；$V_{\mathrm{c}}$ 待广义 $D_{\mathrm{macro}}$ 建立 |
| $\mathrm{d}\ln V / \mathrm{d}t$ 比较 | 时间参数化与 $V$ 的定义具有一致的物理语义 | 尺度鲁棒的候选指标 | 对乘法常数重标度不变，不扩展到非线性重定义 |

**宏观读数协议 $D_{\mathrm{macro}}$。** 经典物理隐含采用的理想化宏观读数协议（国际单位制、孤立系、无测量扰动），可充当部分跨主体比较的公共测量坐标，分两层：**狭义 $D_{\mathrm{macro}}$** 直接采用经典物理测量规则，覆盖 $V_{\mathrm{s}}$ 中 $I_{\mathrm{struct}}, T_{\mathrm{struct}}, E_{\mathrm{struct}}$ 的测量，但跨主体定量比较还须统一对象边界、观察窗、信息操作化定义与能量归属口径，并要求能量构成可比或已有校准——共同单位与协议是必要条件，不是充分条件；**广义 $D_{\mathrm{macro}}$** 是经典测量逻辑的自然延伸，尝试覆盖 $V_{\mathrm{c}}$ 中的 $I_{\mathrm{causal}}, T_{\mathrm{causal}}, E_{\mathrm{causal}}$，这些量最终都表现为物理效应，理论上存在测量可能，但当前缺乏统一的操作化协议，$V_{\mathrm{c}}$ 的跨主体比较因此按“未定义”处理。

$D_{\mathrm{macro}}$ 是 $V_{\mathrm{obj}}$ 这一记法本身默认参照的读数协议：脱离一切解码器的 $V_{\mathrm{obj}}$ 不存在，不存在一个先于它而独立成立、等待被“赋予”的客观量。操作层面，$V_{\mathrm{obj}}$ 只能通过具体测量去逼近其在 $D_{\mathrm{macro}}$ 下的理论取值；测量成本极高时评估精度受 $E_{\mathrm{causal}}$ 约束，各方无法就关键参数达成共识时，有效的 $V_{\mathrm{obj}}$ 可能远低于物理载体完好时的理论上限。$D_{\mathrm{macro}}$ 是理想化协议而非持久结构，不适用 $V(D)$，具体读数总由某个持有者或测量装置执行并承担代价。

**跨观察尺度不可公度。** 若两个观察尺度 $S_A \ne S_B$ 使系统采用不同的粗粒化截断频率或测量协议，则 $\Delta V = V(\cdot\mid S_A)-V(\cdot\mid S_B)$ 未定义；该限制不因引入 $D_{\mathrm{macro}}$ 而消失，除非协议已显式统一尺度。未建模误差只有在比较对象受同一类乘性偏差、且偏差以相同方式作用于各能量分项时才可能抵消，不会自动抵消。

**定量比较的规定。**（1）域内定量：只有同一系统类型内、且边界／解码器／协议／环境／观察窗／尺度／操作化定义／成本归属一致、能量构成相近或经独立校准时，才可比较相对数值。（2）跨域定性：跨系统类型只允许定性陈述（如“两者均满足 $\alpha/\gamma>1$”），禁止并列比较三个指数的数值。（3）$V_{\mathrm{s}}$ 的条件性跨主体比较：固定狭义 $D_{\mathrm{macro}}$ 与上述各项后，还须操作化定义与能量归属口径一致，跨物种的共同单位本身不足以支持直接排序。（4）$V_{\mathrm{c}}$ 当前未定义，需要广义 $D_{\mathrm{macro}}$。跨主体的绝对 $V_{\mathrm{obj}}$ 排序不成立（见 §10.5）。

### 2.2 $E$ 家族（能量家族）

$E$ 家族量化持久结构在存续过程中支付的各种能量成本，基本单位为 $\mathrm{J}$。

| 符号 | 定义 | 关系与边界 |
| :------ | :------------------------- | :------------------------- |
| $E$ | 广义能量，能量家族的父变量 | — |
| $E_{\mathrm{barrier}}$ | 势垒相关的结构成本分摊：按声明规则分配到目标观察窗的成本，不等同于势垒高度 | 势垒高度另记 $\Delta U_{\mathrm{barrier}}$ |
| $E_{\mathrm{survival}}$ | 观察窗内用于主动维持结构组织的能量积分 | 三分解下是 $E_{\mathrm{struct}}$ 的子项，不得与完整 $E_{\mathrm{struct}}$ 重复相加；功率另记 $\dot E_{\mathrm{survival}}$ |
| $E_{\mathrm{causal}}$ | 观察窗内归属于指定持有者、用于读出或处理目标因果效果的能量成本 | 可拆为 $E_{\mathrm{compute}}+E_{\mathrm{refresh}}$；不自动纳入持有者全部代谢，不与 $E_{\mathrm{struct}}$ 重复计量 |
| $E_{\mathrm{struct}}$ | 观察窗内归属于结构通道、用于维持目标 PS 可辨识组织的能量成本 | 三分解下 $E_{\mathrm{struct}}=E_{\mathrm{barrier}}+E_{\mathrm{survival}}$；下界另记 $E_{\mathrm{struct}}^{\min}$ |
| $E_{\mathrm{flow}}$ | 观察窗内累计的活动能量预算（J）；“流”指累计核算，不表示功率 | 基线小计 $E_{\mathrm{survival}}+E_{\mathrm{causal}}$；不再作为独立项加到 $E_{\mathrm{eff}}$；瞬时功率记 $\dot E_{\mathrm{flow}}$ |
| $E_{\mathrm{eff}}$ | 指定核算边界与观察窗内，维持目标 PS 及其所声明因果通道的完整等效热力学成本 | 基本式 $E_{\mathrm{struct}}+E_{\mathrm{causal}}$；仅当同窗、同范围、分项互斥且覆盖完整时可展开为三项之和 |
| $E_{\mathrm{struct}}^{\min}$ | 指定边界与观察窗内维持结构通道所需的最小能量 | 只与 $E_{\mathrm{struct}}$ 同口径比较；不是总成本下限，不用于标记单 bit 擦除下界 |
| $\mathcal{E}_D$ | 进入逻辑操作率上界的解码器物理系统平均能量尺度（J） | 不等于累计的 $E_{\mathrm{eff}}$ 或 $E_{\mathrm{causal}}$；系统边界须先声明 |
| $E_{\mathrm{available}}$ | 系统在声明边界内可获得的最大自由能预算 | 与 $E_{\mathrm{thresh}}$ 作用不同，大小关系不预设；若需区分环境供给上限，记 $E_{\mathrm{max}}$ 且 $E_{\mathrm{available}}\le E_{\mathrm{max}}$ |
| $E_{\mathrm{floor}}$ | 总等效成本下界：$E_{\mathrm{eff}}\ge E_{\mathrm{floor}}\ge E_{\mathrm{struct}}^{\min}>0$ | 与 $E_{\mathrm{struct}}^{\min}$ 不同：后者只是结构通道下限 |
| $E_{\mathrm{thresh}}$ | 损伤触发阈值：模型中不可逆损伤项的触发条件 | 只有与 $E_{\mathrm{eff}}$ 同一边界、同一观察窗及相容定义时才可直接比较；物理机制与校准待建立 |
| $E_{\mathrm{build}}$ | 建造成本：创建新结构或升级现有结构的一次性物理能量 | 由 $L_{\mathrm{lev}}$ 单独评估，不进 $V$ 的动力学公式 |
| $E_{\mathrm{compute}}$ | 计算（含擦除）能耗 | 仅对可计量的逻辑不可逆擦除适用朗道尔下界 |
| $E_{\mathrm{refresh}}$ | 维持（刷新、纠错、保真）能耗 | 只在含可计量逻辑不可逆擦除时适用相应下界；一般刷新下界未建立 |
| $E_{\mathrm{decode}}$ | 认知解码活动的功能标签（暂定） | 尚无独立、非重叠的物理分项，只作功能标注，不独立加总 |

**窗口、嵌套与势垒高度。** 用于单一 $E_{\mathrm{eff}}$ 的各分项必须对应同一声明观察窗、同一核算范围，并按明示规则互斥分配。$E_{\mathrm{survival}}$ 不是与完整 $E_{\mathrm{struct}}$ 并列的额外成本；三分解成立的前提正是 $E_{\mathrm{struct}}=E_{\mathrm{barrier}}+E_{\mathrm{survival}}$ 且三分项覆盖同一范围、彼此不重叠，于是 $E_{\mathrm{eff}} = E_{\mathrm{barrier}}+E_{\mathrm{survival}}+E_{\mathrm{causal}}$。$E_{\mathrm{barrier}}$ 是按模型分摊的结构成本，不是微观跃迁势垒高度（后者记 $\Delta U_{\mathrm{barrier}}$）。一次性建造或写入成本若要纳入存续势，须声明全额计入、按寿命分摊，或仅作历史成本另报。若结构维持与因果处理共用一份能耗，须按可复核的功能或增量成本协议分摊；无法分摊时应保留为合并成本并暂停相应分项或 $V$ 的数值计算，而不是两边全额计入。$E_{\mathrm{survival}}$ 必须是窗口内的能量积分而非功率。被动相仅在 $E_{\mathrm{causal}}=0$ 且结构成本口径一致时，才有 $E_{\mathrm{eff}}=E_{\mathrm{struct}}=E_{\mathrm{barrier}}$。

**$E_{\mathrm{barrier}}$ 的比较规则。** $E_{\mathrm{barrier}}$ 是维持结构有序性、抵抗熵增抹平的势垒成本。在 $I$ 与 $T_{\mathrm{struct}}$ 相同时，$E_{\mathrm{barrier}}$ 越低 $V$ 越高；若势垒变化同时改变 $T_{\mathrm{struct}}$，则属于不同 $(I,T,E)$ 组合之间的权衡，不是“增加势垒让 $V$ 上升”的普遍规律。

**$E_{\mathrm{causal}}$ 的计量边界与社会扩展。** 基础定义是观察窗内归属于指定持有者的实际因果处理能耗；具体模型可按操作类型拆为 $E_{\mathrm{compute}}+E_{\mathrm{refresh}}$，须保证分项互不重叠并覆盖同一窗口与持有者边界。若同一物理系统同时承担结构维持与因果处理，不得把整项代谢或运行能耗同时全额计入 $E_{\mathrm{struct}}$ 与 $E_{\mathrm{causal}}$，应以操作级计量或明示的增量成本协议分摊，不能可靠区分时标注分解不可识别。$E_{\mathrm{decode}}$ 目前只是功能标签，其与 $E_{\mathrm{causal}}$ 可量化子项的关系尚未建立，且可能与计算、刷新分类重叠；没有操作定义、共同窗口、持有者边界与去重规则时不得再相加。购买、保存等非能量支出本身不是能耗，只作资格证据。对由人群组成的社会、经济系统，可在声明的复合核算范围内把持有者群体为目标产出付出的活动能耗（劳动、组织运行）按操作类型计入 $E_{\mathrm{causal}}$，须同时声明持有者范围、共同窗口与重复项去除；未声明时，劳动耗散、军备与组织内耗只作定性示意。

**稳态耗散结构的退化。** 稳态耗散结构以平均功率 $\dot E_{\mathrm{avg}}$ 维持时，窗口内的结构能量成本可估为 $E_{\mathrm{struct}} \approx E_{\mathrm{barrier}} + \dot E_{\mathrm{avg}}\,T_{\mathrm{struct}}$，于是

$$
V_{\mathrm{s}} = \frac{I\,T_{\mathrm{struct}}}{E_{\mathrm{barrier}} + \dot E_{\mathrm{avg}}\,T_{\mathrm{struct}}} \;\xrightarrow{\;E_{\mathrm{barrier}} \to 0\;}\; \frac{I}{\dot E_{\mathrm{avg}}}
$$

对这类结构 $T_{\mathrm{struct}}$ 被约去，$V$ 退化为信息与功率之比（燃料受限的恒星是特例：$T_{\mathrm{struct}}$ 等于燃料储量除以 $\dot E_{\mathrm{avg}}$），$T_{\mathrm{struct}}$ 的独立作用主要体现在势垒型结构与存储刷新上。同类数据中若 $E \propto T$，幂律回归只能识别 $\beta-\gamma$。

### 2.3 $T$ 家族（时间家族）

$T$ 家族量化持久结构涉及的各种时间尺度，基本单位为 $\mathrm{s}$。

各时间量的定义如下：$T_{\mathrm{struct}}$ 为观察窗内结构保持可辨识的时间，$T_{\mathrm{struct}}^{\max}$ 为模型估计的寿命上界（“极端存续上限”一律用这个记号），$T_{\mathrm{causal}}$ 为目标效果可识别、产生响应且持有者付出可测代价的时间总长，$T_{\mathrm{pred}}$ 为内生时间视界，$T_{\mathrm{min}}$ 为最小物理或计算时间粒度，$T_{\mathrm{env}}$ 为环境特征时间，$t_{\mathrm{refresh}}$ 为存储刷新周期；全部单位与汇总见附录 A。

环境温度记 $T_{\mathrm{thermo}}$（单位 $\mathrm{K}$），与时间尺度 $T_{\mathrm{env}}$（单位 $\mathrm{s}$）严格区分。未加上标的 $E_{\mathrm{struct}}$、$T_{\mathrm{struct}}$ 分别表示给定协议与观察窗下的实测结构成本与存续时间；理论下界与上界写作 $E_{\mathrm{struct}}^{\min}$ 与 $T_{\mathrm{struct}}^{\max}$，用于潜力估算时须显式使用带上标的界限量，不得把上下界估算值当作实测值直接比较。

**时间符号规则。** $V_{\mathrm{obj}}$ 是客观量，用 $T_{\mathrm{struct}}$（结构通道）与 $T_{\mathrm{causal}}$（因果通道）；$V^{\mathrm{virt}}$ 与 $V^{\mathrm{val}}$ 是预测量，认知通道用 $T_{\mathrm{pred}}$。**$T_{\mathrm{causal}}$ 描述实际效果持续多久，$T_{\mathrm{pred}}$ 描述系统能看多远，两者不可互换。**

**$T_{\mathrm{pred}}$ 的物理地位。** 经典力学中时间 $t$ 是外生坐标参数；在 SRVD 的主动相中，$T_{\mathrm{pred}}$ 是系统内部的状态变量，可通过认知规划延长，也可在短视压力下坍缩到 $T_{\mathrm{min}}$。它在生命系统中呈连续谱系：细菌趋近 $T_{\mathrm{min}}$（$T_{\mathrm{pred}}\to 0^{+}$），植物可预测数天至数月（$10^{0}\sim 10^{2}$ 天），人类与高阶认知系统可预测数年至数十年（$\gg 1$ 年）。所有具备自主代谢与遗传模板的生命系统都有 $T_{\mathrm{pred}} > T_{\mathrm{min}}$，但极低认知生命紧贴下限。

**时间视界约束：**

$$
T_{\mathrm{min}} < T_{\mathrm{pred}} \le \min(T_{\mathrm{struct}}^{\max},\, T_{\mathrm{env}}) \tag{I-2.2}
$$

内生时间视界不能超过结构的客观物理寿命，也不能超过环境的特征时间尺度。系统把 $T_{\mathrm{pred}}$ 设定得超出这一上界时，会产生脱钩偏差 $\Delta_{\mathrm{VV}}$。

![图 Ⅰ-4　内生时间视界：上界与双维刻画](figures/release/G3_内生时间视界.pdf)

**图 Ⅰ-4　内生时间视界：上界与双维刻画。** 内生时间视界受 $T_{\min} < T_{\mathrm{pred}} \le \min(T_{\mathrm{struct}}^{\max}, T_{\mathrm{env}})$ 约束；视界长度 $L_{\mathrm{pred}}$ 与时间分辨率 $G_{\mathrm{pred}}$ 是两个正交分量，可同时长且细、短且粗。$T_{\mathrm{pred}}$ 不等同于经典时间 $t$，也不可与 $T_{\mathrm{causal}}$ 互换。概念图，不含数值。

### 2.4 $V$ 家族（存续势家族）

$V$ 家族量化持久结构的存续效率、自我评估与行为驱动，基本单位为 $\mathrm{bit \cdot s / J}$。

各存续势量的定义与公式：$V$ 为存续势（正式记号，低阶近似 $V\approx I\cdot T/E$），$V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ 为客观存续势的记账分解（聚合算子暂定），$V^{\mathrm{virt}}$ 为系统经 $D_{\mathrm{cog}}$ 生成的内部模拟值（自我建模特例省略参数，与客观公式同构的双项镜像），$V^{\mathrm{val}}=w_{\mathrm{s}}V_{\mathrm{s}}^{\mathrm{virt}}+w_{\mathrm{c}}V_{\mathrm{c}}^{\mathrm{virt}}$ 为实际优化的行为目标，$w_{\mathrm{s}}+w_{\mathrm{c}}=1$ 分别为生存权重与发展权重，$\Delta_{\mathrm{VV}}=\lvert V^{\mathrm{virt}}-V_{\mathrm{obj}}\rvert$ 为脱钩偏差，$\bar V$ 为同类结构群体的长期平均；单位汇总见附录 A。

**量纲解读。** 在 $I$ 以 bit、$T$ 以 s、$E$ 以 J 计量时，$V$ 的量纲为 $\mathrm{bit \cdot s / J}$，可解释为单位等效热力学成本所对应的信息—时间量。朗道尔关系约束指定逻辑不可逆擦除操作的能量，不会自动授权在存续势公式中消去 bit。若改用“信息比特数为无量纲计数”的约定，必须同步重写 $I$、$V$ 及其边界公式的单位；本书保留 bit 作为显式计量单位，因此存续势的上界也必须保留 bit 因子。除非另行定义参考势并报告 $V/V_0$，不得把 $V$ 本身称为无量纲量。

### 2.5 弹性指数与其他参数

| 符号 | 单位 | 定义 | 适用范围 |
| :-------- | :--------- | :------------------------- | :-------------- |
| $\alpha$ | 无量纲 | 信息弹性指数 $\partial \ln V / \partial \ln I$ | 所有 PS |
| $\beta$ | 无量纲 | 时间弹性指数 $\partial \ln V / \partial \ln T$ | 所有 PS |
| $\gamma$ | 无量纲 | 正向能量弹性指数 $-\partial \ln V/\partial \ln E_{\mathrm{eff}}$；比值 $\alpha:\beta:\gamma$ 是否为不变量待验证 | 所有 PS |
| $\chi$ | $\mathrm{J/(bit\cdot s)}$ | 耦合强度：$I$ 与 $V$ 之间的递归耦合系数 | 仅主动相 |
| $\chi_{\mathrm{c}}$ | $\mathrm{J/(bit\cdot s)}$ | 简化 $I$–$V$ 子系统的临界耦合强度，超过它时正平衡点消失（鞍结分岔） | 仅式 (I-5.12) 子系统 |
| $\gamma_0$ | $\mathrm{s^{-1}}$ | 基线折旧率（与能量弹性指数 $\gamma$ 不是同一个量） | 所有 PS |
| $\rho$ | 无量纲 | 竞争压力指数 | 多主体环境 |
| $\rho_I$ | 无量纲 | 认知投资回报率 $\alpha/\gamma$，与 $\rho$ 是不同的量 | 主动相 |
| $\delta_{\mathrm{dam}}$ | $\mathrm{s^{-1}}$ | 损伤速率 | 触发损伤时 |
| $\delta_{\min}$ | 无量纲 | 操作层预注册的最小效应量（不是竞争压力 $\rho$） | 三层承诺 |
| $L_{\mathrm{lev}}$ | $\mathrm{(bit\cdot s/J)/J}$ | 智慧杠杆系数 $\Delta V / E_{\mathrm{build}}$ | 所有 PS |
| $\mathcal{R}_{\mathrm{e}}$ | $\mathrm{bit/s}$ | 认知处理率 $I_{\mathrm{net}}/T_{\mathrm{pred}}$ | 仅主动相 |
| $\mathcal{L}_{\mathrm{e}}$ | $\mathrm{s/bit}$ | 认知迟滞系数 $T_{\mathrm{pred}}/I_{\mathrm{net}} = 1/\mathcal{R}_{\mathrm{e}}$ | 仅主动相 |
| $\mathcal{Z}_{\mathrm{e}}$ | $\mathrm{bit/J}$ | 因果效率系数 $I_{\mathrm{causal}}/E_{\mathrm{causal}}$，是 $V_{\mathrm{c}}$ 在固定 $T_{\mathrm{causal}}$ 时的正比代理 | 仅主动相 |
| $\alpha_0$ | 无量纲 | 候选范式突破信号门控的预注册显著性水平 | 仅主动相门控 |

强化学习折扣因子记 $\gamma_{\mathrm{RL}}$，与能量弹性指数 $\gamma$ 严格区分；概率函数记 $\Pr$。

**动力学参数**（$k$、$k_I$、$\alpha_{\mathrm{eff}}$、$V_{\mathrm{max}}$、$\alpha_{\mathrm{L}}$、$\sigma$、$\varepsilon_{\mathrm{lr}}$、$k_D$、$k_{\mathrm{s}}$、$\lambda$、$T_{\mathrm{hor}}$、$\psi(\rho)$ 等）均为待标定的模型参数而非测量量，其单位在首次出现的方程处就地列出，汇总见附录 A。

**其余符号**（$r_{\mathrm{v}}$、$g_{\mathrm{net}}$、$\mu_{\mathcal F}$、$\tau_{\mathrm{decay}}$、$\kappa_{\mathrm{topo}}$、$r_{\mathrm{eff}}$、$L_{\mathrm{pred}}$、$G_{\mathrm{pred}}$、$E_{\mathrm{topo}}(D)$ 等）在首次出现的方程处就地给出定义与单位；全部符号及其记账单位统一列于附录 A。

### 2.6 结构同一性判据与 type–token 分离

#### 2.6.1 被动相同一性（适用于无认知解码器的结构）

同一性保持当且仅当：①同一性由参照解码器的辨识类保持（载体可更换；被动相下时空边界连续是其充分条件）；②$I_{\mathrm{struct}}$ 渐进演化，无瞬间全局重排；③结构能量不低于维持下限，$E_{\mathrm{struct}} \ge E_{\mathrm{struct}}^{\min}$。

**辨识判据与检出下限。** 读数者（解码器或公共读数协议）的辨识判据含读数检出下限：结构读数低于该下限时，读数者无法把 $P$ 辨识为同一结构，同一性即告结束。检出下限属读数者一侧，与主动相判据中属结构一侧的维持阈值 $I_{\mathrm{min}}$ 不是同一个量。

结构瓦解有两种物理机制，需严格区分：**外力破坏**——外部高能输入导致的拓扑瓦解，属负效信息 $I^{-}$ 路径，表现为 $I_{\mathrm{struct}}\to 0$；**能量饥饿**——$E_{\mathrm{struct}}<E_{\mathrm{struct}}^{\min}$ 导致的热力学失稳。

**三种事件不得共用一个 0。** 外力破坏与能量饥饿是对象侧的物理失效；读数跌破检出下限是测量侧的识别失败。三者可能都表现为记录里的一个 0 或一个空缺，但含义不同：外力破坏后 $I_{\mathrm{struct}}$ 真实归零；能量饥饿时 $I_{\mathrm{struct}}$ 可以先保持为正，失效的是 $E_{\mathrm{struct}}\ge E_{\mathrm{struct}}^{\min}$；检出下限之下，结构可以完好无损，只是当前协议读不出。

因此，报告记录时须为每项读数附状态（正常取得／实测为零／低于检出下限／在定义下不可定义／未取得），并注明失效原因（外力破坏／能量饥饿／测量失败／其他／未判定）。状态标记是记录元数据：不进入任何方程，不进入 $V$ 的计算，不改变 $I_{\mathrm{struct}}$、$E_{\mathrm{struct}}$ 与两条存续时间的定义。它只防止把“读不出”写成“没有了”。

#### 2.6.2 主动相同一性（适用于有认知解码器的结构）

在满足被动相条件的基础上，附加以下条件。**前四条任一失效，即宣告结构不再保持同一性**；末条 $T_{\mathrm{pred}}>T_{\mathrm{min}}$ 是**主动相标志，不属于同一性条件**——同一性只指持久结构可被识别（即卷Ⅳ §2.2 的四项资格条件），把它与“健康态”分开：

| 条件 | 操作化指标 | 物理含义 |
| :---------------- | :------------------ | :----------------------- |
| $I_{\mathrm{struct}} \ge I_{\mathrm{min}}$；因果通道启用时 $I_{\mathrm{causal}}$ 另须不低于其维持阈值 | 已声明通道的信息量不低于维持阈值 | 拓扑连续性得以维持 |
| $E_{\mathrm{eff}} \le E_{\mathrm{thresh}}$ | 同一观察窗与核算边界下累计等效成本未超过损伤触发阈值 | 按现象学模型未触发损伤项；物理机制与校准待建立 |
| $T_{\mathrm{pred}} > T_{\mathrm{min}}$（**主动相标志，非同一性条件**） | 内生时间视界未坍缩 | 尚未进入短视失控态；失效不意味着结构不再“是同一个”，只意味着进入主动相的短视区 |
| $\Delta_{\mathrm{VV}} \le \delta_{\mathrm{tol}}$ | 脱钩偏差在预注册容差内；$\delta_{\mathrm{tol}}$ 按对象域设定，随报告给出 | 未被虚拟势幻觉俘获 |
| $D$ 未发生根本性漂移 | 解码器仍提取原始因果信息 | 语义同一性得以保全 |

表中第二行的作用方式是：$E_{\mathrm{eff}} > E_{\mathrm{thresh}}$ 并不等于“同一性立即失效、$V$ 立即归零”。它是动力学分支的切换条件，触发之后 $V$ 的走向取决于净增长率与损伤速率的相对大小，可能衰减至零，也可能落到一个较小的正平衡上。这条区分在讨论损伤动力学时必须保留，否则会把条件结论读成无条件结论。

**同一性判定相对于解码器，不等同于身份本身相对。** 上表末条要求 $D$ 未发生根本性漂移，这意味着同一性判定依赖解码器自身的连续性。同一对象若被两个合格解码器读数，可能得到不同判定：以功能因果组织为辨识依据的 $D_1$ 判其连续，以内部模块组织为依据的 $D_2$ 判其已被取代。

此时应逐解码器报告判定，而不是替读者选一个结论。族层面的聚合规则——全体一致、多数、至少一个——都还没有论证，不得默认其中任何一种；多解边界的报告规则不能直接移植为身份判定的聚合规则。

可以确定的是：**同一性判定具有解码器相对性；对象的本体身份是否具有解码器相对性，现有文本不支持。** 判定分歧不证明对象在本体上同时既是原对象又不是原对象。

另有一条接口，与 RIF §12.10 的分名口径一致：该节区分读数检出下限、两对象区分容差与本节的结构侧下限 $I_{\mathrm{min}}$。三者分属两侧，不可互换；“本协议不能区分两个候选”不等于“两个候选是同一个结构”。

#### 2.6.3 type–token 分离

**type（类型）**：可继承的信息模板（如 DNA 序列），由 $I_{\mathrm{struct}}$ 与 $I_{\mathrm{latent}}$ 的稳定部分共同刻画；此处是并列描述，不表示二者可直接数值相加。**token（实例）**：具体个体，由 $I_{\mathrm{active}}$ 与 $I_{\mathrm{struct}}$ 共同刻画；在语义映射未建立前，不把该写法解释为可测的算术和。

**演化链**：岩石（无分离）→ RNA 复制（原始分离）→ 多细胞生物（个体 token 与 type 分离）→ 物种分化（type 分裂）→ 数字实体（$I_{\mathrm{net}}$ 的 token 与 type 分离）。

同一持久结构允许存在多个物理载体。只要这些载体在结构信息、因果信息与解码器状态上持续满足同一性条件，它们就共同构成同一个持久结构；载体之间出现不可逆的信息分化时，原持久结构发生分叉，形成新的持久结构。

**type–token 分离不消除记录缺口。** type 与 token 的分离解决的是“模板与实例不在同一层次”；它不保证 $I_{\mathrm{struct}}$、$I_{\mathrm{latent}}$、$I_{\mathrm{active}}$ 的读数保留了模板或实例内部的关系组织方式。在固定测量协议下，两个关系组织不同的模板仍可能给出相同的 I–T–E 读数（条件式示意，不是存在证明）；反过来，若某个 $I_{\mathrm{struct}}$ 操作化方案已完整编码关系组织，该方案下就不存在这一缺口。

因此本卷只登记一句范围声明：**关系组织是否被读数保留，取决于操作化方案，不由此处的 type–token 区分保证。** 这一缺口不构成新增第四判据的理由，也不进入 $V$。是否成立，取决于协议，本卷不作普遍断言。

***

## 第三章　存续势的数学结构

### 3.1 低阶近似【命题】

$$
V \approx \frac{I \cdot T}{E} \tag{I-3.1}
$$

其中 $V, I, T, E$ 均为广义概念量。这是 SRVD 的最小持续性假设，即在低阶近似中令弹性指数 $\alpha = \beta = \gamma = 1$。

乘法形式基于三个结构要求：（1）**不可替代性**：$V(I, 0) = 0$，$V(0, T) = 0$；（2）**同向贡献**：在其他变量固定时，$I$ 或 $T$ 任一增加均提升 $V$；（3）在要求对 $I$、$T$ 分别线性、连续可微、可分离的指定假设下，乘积 $I\cdot T$ 是自然基准形式。$\sqrt{IT}$ 等函数也满足边界归零与单调性，但不同时满足线性与可分离性。乘积形式是选定的参考形式，幂律是它的推广。

这三条要求本身就是假设，不是从物理定律推出的定理：第（3）条的“线性”与“可分离”是选择参考形式时加上的技术条件，没有它们，满足归零与单调的函数有无穷多个。因此式 (I-3.1) 的地位是一个**被选定的基准**，价值在于给出量纲锚点与可比较的起点，而不在于它是唯一正确的函数形式。**失效条件**：若在同一系统内测得 $V$ 对 $I$ 与 $T$ 的响应存在显著交互项（例如 $I$ 的边际效应随 $T$ 变化而变号），则乘积形式在该系统内失效，应改用含交互项的幂律或一般函数形式。

**与 viability theory 的分工。** Aubin 传统的 viability 问的是“在给定约束下是否存在永远可行的轨道”，答案是**集合**（viability kernel）；本框架的存续势是一个**标量读数**，问“单位能量代价下维持了多少有效信息与时间”。两者共享“可行”一词，不共享数学对象：本框架不给可行集，也不保证 $V$ 最大化的轨道存在。若要与 viability theory 对接，应把 (I-5.19) 的约束域当作约束集、另行讨论其 viability kernel——本卷不做。

### 3.2 客观存续势：双通道叠加

客观存续势把物理载体维持（$V_{\mathrm{s}}$）与认知因果推演（$V_{\mathrm{c}}$）两个独立通道叠加：

$$
V_{\mathrm{obj}} =
\begin{cases}
V_{\mathrm{s}} + V_{\mathrm{c}}, & E_{\mathrm{struct}} \ge E_{\mathrm{struct}}^{\min} \\[6pt]
\text{未定义（结构维持条件失效）}, & E_{\mathrm{struct}} < E_{\mathrm{struct}}^{\min}
\end{cases} \tag{I-3.2}
$$

结构通道 $V_{\mathrm{s}} = I_{\mathrm{struct}} T_{\mathrm{struct}} / E_{\mathrm{struct}}$。因果通道按下式定义，以避免被动结构在 $I_{\mathrm{causal}}=E_{\mathrm{causal}}=0$ 时出现 $0/0$：

$$
V_{\mathrm{c}} =
\begin{cases}
\dfrac{I_{\mathrm{causal}} T_{\mathrm{causal}}}{E_{\mathrm{causal}}}, & E_{\mathrm{causal}}>0 \\[4pt]
0, & E_{\mathrm{causal}}=0 \land I_{\mathrm{causal}}=0 \\[4pt]
\text{未定义（因果信息有读数但无可归属成本）}, & E_{\mathrm{causal}}=0 \land I_{\mathrm{causal}}>0
\end{cases}
$$

若 $V_{\mathrm{c}}$ 未定义，则 $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ 也不作为单一数值报告。能量核算分解为

$$
E_{\mathrm{eff}} = E_{\mathrm{struct}} + E_{\mathrm{causal}} \tag{I-3.3}
$$

采用三分解时另须满足 $E_{\mathrm{struct}}=E_{\mathrm{barrier}}+E_{\mathrm{survival}}$，且所有分项在同一观察窗与核算范围内互不重叠。

**适用域与阈值。** $V_{\mathrm{s}}$ 的有效性以同一观察窗和结构边界下 $E_{\mathrm{struct}} \ge E_{\mathrm{struct}}^{\min}$ 为前提；$E_{\mathrm{struct}}$ 低于该下限表示结构通道未满足定义中的最低维持能量，在本模型同一性判据下被判为存续条件失效。判据应直接比较结构通道成本与其下限，$E_{\mathrm{eff}}$ 是含因果通道的总成本，不能不加说明地替代该判据；若要定义独立的总成本下限，须另设变量并重新给出物理依据。在结构维持适用域内，$E_{\mathrm{eff}} \le E_{\mathrm{thresh}}$ 表示尚未触发阈值损伤项；若 $E_{\mathrm{eff}} > E_{\mathrm{thresh}}$，$V_{\mathrm{obj}}$ 仍是数值状态变量，其演化切换到式 (I-5.3) 的损伤动力学，而不是把 $V_{\mathrm{obj}}$ 本身替换成文字状态。该阈值只能在对象边界、观察窗与能量定义相容且经实例校准时使用，$E_{\mathrm{thresh}}$ 的微观物理含义与校准仍属开放问题。被动结构按约定 $I_{\mathrm{causal}}=E_{\mathrm{causal}}=0$，故 $V_{\mathrm{c}}=0$、$V_{\mathrm{obj}}=V_{\mathrm{s}}$。

**启用的因果通道**须有可操作化的因果效果与可归属成本；只有建立了实际逻辑不可逆擦除量到因果处理的映射，才可进一步使用 $E_{\mathrm{causal}} \ge E_{\mathrm{compute}} \ge E_{\mathrm{Landauer}}(I_{\mathrm{erased}})$ 这一条件性关系。$V_{\mathrm{c}}$ 还须声明持有者是系统自身还是外部宿主；宿主支付时默认逐持有者报告，不跨宿主直接相加。

**双通道分解是模型级聚合假设。** 式 (I-3.2) 的 $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ 不能仅由能量核算式推出。要给出单一 $V_{\mathrm{obj}}$，须先声明共同核算范围、观察窗与两条通道的归属规则，并明确代价分配与重叠效果去重；否则应分别报告 $V_{\mathrm{s}}$ 与各持有者的 $V_{\mathrm{c}}$，不声称存在唯一聚合值。跨案例数值比较另需满足：同一解码器或已校准至共同参照，且协议、环境、观察窗与分析尺度一致；$I$、$T$ 的操作化定义与能量分摊规则一致；能量构成相近或不同构成间已有独立校准。只有在未建模误差确实以相同乘性偏差作用于各分项时，相对排序才可能抵消该误差，不能假定误差自动抵消；若一个案例主要靠 $E_{\mathrm{barrier}}$ 支撑、另一个主要靠 $E_{\mathrm{survival}}$ 支撑且缺乏校准，则不作数值排序。低阶式 $V \approx I_{\mathrm{net}} T/E_{\mathrm{eff}}$ 是正式记号 $V$ 的低阶近似，与式 (I-3.2) 的记账值不等；该差异不用于判定谁替代谁，它来自聚合算子未定与强度量/广延量混用。差多少可以算：取 $E_{\mathrm{struct}}=E_{\mathrm{causal}}=E$、$I_{\mathrm{struct}}=I_{\mathrm{causal}}=I$、两通道时间同为 $T$，则 (I-3.2) 给 $2IT/E$，而 $I_{\mathrm{net}}T/E_{\mathrm{eff}}$ 给 $IT/(2E)$，**相差 4 倍**。根由是 $I_{\mathrm{net}}$ 的能量份额加权平均是强度量，两通道存续势之和是广延量，两者量纲相同而语义不同，不能互相代入，也不能自动修复信息定义或能量归属的不一致。

**积分解读。** 定义累积存续量 $Q = \int I_{\mathrm{causal}}(t)\,\mathrm{d}t$（$\mathrm{bit\cdot s}$）。对近似稳态系统 $Q \approx I_{\mathrm{causal}}T$，认知通道写为 $V_{\mathrm{c}} \approx Q/E_{\mathrm{causal}}$；只有当研究明确采用粗粒化单分母近似、且结构成本可忽略或能量映射已校准时，才可进一步写成 $V \approx Q/E_{\mathrm{eff}}$。它不是双通道定义的恒等变形。

![图 Ⅰ-5　客观存续势：双通道核算](figures/release/G4_客观存续势双通道核算.pdf)

**图 Ⅰ-5　客观存续势：双通道核算。** 结构通道 $V_{\mathrm{s}}$ 与因果通道 $V_{\mathrm{c}}$ 分别按 $I \cdot T / E$ 记账，只有核算条件满足时才聚合为 $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$；$E_{\mathrm{struct}} \ge E_{\mathrm{struct}}^{\min}$ 是结构维持门槛，门槛不满足时 $V_{\mathrm{obj}}$ 未定义。$V \approx I \cdot T/E$ 是 $V$ 的低阶近似；$V_{\mathrm{obj}}$ 的聚合算子暂定。概念图，不含数值。

### 3.3 弹性指数与核心排序命题

幂律形式是粗粒化层面的经验近似，描述 $V$ 对 $I, T, E$ 的总体响应，不要求从双通道叠加严格推出；双通道分解是更细的通道级描述，两者不在同一描述层级。排序命题在粗粒化层面陈述，不声称对每个通道成立。

#### 3.3.1 弹性指数的定义与物理意义

$$
V = V_0 \left(\frac{I}{I_0}\right)^{\alpha} \left(\frac{T}{T_0}\right)^{\beta} \left(\frac{E_{\mathrm{eff}}}{E_0}\right)^{-\gamma} \tag{I-3.4}
$$

$\alpha, \beta, \gamma$ 是无量纲的**弹性指数**，定义为 log–log 斜率。因括号内均为无量纲比值，$V_0$ 必须具有 $V$ 的量纲；在 $I$ 以 bit、$T$ 以 s、$E$ 以 J 计时，$V_0$ 为 bit·s/J。只有另定义 $v:=V/V_0$ 才得到无量纲指标 $v$，它不能与带单位的 $V$ 混称。

$$
\alpha := \left.\frac{\partial \ln V}{\partial \ln I}\right|_{E,T}, \qquad
\beta := \left.\frac{\partial \ln V}{\partial \ln T}\right|_{I,E}, \qquad
\gamma := -\left.\frac{\partial \ln V}{\partial \ln E_{\mathrm{eff}}}\right|_{I,T} \tag{I-3.5}
$$

式中 $I$ 按用语约定指 $I_{\mathrm{net}}$。由于 $I_{\mathrm{net}}$ 的通道权重 $\varphi$ 取自能量份额，改变 $E_{\mathrm{causal}}$ 会同时移动 $I_{\mathrm{net}}$；估计 $\alpha$、$\gamma$ 时须使用分通道读数或固定 $\varphi$，否则直接能耗效应与权重效应会混杂。弹性指数的含义须分两层：在基准形式下系数恒为 1，这是定义的直接后果，不是经验规律；在一般形式下，$\alpha,\beta,\gamma$ 的具体数值不是普适常数，被视为待验证理论不变量的是比值排序 $\alpha/\gamma>1>\beta/\gamma$，且该排序可能随系统类型、物质载体与能量构成变化。当前更优的分析锚点是认知投资回报率收支平衡面 $\rho_I=\alpha/\gamma=1$，它定义相对于具体系统类型的认知相区间边界。凡涉及弹性指数排序、温区策略差异的内容，均标注为“候选推论”或“待验证假说”；在无独立实验锚点时，不给出弹性指数随温度变化的显式函数形式。

影子价格是给定约束下资源的**边际有效价值**，随局域生存约束大幅波动，与弹性指数不可混淆。

#### 3.3.2 弹性指数的不变量与排序命题【假说】

弹性指数是 log–log 斜率，单纯改变 $I,T,E,V$ 的计量单位不会改变这些斜率：单位换算是分子分母同时平移。会改变估计值的是操作化定义、代理指标、观察域与拟合模型，不是单位。比值与单个弹性指数同样对单位换算不变，差别在于比值在跨系统时可能更稳定，而这份稳定性是经验问题。比值 $\alpha:\beta:\gamma$ 是否构成跨域理论不变量仍待验证，排序命题因此以无量纲比值形式陈述：

$$
\frac{\alpha}{\gamma} > 1 > \frac{\beta}{\gamma} \tag{I-3.6}
$$

这是基于三类资源相对稀缺性的定性猜想：信息是熵增宇宙中最稀缺的资源，能量丰富但需主动获取，时间被动给予、无法生产。它尚未获得第一性原理推导或可靠实证支持，属待验证假说，弹性指数概念本身不受此影响。在只讨论比值的语境中可把 $\alpha/\gamma$ 简写为 $\alpha$、$\beta/\gamma$ 简写为 $\beta$，记号退化为 $\alpha>1>\beta$，这只是记号简写。基准形式 $\alpha=\beta=\gamma=1$ 是度量衡参考点，不是预测公式；$\gamma\approx 1$ 作为独立的经验命题另行检验，其证伪不影响排序命题。

对势函数取全微分，得边际收益等式：

$$
\frac{\Delta V}{V} \approx \alpha \cdot \frac{\Delta I}{I} + \beta \cdot \frac{\Delta T}{T} - \gamma \cdot \frac{\Delta E_{\mathrm{eff}}}{E_{\mathrm{eff}}} \tag{I-3.7}
$$

**资源配置推论（候选推论，依赖排序命题 (I-3.6) 成立）**：**使用前须知**——基线 $\alpha=\beta=\gamma=1$ 使 $\rho_I=\alpha/\gamma=1$，恰好落在主动/被动相界上，对相判别**没有判别力**；序关系 $\alpha/\gamma>1>\beta/\gamma$ 是假设，须单独估计（卷Ⅱ 附录 C.2 同此声明）。（1）**信息优先**——信息增量的获取成本低于 $\alpha/\gamma$ 倍时，优先投资信息而非延长时间；（2）**时间止损**——窗口内无信息增量时，继续维持能量消耗即为净亏损，停滞期必须收缩能耗；（3）**能耗红线**——信息红利耗尽、系统达到最优规模边界后，追加能量将直接导致存续势下降。

若测得表观 $\alpha/\gamma \le 1$，先做预先登记的测量有效性检验：同域重复测量一致、$I$、$T$、$E$ 取自同一窗口与同一协议、代理与目标量的相关性达到登记阈值。检验通过而仍得 $\alpha/\gamma \le 1$，计为排序命题的反例，适用域相应收缩；检验不通过才可诊断为测量失效。阈值在测量前锁定。

#### 3.3.3 弹性指数的恒常性

排序的猜想性不等于数值的恒常性，三种可能性并存：**强假说**（三个指数在所有系统中取相同数值，无直接证据）、**中假说**（在同类系统内恒定、跨类型不同）与**弱假说**（只有 $\alpha/\gamma>1>\beta/\gamma$ 普适，具体数值随系统变化）。当前保留的是弱假说：该排序的成立与否取决于环境参数、物质载体、能量构成与解码器四层条件，在常温、自由能通量充足的环境类中作为候选排序成立，可能在其他温区或无源环境中失效。三个指数数值的恒常性需在统一的信息复杂度度量框架建立后才能判定。

#### 3.3.4 数值精度的现状与局限

当前定量比较的根本限制在于：不同系统类型对 $I$ 的定义方式根本不同，且目前无法在跨域尺度上统一。

| 系统类型 | $I$ 的自然定义 | 测量方式 | 现状 |
| :----------- | :------------------ | :-------------- | :------------- |
| DNA 序列 | 生成该基因组所需的最小编码长度 | LZMA 压缩 | 可测量，域内共识 |
| 神经网络 | 网络参数的有效维度或秩 | 参数计数、Fisher 秩 | 同域内可比 |
| 图像、艺术 | 视觉结构复杂度 | 视觉编码器 | 无成熟定义 |
| 社会结构 | 社会组织复杂度 | — | 完全未定义 |

表中测量方式均为现有代理，不是 $I$ 的唯一或最终协议；代理与 $I_{\mathrm{struct}}$ 本身的关系（如压缩长度对随机序列最大）需在各域内校准。因此域内可作精确的相对数值比较，跨域只允许定性陈述，明确禁止把不同系统类型的 $\alpha, \beta, \gamma$ 数值并列比较。

### 3.4 虚拟存续势

**定义**：虚拟存续势是系统通过自身认知解码器 $D_{\mathrm{cog}}$，对**任意持久结构 $P$**（可以是自身，也可以是其他任意 PS）在**任意指定解码器 $D$** 下的存续势所生成的内部模拟值，记为 $V^{\mathrm{virt}}(P, D)$。它是系统内部预测模型的通用输出接口：系统同样可以用它模拟竞争对手、合作者、猎物或任何其他 PS 在某个解码器下的存续状况，这是博弈、捕食、社会认知等一切“预判他者”行为的计算基础。

$$
V^{\mathrm{virt}}(P, D) = \frac{I_{\mathrm{struct}}^{\mathrm{virt}}\,T_{\mathrm{struct}}^{\mathrm{virt}}}{E_{\mathrm{struct}}^{\mathrm{virt}}} + \frac{I_{\mathrm{causal}}^{\mathrm{virt}}\,T_{\mathrm{causal}}^{\mathrm{virt}}}{E_{\mathrm{causal}}^{\mathrm{virt}}} \tag{I-3.8}
$$

带 $^{\mathrm{virt}}$ 上标的变量都是系统的内部评估值，与客观变量同构但不相等，且均隐含以 $(P, D)$ 为参数；对不同目标结构、不同参照解码器的模拟是各自独立的一组变量。虚拟存续势是系统对某个目标 $(P,D)$ 的**主观认知镜像**，不要求与该目标的客观存续势一致。

**同一视界约定。** (I-3.8) 的因果通道统一记 $T_{\mathrm{causal}}^{\mathrm{virt}}$，而 (I-3.2) 的 $V_{\mathrm{c}}$ 用 $T_{\mathrm{causal}}$ 度量，二者含义不同；若不加对齐，即使预测完全准确，$\Delta_{\mathrm{VV}}$ 也不为零。故约定 $T_{\mathrm{causal}}^{\mathrm{virt}}:=\min(\hat T_{\mathrm{causal}},\,T_{\mathrm{pred}})$——系统只能在自己看得到的窗口内评估因果存续，评估值取客观估计与预测视界的较小者；$\Delta_{\mathrm{VV}}$ 的相减只在这一同一视界上进行。

**自我建模是其中的特例。** 当 $P$ 就是系统自身、$D$ 取自身的解码器 $D_{\mathrm{self}}$ 时，$V^{\mathrm{virt}}(P_{\mathrm{self}}, D_{\mathrm{self}})$ 简记为 $V^{\mathrm{virt}}$。后文的脱钩偏差 $\Delta_{\mathrm{VV}}$ 与短视失控态讨论的都是这一特例：只有 $P=P_{\mathrm{self}}$ 时，$V^{\mathrm{virt}}$ 才能与系统自身的 $V_{\mathrm{obj}}$ 相减、定义偏差，进而驱动自身决策；对其他目标的模拟值不进入 $\Delta_{\mathrm{VV}}$，而作为博弈与社会认知模块的输入。

$V^{\mathrm{virt}}$ 的数值独立于 $V_{\mathrm{obj}}$：系统计算它时输入的是内部模型对各参数的主观估计，由当前认知状态决定，不由外部热力学测量决定。因此即使客观物理参数在恶化，$V^{\mathrm{virt}}$ 仍可能通过乐观估计保持高值甚至继续膨胀。$V^{\mathrm{virt}}$ 与 $V_{\mathrm{obj}}$ 之间的系统性偏差，是认知脱钩、自我欺骗与非理性决策的数学根源。

### 3.5 价值存续势

$$
V^{\mathrm{val}} = w_{\mathrm{s}} V_{\mathrm{s}}^{\mathrm{virt}} + w_{\mathrm{c}} V_{\mathrm{c}}^{\mathrm{virt}}, \qquad w_{\mathrm{s}} + w_{\mathrm{c}} = 1 \tag{I-3.9}
$$

其中 $V_{\mathrm{s}}^{\mathrm{virt}} = I_{\mathrm{struct}}^{\mathrm{virt}} T_{\mathrm{struct}}^{\mathrm{virt}} / E_{\mathrm{struct}}^{\mathrm{virt}}$，$V_{\mathrm{c}}^{\mathrm{virt}} = I_{\mathrm{causal}}^{\mathrm{virt}} T_{\mathrm{pred}}^{\mathrm{virt}} / E_{\mathrm{causal}}^{\mathrm{virt}}$；$w_{\mathrm{s}}$、$w_{\mathrm{c}}$ 为价值目标权重，分别称生存权重与发展权重。

**核心命题（框架命题）：系统实际优化的是 $V^{\mathrm{val}}$。** 当 $w_{\mathrm{s}}$ 与 $w_{\mathrm{c}}$ 发生极端偏置（如 $w_{\mathrm{s}}\to 0$ 且 $\Delta_{\mathrm{VV}}\gg 0$）时，系统可能从“追求客观存续”转变为“追求虚拟的、自毁性的目标”。价值目标权重相变的完整动力学（含阈值条件与稳态分析）有待后续工作。**失效条件**：若在某一系统中，行为选择可完全由 $V_{\mathrm{obj}}$ 的当期梯度解释、且引入 $w_{\mathrm{s}}, w_{\mathrm{c}}$ 后预测力无提升，则该系统内不必引入 $V^{\mathrm{val}}$。

**对称劫持。** 短视失控并非只劫持 $V_{\mathrm{c}}$ 通道：$w_{\mathrm{s}}$ 与 $w_{\mathrm{c}}$ 对称，任何一权被虚拟信号过度加权都可能参与自我劫持，结构通道的主观评估分量 $V_{\mathrm{s}}^{\mathrm{virt}}$ 同样是被劫持的潜在目标。“三重分裂只作用于 $V_{\mathrm{c}}$”是常见误读。

### 3.6 选择动力学：Price 协方差的存续势形式【定理】

前三节给出 $V$ 的静态分解，本节补一条动力学锚点：当结构群体按复制选择演化时，平均存续势的变化率有闭式。**本式为 Price（1970）协方差选择数学的直接应用**；这里不重复其推导，只给出在本框架变量下的读法，并注明它在什么条件下只是恒等式（见本节末）。

设一组结构 $i=1,\ldots,N$，其频率 $x_i$ 满足复制选择方程

$$
\dot x_i\ =\ x_i\left(r_i-\bar r\right),\qquad \bar r\ =\ \sum_j x_j r_j \tag{I-3.10}
$$

若各结构的存续势 $V_i$ 在观察窗内固定，且复制率 $r_i=r(V_i)$ 对 $V$ 严格递增，则平均存续势满足

$$
\frac{\mathrm{d}\langle V\rangle}{\mathrm{d}t}\ =\ \operatorname{Cov}\!\left(V,\,r(V)\right)\ \ge\ 0,
\qquad \langle V\rangle\equiv\sum_i x_i V_i \tag{I-3.11}
$$

**前提**：（i）$V_i$ 在窗口内固定；（ii）$r$ 是 $V$ 的严格递增函数；（iii）群体封闭，无迁入迁出；（iv）$x_i$ 按 (I-3.10) 连续演化。
**结论**：平均存续势单调不减，其变化率恰为 $V$ 与复制率的协方差。
**失效条件**：$V_i$ 随频率变化（频率依赖选择）、存在迁入迁出、或 $r$ 对 $V$ 不单调时，(I-3.11) 不成立。

**证明**：由 (I-3.10)，

$$
\frac{\mathrm{d}\langle V\rangle}{\mathrm{d}t}=\sum_i V_i\dot x_i
=\sum_i V_i x_i\left(r_i-\bar r\right)
=\langle Vr\rangle-\langle V\rangle\langle r\rangle
=\operatorname{Cov}(V,r).
$$

协方差非负由 $r$ 对 $V$ 单调递增给出：两个同时递增的量在同一分布上的协方差不为负（离散情形即切比雪夫和不等式）。

**它证明什么、不证明什么。** 它证明的是“**若**选择按存续势单调进行，**则**平均存续势不得下降”——这是恒等式层面的结果，不是经验预测。它不保证 $r$ 真的随 $V$ 递增，也不保证 $V$ 就是选择实际依据的那个量；后两件属经验问题，见第八章。因此本条称【定理】只就 (I-3.11) 自身而言，不外推到任何现实系统。

***

## 第四章　解码器框架

### 4.1 以解码器为中心的描述原则

SRVD 不直接描述世界，而描述持久结构通过解码器 $D$ 与世界的交互；信息、预测、价值与测量都通过解码过程定义。这是它区别于大多数固定观察框架的根本特征：结构不仅改变自身状态，还改变自己认识世界的方式。

**解码器的物理实体地位。** $D$ 不是数学算子或形而上的解释规则，而是在具体载体上实现、由某个物理系统承载的选择性提取机制，如神经组织或硅基电路。文化、理论或语言层面的解码活动也依赖物理载体，但载体的维持成本须按明确的主体边界单独核算。若在指定窗口内已把解码器的操作映射为 $I_{\mathrm{erased}}(D)$ 个逻辑不可逆擦除，且擦除成本与 $E_{\mathrm{eff}}(D)$ 使用同一核算边界，则可写出条件性下界：

$$
E_{\mathrm{eff}}(D) \ge E_{\mathrm{struct}}(D) + k_B T_{\mathrm{thermo}} \ln 2 \cdot I_{\mathrm{erased}}(D) \tag{I-4.1}
$$

这里 $E_{\mathrm{struct}}(D)$ 与 $E_{\mathrm{eff}}(D)$ 必须采用同一解码器边界与观察窗；$I_{\mathrm{erased}}(D)$ 是该窗口内的实际逻辑擦除量，不等同于维持解码能力所需的 $I_{\mathrm{min}}(D)$。没有擦除映射时，不能从 $I_{\mathrm{min}}(D)$ 单独推出朗道尔成本下界；本式也不保证所有读出、计算或刷新过程均达到该下界。

**测量与观察。** 所有核心变量都依赖具体解码器的定义。观察者本身也是持久结构，任何测量都对应特定解码条件下的信息提取；观测能力受能量成本、时间分辨率与信噪比约束，这些边界由物理信道决定，而非来自任何超物理假设。

### 4.2 信息极性

物理因果交互不等于有效因果信息。信息依据其对系统长期存续相空间拓扑方向的影响分为三类：**正效信息 $I^{+}$**——增加系统长期可达状态空间、增强结构可塑性的输入；**负效信息 $I^{-}$**——损伤结构、引发不可逆熵增或压缩状态空间的输入；**中性噪声 $I^{0}$**——产生物理因果但未映射至存续极性的输入。

**极性的关系性本质。** 信息的物理基础是客观拓扑构型，但其极性由与解码器 $D$ 的关系决定。同一对象对不同解码器可以展现完全不同的极性：一本书对读者提供生存知识（$I^{+}$），同一病毒对宿主细胞造成结构破坏（$I^{-}$），随机噪声无法与任何解码器形成有效匹配（$I^{0}$）。因果效力是拓扑构型与解码器结构之间匹配程度的度量。

**测量论声明（主动相适用）。** 对具备 $D_{\mathrm{cog}}$ 的系统，$I^{+}$ 与 $I^{-}$ 的极性判定是在 $T_{\mathrm{pred}}$ 窗口内基于 $V^{\mathrm{virt}}$ 的预测梯度实时进行的动态标签（前瞻性评估），不是等待 $V_{\mathrm{obj}}$ 实际展开后的回溯性分类；系统依据此标签驱动 $E_{\mathrm{causal}}$ 的分配。当 $\Delta_{\mathrm{VV}}>0$ 时，该前瞻性评估可能系统性偏离客观现实，这种偏离正是短视失控态的动力燃料。

**范式层次。** 在 $I^{+}$ 内部可进一步按解码器拓扑被重构的深度分级。此处必须把三个常被混用的对象分开，其分层已在 §2.1 给出（候选信号 $\tilde I_{\mathrm{orig}}$／事后量 $I_{\mathrm{orig}}$／事件 $\mathcal{T}$），此处只补两点操作后果：**只有第一层能进门控**，因为只有它在跃迁之前有定义且可算，用事后量门控是循环，用事件门控是同义反复；**门控不等于结论**，代理读数过槛只说明现有解码器在该目标上明显失灵，失灵可能源于噪声、漂移、仪器故障、任务不可学，也可能源于真正的新维度，门控筛出的只是“值得投入试错成本”的候选集，其用途是把有限的 $E_{\mathrm{build}}$ 集中到少数候选上并在被证伪时快速止损。

$I_{\mathrm{orig}}$ 与范式解释信息 $I_{\mathrm{interp}}$ 都不是可直接测得的比特数，二者的区分以是否触发解码器拓扑跃迁（$D_{\mathrm{depth}}$ 增加）为候选判据：范式突破信息开辟全新因果维度，边际效能不随复制衰减，可强制重置生态位的拓扑距离；范式解释信息则是在现有范式内作高质量执行或局部参数优化，边际效能随同质化快速衰减（$\Delta I\to 0$）。这一区分是解释人工智能时代同质化危机的物理基础。

![图 Ⅰ-6　信息极性由解码器关系决定](figures/release/G5_信息极性由解码器关系决定.pdf)

**图 Ⅰ-6　信息极性由解码器关系决定。** 同一物理输入不携带固定极性：经解码器 $D$ 映射后可分为正效信息 $I^{+}$（扩大长期可达状态空间）、负效信息 $I^{-}$（损伤结构组织）、中性噪声 $I^{0}$（未映射到存续极性）。极性是面向特定 $D$ 的动态标签，不是信号的固有属性；$I^{+}$ / $I^{-}$ 仅在主动相适用。概念图，不含数值。

### 4.3 与已有框架的关系

SRVD 是粗粒化的宏观动力学框架，不与下列已建立的理论竞争，而是把它们映射为特例或边界输入。

| 框架 | 在 SRVD 中的角色 | SRVD 的扩展与区别 |
| :--------------- | :----------------------- | :-------------------- |
| 热力学第二定律 | 核心约束，不违反 | 描述局域对抗熵增的结构，全局熵增是内在驱动力 |
| 普里戈金（I. Prigogine）耗散结构理论 | 描述主动存续域中 $E_{\mathrm{survival}}$ 主导的区间 | 增加 $E_{\mathrm{barrier}}$ 与 $E_{\mathrm{causal}}$ 分量，并超越近平衡态 |
| Ulanowicz 上升度理论（1997） | $A=T_{\mathrm{ST}}\cdot\mathrm{AMI}$ 与 $V$ 的分子形似，含义不同（$T_{\mathrm{ST}}$ 不是时间） | 提供分母 $E_{\mathrm{eff}}$，使跨底物比较成为可能 |
| Still 等（2012） | 单步时间尺度上的信息—能量效率权衡，与 $V$ 形式同构；不构成 $V$ 公式的推导前提 | $I_{\mathrm{causal}}$ 带极性与解码器相对性；其 $T$ 折在速率里，无独立时间维度 |
| 朗道尔原理 | 提供 $E_{\mathrm{compute}}\ge k_BT_{\mathrm{thermo}}\ln2\cdot I_{\mathrm{erased}}$ 的擦除下界 | 只作 $E_{\mathrm{compute}}$ 的基底，不适用于 $E_{\mathrm{refresh}}$ |
| 自由能原理、广义相对论、量子力学、香农信息论、复杂适应系统理论 | 分别为单一能量通道的局部类比、引力与黑洞热力学的边界输入、朗道尔的微观来源与退相干下界、去极性后的概率极限、规则集—选择—涌现的定性机制 | 本卷或只取其结论作边界输入（不改写原方程），或以 $I_{\mathrm{net}}$ 的解码器相对性与存续极性相区别，或以 $V$ 把适应度标量化 |

***

## 第五章　扩展动力学

### 5.1 五重递归架构

五重递归是 SRVD 描述主动相系统演化的核心架构：$I, V, T, E, D$ 五个变量相互耦合，给出定性的演化图景。低阶被动结构不激活这一架构，其动力学退化为存续势的静态估计。

本节的递归式是**待严格化的启发式离散模型**，价值在于揭示耦合的定性方向与相变的存在性，不是可直接拟合数据的精确函数形式。本章数学基础最扎实的部分是三重分裂的本体论机制与脱钩偏差动力学，它们具备严格的常微分方程形式与显式解。

**线性化假设。** 以下假设各变量间的主导耦合方向是单向的（$I\to V\to T\to E\to D$），对应“快速驱动、慢速响应”的尺度分离。实际系统可能存在双向反馈环路，完整的耦合方程组是开放问题；当前保留为离散递归的一阶近似，供数值示意与定性讨论。

本章两个算子分工明确，不可混用：$\mathcal{F}$ 是**递归展开算子**，在给定拓扑内增加信息，受容量约束；$\mathcal{T}$ 是**拓扑跃迁算子**，更换拓扑本身，一次性支付 $E_{\mathrm{build}}$ 并重置容量。$\mathcal{F}$ 饱和不等于 $\mathcal{T}$ 发生，这是本章多处论证的共同前提。

![图 Ⅰ-7　五重递归：主导耦合链与算子分工](figures/release/G6_五重递归耦合链.pdf)

**图 Ⅰ-7　五重递归：主导耦合链与算子分工。** 本卷采用快—慢尺度分离下的单向离散近似（$I \to V \to T \to E \to D$），$D$ 的更新进入下一轮信息提取；$\mathcal{F}$（递归展开算子）在给定拓扑内增加信息，$\mathcal{T}$（拓扑跃迁算子）改变拓扑本身并支付 $E_{\mathrm{build}}$，$\mathcal{F}$ 饱和不等于 $\mathcal{T}$ 发生。完整双向耦合仍属开放问题。概念图，不含数值。

#### 5.1.1 $I$ 递归（信息自我放大）

$$
I_{\mathrm{net},n+1} = I_{\mathrm{bas}} \left(1 + \chi \cdot V_{\mathrm{obj},n}\right) \tag{I-5.1}
$$

$I_{\mathrm{bas}}$ 是系统在 $V=0$ 时的基线 $I_{\mathrm{net}}$；$\chi$ 为耦合强度，量纲 $[V]^{-1}$（即 $\mathrm{J/(bit\cdot s)}$），以确保 $\chi V$ 无量纲。**$\chi$ 的唯象地位。** $\chi$ 是解码器 $D$ 自身结构特征的内禀属性，唯象地刻画“系统利用当前存续状态的反馈加速信息提取”的自指回路强度，是决定分裂之后走向哪条路径的核心参数。完整的微观推导有待后续工作，当前作为唯象参数处理，取值由系统的统计行为反推。

**数值使用前提。** 式中 $I_{\mathrm{net}}$ 只有在 §2.1 的四项校准条件满足时才作数值状态变量；未满足时只保留序关系解释，不据此报告定量增长率或容量。**适用域。** 线性形式只在 $V_{\mathrm{obj},n}>0$ 的活跃存续域内成立；$V_{\mathrm{obj},n}\le 0$ 时系统已进入结构降解或解体区间，$I_{\mathrm{net}}$ 的演化由耗散失控与损伤项共同决定。需要在全域保持连续与正定时，可改用指数形式 $I_{\mathrm{net},n+1} = I_{\mathrm{bas}} \exp(\chi V_{\mathrm{obj},n})$，它在 $V_{\mathrm{obj},n}\to -\infty$ 时渐近趋于零而不变负；线性形式作为低阶近似保留。

**统一信息演化方程。** 式 (I-5.1) 是离散映射。为与连续时间的衰减、以及离散的拓扑跃迁同时兼容，本卷把信息演化写成**连续流＋离散跳跃**的混合动力系统：

$$
\begin{aligned}
\frac{\mathrm{d}I_{\mathrm{net}}}{\mathrm{d}t}
&= \underbrace{\mu_{\mathcal F}\, I_{\mathrm{net}}\left(1 - \frac{I_{\mathrm{net}}}{I_{\max}(D)}\right)}_{\text{递归展开 }\mathcal F\text{：容量受限的 logistic 增长}}\\
&\quad- \underbrace{\frac{I_{\mathrm{net}} - I_{\mathrm{eq}}}{\tau_{\mathrm{decay}}}}_{\text{热力学衰减：向热背景弛豫}}
\end{aligned}
\tag{I-5.1a}
$$

$$
\begin{aligned}
&\text{跳跃映射（}\mathcal T\text{ 事件）：}\\
&I_{\mathrm{net}}^{+} = I_{\mathrm{net}}^{-} + \Delta I_{\mathcal{T}},\qquad
\Delta I_{\mathcal{T}} \equiv \kappa_{\mathrm{topo}}\,\tilde I_{\mathrm{orig}}\ \text{（待标定）},\\
&I_{\max}(D^{+}) > I_{\max}(D^{-})
\end{aligned}
\tag{I-5.1b}
$$

**分工与去重复。** 连续流 (I-5.1a) 只负责 $\mathcal F$ 展开与热弛豫，跳跃映射 (I-5.1b) 只负责拓扑跃迁造成的信息阶跃与容量重置。同一跳变不得在两项中重复计入；若某实现选择用 (I-5.1b) 表达容量重置，则不得再把它写成 (I-5.1a) 里的连续脉冲项。把一次跃迁同时记成“脉冲增加”与“容量抬升”，会让同一份 $E_{\mathrm{build}}$ 被记两次收益，估值随记账方式漂移。

**无 $\mathcal T$ 时的不动点。** 令 (I-5.1a) 右端为零，取正根得唯一的物理不动点

$$
I_{\mathrm{net}}^{*}
= \frac{I_{\max}(D)}{2\mu_{\mathcal F}}
\left[\,\left(\mu_{\mathcal F} - \tau_{\mathrm{decay}}^{-1}\right)
+ \sqrt{\left(\mu_{\mathcal F} - \tau_{\mathrm{decay}}^{-1}\right)^{2}
+ \frac{4\,\mu_{\mathcal F}\,I_{\mathrm{eq}}}{\tau_{\mathrm{decay}}\,I_{\max}(D)}}\ \right] \tag{I-5.1c}
$$

它是稳定的（$f'(I^{*})<0$）。两个极限情形值得单列：$I_{\mathrm{eq}}=0$（无热背景信息）时 $I^{*} = I_{\max}(D)(1-1/(\mu_{\mathcal F}\tau_{\mathrm{decay}}))$，存在正不动点的充要条件是

$$
\mu_{\mathcal F}\,\tau_{\mathrm{decay}} > 1 \tag{I-5.1d}
$$

即递归展开增益必须快过热弛豫，否则信息单调衰减至零，这是一个可证伪的定量判据；$\tau_{\mathrm{decay}}\to\infty$（无热弛豫）时 $I^{*}\to I_{\max}(D)$，退化为纯 logistic 饱和。

**判据 (I-5.1d) 的三行摘要**：（i）前提——logistic 增长、常数 $\mu_{\mathcal F}$ 与 $\tau_{\mathrm{decay}}$、$I_{\mathrm{eq}}=0$、无拓扑跃迁；（ii）结论——$\mu_{\mathcal F}\tau_{\mathrm{decay}}>1$ 是正不动点存在的充要条件，临界值 $\mu_{\mathcal F}\tau_{\mathrm{decay}}=1$ 处零不动点与正不动点交换稳定性，是**跨临界分岔**（transcritical），不是鞍结分岔；本卷真正的鞍结分岔在 §5.2.3 的 $\chi_{\mathrm{c}}$ 处；（iii）失效条件——若 $I_{\mathrm{eq}}>0$（存在热背景信息注入），则即使 $\mu_{\mathcal F}\tau_{\mathrm{decay}}<1$ 也仍有正不动点，判据须改用 (I-5.1c) 的完整形式。

**动力学解读。** 系统的结构存续状态反馈到解码器的信息提取效率：结构稳定性与冗余度越高，维持复杂预测结构的能力越强，有效因果信息的提取效率随之提升。$\chi$ 过高时，内生虚拟存续势与物理约束解耦，进入非线性膨胀，最终引发短视失控态。

#### 5.1.2 $V$ 递归（存续势更新）

本节的 logistic 方程是**单一演化通道的约化模型**，不是双通道总量 $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ 的普遍动力学。其推导要求结构通道在观察窗内可忽略（$V_{\mathrm{s}}\approx0$），从而 $V_{\mathrm{obj}}\approx V_{\mathrm{c}}$；同时，信息输入须在 §2.1 的域内校准下满足 $I_{\mathrm{net}}\approx I_{\mathrm{causal}}$，否则 (I-5.1a) 的信息状态不能直接映射为因果通道状态；若 $V_{\mathrm{s}}$ 非零但近似恒定，方程至多适用于扣除该固定基线后的演化分量，不能直接把总量 $V_{\mathrm{obj}}$ 代入。结构通道不可忽略或两通道同时变化时，应使用 (I-5.20a) 的分通道记账式，而不套用本节 logistic 轨迹。**$r_{\mathrm{v}}$ 在约化观察窗内取常数（$\mathrm{s^{-1}}$）**，不作为该约化状态的函数。它不是可自由赋值的经验参数：在 (I-5.2) 作为 (I-5.1a) 准静态像的适用范围内，$r_{\mathrm{v}}=\mu_{\mathcal F}$、$\gamma_0=\tau_{\mathrm{decay}}^{-1}$（见本节末“式 (I-5.2) 与 (I-5.1a) 的关系”），资源可得性与该结构的约束几何通过 $\mu_{\mathcal F}$ 与 $I_{\max}(D)$ 进入模型，不另设与之并列的独立驱动率：

$$
\frac{\mathrm{d}V_{\mathrm{obj}}}{\mathrm{d}t} = V_{\mathrm{obj}} \cdot (r_{\mathrm{v}} - \gamma_0) \cdot \left(1 - \frac{V_{\mathrm{obj}}}{V_{\mathrm{max}}}\right) \tag{I-5.2}
$$

在本模型的现象学近似中，若同一核算边界与观察窗下的 $E_{\mathrm{eff}}$ 超过已校准的 $E_{\mathrm{thresh}}$，则触发不可逆损伤项；这一阈值关系不是已知物理定律：

$$
\frac{\mathrm{d}V_{\mathrm{obj}}}{\mathrm{d}t} = V_{\mathrm{obj}} \cdot (r_{\mathrm{v}} - \gamma_0) \cdot \left(1 - \frac{V_{\mathrm{obj}}}{V_{\mathrm{max}}}\right) - \delta_{\mathrm{dam}} \cdot V_{\mathrm{obj}} \cdot \mathbf{1}\left[E_{\mathrm{eff}} > E_{\mathrm{thresh}}\right] \tag{I-5.3}
$$

式 (I-3.2) 定义数值状态 $V_{\mathrm{obj}}$，式 (I-5.3) 在阈值超限时加入连续时间损伤项；阈值是动力学分支的切换条件，不是把状态变量替换为文字。若将 (I-5.3) 用于实际轨迹，必须预先声明 $E_{\mathrm{eff}}(t;W)$ 的核算窗口 $W$ 是固定、滚动还是累计至时刻 $t$，并说明窗口重置规则；未规定时只能用于指定窗口的静态诊断，不能声称已确定瞬时触发时刻。

**触发之后 $V$ 不会自动归零。** 把阈值指示函数写成“一旦超限就 $V\to 0$”是错的：式 (I-5.3) 在触发域内仍有增长项、饱和项与损伤项，它自己的不动点决定 $V$ 的去向。触发域内的有效净增长率是 $r_{\mathrm{net}}\equiv r_{\mathrm{v}}-\gamma_0-\delta_{\mathrm{dam}}$，统一写作 $g_{\mathrm{net}}\equiv (r_{\mathrm{v}}-\gamma_0)-\delta_{\mathrm{dam}}\mathbf{1}[E_{\mathrm{eff}}>E_{\mathrm{thresh}}]$，触发域内 $g_{\mathrm{net}}=r_{\mathrm{net}}$。据此必须分三种情形陈述。

**情形（a）：$0\le r_{\mathrm{v}}-\gamma_0<\delta_{\mathrm{dam}}$（归零型）。** 在约化模型的正状态域内，有效净增长率为负，括号内的“增长减损伤”在 $0<V\le V_{\mathrm{max}}$ 上为负，故对任意正状态 $\mathrm{d}V/\mathrm{d}t<0$，$V$ 单调衰减至 0。这是真正的崩溃情形：损伤速率压过净增长率，结构无论多大都救不回来，衰减初始速率约为 $\delta_{\mathrm{dam}}-(r_{\mathrm{v}}-\gamma_0)$。$r_{\mathrm{v}}-\gamma_0=\delta_{\mathrm{dam}}$ 是临界边界，此时 $\mathrm{d}V/\mathrm{d}t = -(r_{\mathrm{v}}-\gamma_0)V^{2}/V_{\mathrm{max}}$，衰减由指数型转为代数型（$V\sim V_{\mathrm{max}}/((r_{\mathrm{v}}-\gamma_0)t)$），仍趋向 0，但时间尺度被拉长。

**情形（b）：$r_{\mathrm{v}}-\gamma_0>\delta_{\mathrm{dam}}>0$（降阶型）。** 有效净增长率为正，触发域内存在一个**较小的正平衡**

$$
V^{*} = V_{\mathrm{max}}\left(1 - \frac{\delta_{\mathrm{dam}}}{r_{\mathrm{v}} - \gamma_0}\right) > 0
$$

且它是稳定的：在 $V^{*}$ 处对 $V$ 求导得 $-(r_{\mathrm{v}}-\gamma_0)V^{*}/V_{\mathrm{max}}<0$。因此损伤触发并不必然把 $V$ 打到零，而是把系统推向较低正平衡：若触发时 $V>V^{*}$，则 $V$ 单调下降至 $V^{*}$；若触发时 $0<V<V^{*}$，则 $V$ 单调上升至 $V^{*}$。物理上这对应“带着永久性损伤继续运行”：产能被损伤项吃掉一部分，剩下的刚好维持一个缩小的规模。比值 $1-\delta_{\mathrm{dam}}/(r_{\mathrm{v}}-\gamma_0)$ 是损伤的“折价率”，损伤越强、净增长率越弱，折价越狠；当 $\delta_{\mathrm{dam}}\to r_{\mathrm{v}}-\gamma_0$ 时 $V^{*}\to 0$，情形（b）连续退化为情形（a）。

**情形（c）：$r_{\mathrm{v}}<\gamma_0$ 且阈值已触发（加速崩溃）。** 在约化模型的状态域 $0<V_{\mathrm{obj}}\le V_{\mathrm{max}}$ 内，增长项与损伤项同号：$\mathrm{d}V/\mathrm{d}t = V[(r_{\mathrm{v}}-\gamma_0)(1-V/V_{\mathrm{max}})-\delta_{\mathrm{dam}}]$，方括号内两项皆为负，衰减速率大于任一单项，崩溃被加速。这类系统的损伤是把本已开始的衰退踩到底；其特征是崩溃时间显著短于按单一损伤速率估计的时间。

![图 Ⅰ-8　终局相图与双稳盆地](figures/release/F8_终局相图与双稳盆地.pdf)

**图 Ⅰ-8　终局相图与双稳盆地。**（a）终局 $V/V_{\max}$ 在 $(g_0,\delta_{\mathrm{dam}})$ 平面上的相图，白虚线为 $g_0=\delta_{\mathrm{dam}}$；（b）移动目标的偏差曲线与可接受漂移上限——漂移率达到净增长率的 0.8% 时偏差已超 10%；（c）$\chi=0.9\chi_{\mathrm c}$ 时的双稳盆地，发散初值占 29%。白线右侧整片都是「带伤运行」：阈值触发不等于归零，带伤平台 $V^{*}>0$ 占相当大一片。

**三条情形的共同前提与边界。** 上述分析以 $V_{\mathrm{max}}$、$\delta_{\mathrm{dam}}$、$r_{\mathrm{v}}$、$\gamma_0$ 在观察窗内为常数为前提；任一时变参数都会把不动点变成移动目标，此时只能作分段近似——但“分段近似”须给出量级：以 $\varepsilon$ 记 $r_{\mathrm{v}}$ 的相对漂移率，冻结不动点的预测在 $\varepsilon/g_0\lesssim10^{-2}$ 时与真实轨迹相符（偏差 $<10\%$）；超过这个量级，不动点只能当**瞬时参考**，不能当预测。原因是 $\partial V^{*}/\partial g_0=\delta_{\mathrm{dam}}/g_0^{2}$，在 $g_0\to\delta_{\mathrm{dam}}^{+}$ 时发散。算例：漂移率达到净增长率的 $0.8\%$ 时，预测偏差已超过 $10\%$（附录 F 表 F-6；图 Ⅰ-8(b)）。$V_{\mathrm{max}}$ 本身是待标定参数，因此 $V^{*}$ 的数值也带同样的不确定性；在本卷的定位里，$V^{*}$ 是一个结构性预测（“存在一个非零的低位平台，而不是归零”），不是可直接与实测比对的数值。**失效条件**：若实测轨迹在阈值触发后直接跌至读数下限而没有平台段，则情形（b）在该系统内不成立，应回到情形（a）并检查 $\delta_{\mathrm{dam}}$ 的标定。

**闭环特例（Allee 型）。** 若某类系统确由 $V$ 自身驱动增长，即取 $r_{\mathrm{v}}=k_{\mathrm{v}}V$，则 (I-5.2) 变为 $\dot V=k_{\mathrm{v}}V^{2}(1-V/V_{\mathrm{max}})-\gamma_0V$，出现一个不稳定阈值 $V_{\mathrm{A}}=\tfrac{V_{\max}}{2}\bigl[1-\sqrt{1-4\gamma_0/(k_{\mathrm{v}}V_{\max})}\bigr]$：低于它即使无损伤也趋向零，高于它才升向容量上限（$\gamma_0/k_{\mathrm{v}}$ 只是 $V_{\max}\to\infty$ 的一阶极限，不是阈值本身）。这是另一种动力学，其判据不能套用上面的三情形。上面三条属于「驱动与 $V$ 无关」这一支，本节余下各处的 $r_{\mathrm{v}}$ 一律指这一支的常数；闭环特例是唯一例外，此时 $r_{\mathrm{v}}$ 不再由 (I-5.1a) 的像定出。

$V_{\mathrm{max}}$ 在模型中被设为热力学容量上界，并假定与环境可用自由能通量 $\dot{F}_{\mathrm{avail}}$、最小熵产率 $\sigma_{\mathrm{min}}$ 有关；但本卷尚未给出把这些物理量映射为 $V$ 量纲的校准公式，因此 $V_{\mathrm{max}}$ 当前只能作为待标定参数，不能由上述两个量直接算出。本式的 $V_{\mathrm{max}}$ 即可达 $V$ 的上确界 $V_{\mathrm{max}}(D,S)$，与其标度关系中的 $V_{\mathrm{max}}$ 指同一个量；该标度关系只给比例关系，比例系数待标定。

**两个来源的条件性合并规则。** $V_{\mathrm{max}}$ 有两条候选上界：(I-5.1a) 单通道约化模型给出的信息容量映射，以及 (I-6.7) 的生态位容量标度。只有在两条约束都针对同一状态变量（而非一条约束 $V_{\mathrm{c}}$、另一条约束总量 $V_{\mathrm{obj}}$）、同一系统边界与同一观察窗时，才取较紧者：

$$V_{\mathrm{max}}=\min\Bigl\{\,\zeta_V I^{*},\ \ \alpha_{\mathrm{cap}}\,\dot F_{\mathrm{avail}}/(\sigma_{\min}\gamma_0)\,\Bigr\}$$

$\alpha_{\mathrm{cap}}$ 为 (I-6.7) 的待标定比例系数（下称容量系数），与信息弹性指数 $\alpha$ 无关；$\zeta_V$ 为信息容量到约化存续势容量的比例系数，单位 $\mathrm{s/J}$，须在目标域内标定。第一支中的 $I^{*}$ 取 (I-5.1c) 的正平衡根，只有 $I_{\mathrm{eq}}=0$ 时才化为 $I_{\max}(1-\gamma_0/r_{\mathrm{v}})$。理由：容量上界是“在已声明约束下可达的上确界”；两条约束同时作用于同一状态变量时，可达上界由更紧的一条决定。若状态变量或核算边界不同，取小没有数学意义，须分开报告。若研究对象只受其中一条约束（例如 $I_{\max}$ 由协议给定而生态位通量不受限），须写明“本节只用哪一支”；**不得同时引用两式而不说明**——否则同一个 $V_{\mathrm{max}}$ 会给出两个不同的容量上界，进而使 $V^{*}$ 与饱和态的阈值不可比。

**饱和态。** 系统进入稳定饱和态，当且仅当 $E_{\mathrm{struct}}\ge E_{\mathrm{struct}}^{\min}$、$\rho\to 0$ 与 $\Delta_{\mathrm{VV}}\to 0$ 三个条件同时满足；这些条件连同 $g_0\equiv r_{\mathrm{v}}-\gamma_0>0$ 与约化单通道状态达到其容量上界共同定义该约化模型的饱和流形；只有在 $V_{\mathrm{s}}\approx0$ 时，才可把该状态写作 $V_{\mathrm{obj}}=V_{\mathrm{max}}$。**饱和的条件是 $g_0>0$，不是 $g_0=0$**：$g_0=0$ 时 (I-5.2) 给出 $\mathrm{d}V/\mathrm{d}t\equiv0$，$V$ 停在初值，既非饱和也非崩溃；只有 $g_0>0$ 才使 $V\to V_{\mathrm{max}}$。离散更新形式为

$$
V_{\mathrm{obj},n+1} = \frac{I_{\mathrm{struct}}\,T_{\mathrm{struct}}}{E_{\mathrm{struct}}} + V_{\mathrm{c},n+1} \tag{I-5.4}
$$

其中 $V_{\mathrm{c},n+1}$ 按 §3.2 中 $V_{\mathrm{c}}$ 的分段定义取值：因果通道未启用时取 $0$；若因果信息有非零读数却没有可归属能耗，则该更新值未定义，不直接计算 $0/0$。

**式 (I-5.2) 的地位。** 式 (I-5.2) 是单通道约化状态的轨迹，式中不显含 $I,T,E$；(I-5.12) 是另一个辅助子系统，二者不联立。**式 (I-3.2) 始终是唯一的双通道读数定义**；一般情形下 $V_{\mathrm{obj}}$ 的变化由 (I-5.20a) 分通道记账。只有在 $V_{\mathrm{s}}$ 可忽略、因果通道占主导且相应变量满足冻结条件时，(I-5.2)／(I-5.3) 才可作为 $V_{\mathrm{obj}}\approx V_{\mathrm{c}}$ 的约化轨迹，其系数由 (I-5.1a) 定出（见下一段）。因此完整双通道情形使用 (I-5.20a)，满足前述单通道约化条件时才使用 (I-5.2)／(I-5.3)。凡 (I-5.2)／(I-5.3) 成立之处，$I,T,E$ 的变动已被冻结条件吸收进 $r_{\mathrm{v}}$ 与 $V_{\mathrm{max}}$，不另行对 $V$ 产生动力学作用。完整的约束相图留作后续工作，见第十章开放问题。

**记账恒等式 (I-5.20a)／(I-5.20b)。** 因 (I-3.2) 是 $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ 且 $V_k=I_kT_k/E_k$，先写分通道式

$$
\dot V_{\mathrm{obj}}
=\sum_{k\in\{\mathrm{s},\mathrm{c}\}}V_k\left(
\frac{\dot I_k}{I_k}+\frac{\dot T_k}{T_k}-\frac{\dot E_k}{E_k}\right)
\tag{I-5.20a}
$$

单通道近似 $V\approx I\,T/E$ 时退化为

$$
\frac{\dot V}{V}=\frac{\dot I}{I}+\frac{\dot T}{T}-\frac{\dot E_{\mathrm{eff}}}{E_{\mathrm{eff}}}
\tag{I-5.20b}
$$

两式都是定义的恒等式，不是新假设。不得拿 (I-5.20b) 当 (I-5.20a) 的替代：同一组 $I,T,E$ 下二者数值差 4 倍（§3.2）。

**式 (I-5.2) 与 (I-5.1a) 的关系。** (I-5.2) 是 (I-5.1a) 在准静态极限下的像。在 $V=I\,T/E$ 的单通道基准形式下，且 $I_{\mathrm{eq}}=0$、$I_{\mathrm{net}}\approx I_{\mathrm{causal}}$ 的映射已校准，若结构通道在一个存续势时间尺度内冻结（$\dot I_s=\dot T_s=\dot E_s\approx0$），且因果通道的时间与能耗也冻结（$\dot T_c=\dot E_c\approx0$），则记账恒等式 (I-5.20a) 退化为 $\dot V_c/V_c=\dot I_c/I_c$，即 $V_c\propto I_c$。代入 (I-5.1a) 的连续流形式并与 (I-5.2) 作系数比对，得

$$
r_{\mathrm v}=\mu_{\mathcal F},\qquad \gamma_0=\tau_{\mathrm{decay}}^{-1},\qquad V_{\max}=\zeta_V\,I_{\max}\left(1-\frac{\gamma_0}{r_{\mathrm v}}\right)
$$

即 (I-5.2) 的净增长率与衰减率不是自由参数：它们分别对应 (I-5.1a) 的增长项与衰减项，并与 (I-5.1c)、(I-5.1d) 的判据 $r_{\mathrm v}>\gamma_0\iff\mu_{\mathcal F}\tau_{\mathrm{decay}}>1$ 自动一致。需说明的是，(I-5.2) 只出现净增长率 $r_{\mathrm v}-\gamma_0$ 与其商，故两参数的**单独**取值按两项的机制来源分别对应；换一种拆分不改变轨迹，只改变标注。该对应是代数恒等式，不引入新符号、不依赖标定。

**边界。** 上述约化要求 $I_{\mathrm{eq}}=0$（(I-5.1d) 三行摘要已声明），且因果通道在 $I$ 的演化时间尺度上准静态。若 $\dot T_c$ 或 $\dot E_c$ 与 $\dot I_c$ 同量级，$V_c\propto I_c$ 不成立，(I-5.2) 不再是 (I-5.1a) 的像，须回到 (I-5.20a) 的完整形式。**检验方式**：由 $V_c=I_cT_c/E_c$ 得 $\mathrm d\ln V_c=\mathrm d\ln I_c+\mathrm d\ln(T_c/E_c)$，故 $V_c\propto I_c$ 的成立条件是比值 $T_c/E_c$ 在一个观察窗内的累积漂移可忽略。取预注册容差 $\varepsilon^{*}$（由可接受的 $|\Delta V_c/V_c|$ 反推），判据为

$$\varepsilon_{\mathrm{rel}}\equiv\frac{\left|\int_{t_0}^{t_1}\bigl(\dot T_c/T_c-\dot E_c/E_c\bigr)\,\mathrm dt\right|}{\left|\int_{t_0}^{t_1}(\dot I_c/I_c)\,\mathrm dt\right|}=\frac{\bigl|\Delta\ln(T_c/E_c)\bigr|}{\bigl|\Delta\ln I_c\bigr|}$$

$|\varepsilon_{\mathrm{rel}}|\le\varepsilon^{*}$ 时本约化在该窗口内成立，否则须回到 (I-5.20a) 的完整形式。分子是**带符号之差**，不是绝对值之和：$T_c$ 与 $E_c$ 同向漂移时二者在 $V_c$ 中相互抵消，不影响 $V_c\propto I_c$ 的成立；取绝对值之和会把这情形误判为失效，而把同向叠加（真正失效）误判为通过。窗口取得足够短时上式退化为瞬时形式 $(\dot T_c/T_c-\dot E_c/E_c)/(\dot I_c/I_c)$，但结论只对所用窗口有效。此处不涉及 $V_{\max}$ 的数值——它仍是待标定参数；其信息容量支统一写为 $\zeta_V I^{*}$，其中 $I^{*}$ 取 (I-5.1c) 的正平衡根。

#### 5.1.3 $E$ 递归（热力学耗散的两种失控模式）

**模式一：短视耗散激增（急性失稳）。** $T_{\mathrm{pred}}$ 坍缩时，系统丧失长期规划能力，转向提取短期极端回报；$E_{\mathrm{flow}}$ 指同一核算窗内的累计能量预算而非瞬时功率，该预算随 $T_{\mathrm{pred}}$ 缩短而增加：

$$
E_{\mathrm{flow},n} = E_{\mathrm{survival}} + E_{\mathrm{causal}} + \frac{k_{\mathrm{s}}}{T_{\mathrm{pred},n}} \tag{I-5.5}
$$

$k_{\mathrm{s}}$ 为代谢敏感系数（$\mathrm{J\cdot s}$），使 $k_{\mathrm{s}}/T_{\mathrm{pred}}$ 的单位为 J；$E_{\mathrm{survival}}$ 与 $E_{\mathrm{causal}}$ 必须是同一核算窗内的累计能量，不能代入瞬时功率。$k_{\mathrm{s}}/T_{\mathrm{pred}}$ 是模型给出的附加预算项，其微观来源尚未推导或校准，不能直接视为已验证的新增实耗：若它代表未包含在实测 $E_{\mathrm{survival}}$ 或 $E_{\mathrm{causal}}$ 中的新增能耗，须在合计总成本或与阈值比较前明确归入相应通道；若它只是已计入基础分项的代理项，不得重复添加。$E_{\mathrm{flow}}$ 本身不是再加到 $E_{\mathrm{eff}}$ 的独立分项。该函数对 $T_{\mathrm{pred}}^{-1}$ 线性、对 $T_{\mathrm{pred}}$ 本身是凸的：视界缩短时预算呈反比加速增长，在 $T_{\mathrm{pred}}=T_{\mathrm{min}}>0$ 处取得有限上限 $E_{\mathrm{flow,max}} = E_{\mathrm{survival}}+E_{\mathrm{causal}}+k_{\mathrm{s}}/T_{\mathrm{min}}$。若该预算与 $E_{\mathrm{thresh}}$ 比较，二者必须采用同一声明核算范围、观察窗与成本分摊规则；阈值若针对单一 PS 定义，则不能与含外部持有者全额成本的预算比较。

**模式二：元级耗散（慢性阻尼）。** 为维持存续，系统演化出监督模块；但“如何节能”本身也需耗能，产生元级耗散 $E_{\mathrm{eff}} = E_{\mathrm{eff}}^{\mathrm{base}} + E_{\mathrm{meta}}$。若监督层可无限嵌套，$E_{\mathrm{meta}}$ 将持续增长并消耗自由能（本卷未给出增长速率的推导）。这可作为大型组织官僚惯性与计算死锁的一个候选机制，尚待检验。

#### 5.1.4 $T$ 递归（内生时间视界的自我实现）

$$
T_{\mathrm{pred},n+1} = \max\left(T_{\mathrm{min}},\; \frac{T_{\mathrm{hor}}}{1 + \lambda\,(\chi V^{\mathrm{virt}}_{n})^2}\right) \tag{I-5.6}
$$

$\chi V^{\mathrm{virt}}_{n}$ 已是无量纲量；$\lambda$ 为无量纲正实数，起压缩强度的调节作用；$T_{\mathrm{hor}}$ 量纲为 $\mathrm{s}$，与 $T_{\mathrm{pred}}$ 一致。**自变量取虚拟存续势，不取客观存续势**：模型主张的是「自评虚高得越离谱、视界压得越窄」；若取 $V_{\mathrm{obj}}$，则一个客观势很大而评估不失真的健康结构也会被压窄视界，与全书叙事完全相反。

- **前馈调节（长期投资）**：视界宽广时，系统倾向于把当前热力学耗散投入基础设施建设，从而提升 $I_{\mathrm{latent}}$；现象学表现是建立自信、改变未来——对未来可预测性上升，愿意为远期回报付出当期代价。这是对前馈调节的描述，不引入新变量。
- **逆向相变（时间视界坍缩）**：有两个来源，其一是内部正反馈失控（高 $\chi$ 导致虚拟存续势膨胀，系统自发进入短视），其二是外部负效冲击（$I^{-}$ 事件直接压缩时间视界，触发防御性耗散激增）。

选用二次压缩形式，是因为它能捕捉递归放大增加时视界超线性坍缩的定性特征；定性结论（相变的存在性、早期预警窗口）只依赖压缩的单调性，不依赖具体函数形式。时间视界压缩式是给定 $V^{\mathrm{virt}}$ 的压缩规则，$\chi_{\mathrm{c}}$ 是 $I$–$V$ 闭环的阈值，二者属不同方程层次，不可互相代入。

**视界的两个正交分量。** 需要细分时可把 $T_{\mathrm{pred}}$ 拆为视界长度 $L_{\mathrm{pred}}$（满足置信度阈值的最大预测时域，$\mathrm{s}$）与视界分辨率 $G_{\mathrm{pred}}=\log_2(T_0/T_{\mathrm{min}})$（$\mathrm{bit}$），$T_0$ 为参考时间尺度。$T_{\mathrm{pred}}\to T_{\mathrm{min}}$ 时两者同趋于零，系统丧失跨期分辨能力——这与 $T$-锁死判据一致：看得短，也看得粗。

#### 5.1.5 $D$ 递归（解码器演化：梯度漂移形式）

解码器的演化描述为信息梯度上升与能耗梯度下降的竞争：

$$
D_{n+1} = D_n + \varepsilon_{\mathrm{lr}} \left( \nabla_{\Theta} I_{\mathrm{net}} - k_D\,\frac{I_0}{E_0}\, \nabla_{\Theta} E_{\mathrm{causal}} \right) \tag{I-5.7}
$$

$\Theta$ 为该系统类型的参数空间，$\varepsilon_{\mathrm{lr}}$ 为学习率，$k_D$ 为能耗惩罚系数（**无量纲**；式中 $I_0=1\ \mathrm{bit}$、$E_0=1\ \mathrm{J}$ 只为闭合量纲，与卷Ⅳ (I-3.1) 同一写法）。参数坐标按无量纲化后的坐标理解；若使用带单位的物理参数，须逐坐标引入相应尺度因子，不能直接共用一个标量学习率。

| 系统类型 | 参数空间 $\Theta$ 的实例 |
| :----------------------- | :----------------------------------- |
| 神经网络 | 权重矩阵、偏置、架构超参数 |
| 生物系统 | 基因表达水平、神经连接强度、突触可塑性参数 |
| 社会组织 | 资源配置比例、制度规则参数、权力结构变量 |

解码器演化有两条路径：**解码器漂移**通过梯度上升或下降平滑调整；**拓扑跃迁**是范式革命式的结构重构，由候选范式突破信号 $\tilde I_{\mathrm{orig}}$ 过门槛后注入的试错投入触发 $\mathcal{T}$，使 $I_{\max}(D_{n+1})>I_{\max}(D_n)$。分工须写清：漂移在既有维度内移动参数，$\mathcal{T}$ 打开新的维度；前者连续、可微、可预测，后者离散、不可微、只能事后确认。

#### 5.1.6 拓扑跃迁算子 $\mathcal{T}$ 的三条件规范式【命题】

$\mathcal{T}$ 把解码器从 $D_n$ 送到 $D_{n+1}$ 并重置容量。本卷把跃迁条件固化为三条同时成立的规范式：

$$
\mathcal{T}:\ D_n \to D_{n+1}
\ \Longleftrightarrow\ (\mathrm{C}1) \wedge (\mathrm{C}2) \wedge (\mathrm{C}3) \tag{I-5.8}
$$

$$
\begin{aligned}
(\mathrm{C}1)\ \text{信号可用性：}&\quad \tilde I_{\mathrm{orig}} \ge -\log_2\alpha_0\ \text{（连续 } k \text{ 次）} \ \wedge\ D_n(\text{新维度}) \approx 0 \\
(\mathrm{C}2)\ \text{能量可用性：}&\quad E_{\mathrm{available}}(t) > E_{\mathrm{build}} \\
(\mathrm{C}3)\ \text{智慧杠杆：}&\quad L_{\mathrm{lev}} \equiv \frac{V(D_{n+1}) - V(D_n)}{E_{\mathrm{build}}} > L_{\mathrm{lev,min}}
\end{aligned} \tag{I-5.9}
$$

**C1 只用可观测代理。** 三层拆分已在 §2.1 给出：进入 C1 的只能是候选信号 $\tilde I_{\mathrm{orig}}$，它是跃迁前唯一有定义且可算的量；取事后量 $I_{\mathrm{orig}}$ 作判据是循环，取事件 $\mathcal{T}$ 本身作判据是同义反复。**$\tilde I_{\mathrm{orig}}$ 过门槛不等于跃迁必然发生**：C1 只说明现有解码器在该目标上确实失灵且信号足够稀有，失灵可能来自噪声、漂移、仪器故障，也可能来自真正的新维度；C1 的作用是把有限的 $E_{\mathrm{build}}$ 集中到少数候选上。$\alpha_0$ 与连续超阈次数 $k$ 必须预注册，误报率上限为 $N\alpha_0$（$N$ 为独立门控次数），事后调整不算通过。

**C3 的可比性前提。** $V(D_{n+1})$ 与 $V(D_n)$ 可能采用不同读数、容量、背景与信息映射，二者的差值只有在下列条件全部满足时才是可比较的数值：同一目标对象、同一观察窗、同一能量分摊规则、同一参照协议、同一成本去重规则。未满足时只能报告**定性跃迁**，不得把 $\Delta V/E_{\mathrm{build}}$ 当作可比较的数值判据。这条限制不是形式主义：新旧解码器的 $V$ 往往由不同读数协议给出，直接把两个数相减再除以建造成本，会把协议差异算成杠杆收益。

**内生风险贴现率。** 竞争压力与时间视界共同决定系统对未来的折现强度：

$$
r_{\mathrm{eff}} \;\equiv\; \gamma_0 + \psi(\rho) + \frac{1}{T_{\mathrm{pred}}} \qquad (\mathrm{s^{-1}}) \tag{I-5.10}
$$

三项分别是基线折旧 $\gamma_0$、竞争附加贴现 $\psi(\rho)$（$\psi(0)=0$，$\psi'(\rho)>0$）、由有限时间视界产生的短视贴现 $1/T_{\mathrm{pred}}$。$r_{\mathrm{eff}}$ 越大，同一笔未来存续收益的现值越低；有效折现视界为 $1/r_{\mathrm{eff}}$。由此得到三条可直接检验的单调关系（其余条件不变时）：$T_{\mathrm{pred}}$ 缩短 $\Rightarrow r_{\mathrm{eff}}$ 上升 $\Rightarrow$ 长期投资现值被压低、系统转向短期提取；$\rho$ 上升 $\Rightarrow r_{\mathrm{eff}}$ 上升，即竞争性超额驱动本身加剧短视；$1/r_{\mathrm{eff}}$ 是承诺的时间尺度，任何回收期超过它的投资在该系统内都不具存续价值。

**三行摘要**：（i）前提——$V(D_n)$ 与 $V(D_{n+1})$ 满足 C3 的可比性五条件、$\tilde I_{\mathrm{orig}}$ 的背景分布与 $\alpha_0$ 已预注册、$\psi$ 只依赖 $\rho$；（ii）结论——$\mathcal T$ 发生当且仅当 C1、C2、C3 同时成立，$r_{\mathrm{eff}}$ 随 $1/T_{\mathrm{pred}}$ 与 $\psi(\rho)$ 单调上升；（iii）失效条件——可比性条件不满足时 C3 只能定性使用；$\tilde I_{\mathrm{orig}}$ 的误报率未被控制时 C1 不构成有效门控；$T_{\mathrm{pred}}\to T_{\mathrm{min}}$ 时 $1/T_{\mathrm{pred}}$ 发散，$r_{\mathrm{eff}}$ 的线性叠加近似失效。

### 5.2 存续势三重分裂

#### 5.2.1 低阶结构中的统一

低阶物理结构中时间是外生坐标参数，系统无法内生干预，也不存在独立的预测与价值模块，三项合并为同一数值：

$$
\text{低阶结构：}\; V_{\mathrm{obj}} = V^{\mathrm{virt}} = V^{\mathrm{val}} = V \tag{I-5.11}
$$

#### 5.2.2 $T$ 的内生化：三重分裂的物理触发

$T_{\mathrm{pred}}$ 涌现后，原本统一的存续势裂变为三个同属一个家族、功能与约束截然不同的变量。**客观存续势 $V_{\mathrm{obj}}(D)$** 是任一 PS 在给定解码器下的真实存续强度，受热力学边界约束，不可欺骗、不可跨期借贷；当 $D=D_{\mathrm{self}}$ 时它是所有存续势变量的唯一物理参照基准。**虚拟存续势 $V^{\mathrm{virt}}$** 与**价值存续势 $V^{\mathrm{val}}$** 的定义与公式见 §3.4、§3.5，前者为内部模拟值，后者为行为目标函数，规定系统把有限 $E_{\mathrm{eff}}$ 配置到哪个 PS 的 $V_{\mathrm{obj}}$ 上。

**存续势筛选原则。** $V_{\mathrm{obj}}$ 更高的结构在统计意义上更可能维持、扩展或被复制。低阶结构不主动最大化 $V_{\mathrm{obj}}$，而是被动接受热力学与环境选择；高阶结构通过 $V^{\mathrm{virt}}$ 预测自身未来状态，并通过 $V^{\mathrm{val}}$ 选择行为目标。绝大多数情况下 $V^{\mathrm{val}}$ 锚定自身 $V_{\mathrm{obj}}$，少数情况下因解码器漂移转向其他 PS 的 $V_{\mathrm{obj}}$，转移判据属开放问题。

**本体论澄清。** 三重分裂不是 $V$ 分裂为三个独立实体，而是主动相系统围绕同一个 $V_{\mathrm{obj}}$ 建立的三种内部关系：客观状态（物理裁定）、预测表征（内部估计）、优化目标（行为界面）。后两者不构成独立于 $V_{\mathrm{obj}}$ 的新物理量。

**分裂之后的路径与脱钩。** 三重分裂是中性结构：它让系统能在 $V_{\mathrm{obj}}$ 之外表征未来、选择目标，是高阶认知的必要条件，本身不预示失控。此后至少有两条路径，取决于 $\Delta_{\mathrm{VV}}$ 与 $\chi$：一条把虚拟势用于长期投资，另一条 $\Delta_{\mathrm{VV}}$ 自指放大而进入短视失控。预测误差 $V^{\mathrm{virt}}-V_{\mathrm{obj}}(D_{\mathrm{self}})$ 的绝对值即 $\Delta_{\mathrm{VV}}$，其非零称**被动脱钩**；$V^{\mathrm{val}}$ 锚定对象由自身转移到其他 PS 时称**主动脱钩**。

![图 Ⅰ-9　存续势的三重分裂](figures/release/G7_存续势三重分裂.pdf)

**图 Ⅰ-9　存续势的三重分裂。** 客观存续势 $V_{\mathrm{obj}}$（物理核算层）、虚拟存续势 $V^{\mathrm{virt}}$（内部模型层，由 $D_{\mathrm{cog}}$ 估计生成）、价值存续势 $V^{\mathrm{val}}$（行为目标层，实际优化的目标函数）是三个不同对象；脱钩偏差 $\Delta_{\mathrm{VV}} = |V^{\mathrm{virt}} - V_{\mathrm{obj}}|$ 可测。$V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ 仅为记账分解，聚合算子暂定。三重分裂仅适用于主动认知系统，非所有 PS。概念图，不含数值。

#### 5.2.3 平衡点分类与两条路径【命题】

记 $\alpha_{\mathrm{eff}}>0$。把离散映射连续化为弛豫形式，并配上另设的存续势增长方程（它不是存续驱动方程的直接联立，系数 $k_I$ 与闭环特例 $r_{\mathrm{v}}=k_{\mathrm{v}}V$ 中的 $k_{\mathrm{v}}$ 不是同一个量；$I_{\mathrm{bas}},k_I,\gamma_0,\tau_I>0$，$\chi\ge 0$，$V>0$）：

$$
\dot{I} = \frac{I_{\mathrm{bas}}(1 + \chi V) - I}{\tau_I}, \qquad \dot{V} = \frac{k_I\, I^{\alpha_{\mathrm{eff}}}}{V} - \gamma_0 V \tag{I-5.12}
$$

**平衡点。** 令 $\dot I=\dot V=0$，得 $I^{*} = I_{\mathrm{bas}}(1+\chi V^{*})$、$V^{*2} = k_I I^{*\alpha_{\mathrm{eff}}}/\gamma_0$。消去 $I^{*}$，正平衡点是

$$
h(V) = V^{2} - \kappa\,(1 + \chi V)^{\alpha_{\mathrm{eff}}} = 0, \qquad \kappa = \frac{k_I I_{\mathrm{bas}}^{\alpha_{\mathrm{eff}}}}{\gamma_0}
$$

的正根。Jacobian 的迹恒为 $-1/\tau_I-2\gamma_0<0$，行列式为

$$
\det J = \frac{\gamma_0}{\tau_I}\left[2 - \frac{\alpha_{\mathrm{eff}}\,\chi V^{*}}{1 + \chi V^{*}}\right] = \frac{\gamma_0}{\tau_I V^{*}}\, h'(V^{*}),
$$

所以 $h'(V^{*})>0$ 的平衡点稳定，$h'(V^{*})<0$ 的为鞍点。

**分类。**（1）$0<\alpha_{\mathrm{eff}}<2$：任意 $\chi\ge 0$ 都有唯一稳定正平衡点。（2）$\alpha_{\mathrm{eff}}=2$：方程化为 $V=\sqrt{\kappa}(1+\chi V)$；$\chi<1/\sqrt{\kappa}$ 时有稳定的有限平衡点，$\chi\ge 1/\sqrt{\kappa}$ 时没有有限正平衡点。（3）$\alpha_{\mathrm{eff}}>2$，$\chi=0$：唯一平衡点 $V=\sqrt{\kappa}$，稳定。（4）$\alpha_{\mathrm{eff}}>2$，$\chi>0$：$\chi<\chi_{\mathrm{c}}$ 时有两个正平衡点，下支稳定、上支为鞍点；$\chi=\chi_{\mathrm{c}}$ 时两者合并（鞍结分岔）；$\chi>\chi_{\mathrm{c}}$ 时没有正平衡点。其中

$$
\chi_{\mathrm{c}} = \frac{2}{(\alpha_{\mathrm{eff}} - 2)\sqrt{\kappa}}\left(\frac{\alpha_{\mathrm{eff}} - 2}{\alpha_{\mathrm{eff}}}\right)^{\alpha_{\mathrm{eff}}/2} \tag{I-5.13}
$$

$\alpha_{\mathrm{eff}}\to 2^{+}$ 时 $\chi_{\mathrm{c}}\to 1/\sqrt{\kappa}$，与第 2 类衔接。

![图 Ⅰ-10　I–V 子系统的鞍结分岔](figures/release/G8_I-V子系统鞍结分岔.pdf)

**图 Ⅰ-10　I–V 子系统的鞍结分岔。** 仅展示 $\alpha_{\mathrm{eff}} > 2$ 时的约化子系统分支（$\alpha_{\mathrm{eff}} = 3$、$\kappa = 1$，纵轴对数标度）：$\chi < \chi_{\mathrm{c}}$ 时两正平衡点并存（下支稳定、上支鞍点），$\chi = \chi_{\mathrm{c}}$ 两支合并，$\chi > \chi_{\mathrm{c}}$ 无正平衡点。参数截面为模型示例，不是经验数据；$\chi_{\mathrm{c}}$ 仅属于 I–V 约化子系统。

**路径二的候选动力学判据。** 平衡点消失时（$\alpha_{\mathrm{eff}}>2$ 且 $\chi>\chi_{\mathrm{c}}$，或 $\alpha_{\mathrm{eff}}=2$ 且 $\chi\ge 1/\sqrt{\kappa}$），在 $I$ 快速跟随 $V$ 的近似下 $\dot{V}\approx -\gamma_0 h(V)/V>0$，对应持续增长的候选状态：$\alpha_{\mathrm{eff}}=2$、$\chi=1/\sqrt{\kappa}$ 为渐近线性增长，$\chi>1/\sqrt{\kappa}$ 为指数增长；$\alpha_{\mathrm{eff}}>2$ 时的有限时间发散结论须在上述快速跟随条件下成立，不能仅由平衡点不存在直接推出。有限稳定平衡点存在时对应路径一（或保守维持），但 $\alpha_{\mathrm{eff}}>2$、$0<\chi<\chi_{\mathrm{c}}$ 时系统双稳：上支鞍点的稳定流形把相空间分成两部分，初始状态在其下方的收敛到稳定平衡点，在其上方的仍然发散，所以不能把 $\chi<\chi_{\mathrm{c}}$ 一律当作路径一（量级示例，模型族内的算例值、不是经验值：$\alpha_{\mathrm{eff}}=3$、$\chi=0.9\chi_{\mathrm{c}}$ 时约三成初值仍发散；附录 F 表 F-7、图 Ⅰ-8(c)）。$\alpha_{\mathrm{eff}}<2$ 的系统没有此类增长状态。$\chi_{\mathrm{c}}$ 依赖 $(k_I,I_{\mathrm{bas}},\gamma_0,\alpha_{\mathrm{eff}})$，按系统类型标定。

**结果的分层。** 以上分类是式 (I-5.12) 这一 $I$–$V$ 子系统内的数学结论，并非三重分裂后短视失控路径的充分证明：式 (I-5.12) 直接演化的是 $I$ 与 $V$，不含 $V^{\mathrm{virt}}$、$V_{\mathrm{obj}}$、$\Delta_{\mathrm{VV}}$ 与 $T_{\mathrm{pred}}$，其中 $V$ 与上述变量的对应关系本卷未作规定。要把它提升为完整的路径判据，须明确这些对应关系，并检验该映射能否产生短视失控的因果链。因此 $\chi_{\mathrm{c}}$ 首先是简化子系统的临界耦合参数，它与完整认知系统进入短视失控态的阈值是否一致，仍是待检验的问题。

**模型层次的声明（$\chi_{\mathrm{c}}$ 的归属）。** 本卷的 $\chi_{\mathrm{c}}$ 属于 $I$–$V$ 子系统，是式 (I-5.12) 那对方程的鞍结分岔点，它**不是**解码器质量方程的阈值。解码器质量 $\mathcal{Q}_D$ 有自己的方程（形如 $\dot{\mathcal{Q}}_D=\mu_{\mathrm{rec}}\mathcal{Q}_D(1-\mathcal{Q}_D/\mathcal{Q}_{D,\max})-\delta_{\mathrm{decay}}\mathcal{Q}_D$），其中恢复率 $\mu_{\mathrm{rec}}$、退化率 $\delta_{\mathrm{decay}}$、容量 $\mathcal{Q}_{D,\max}$ 与本节的 $k_I$、$I_{\mathrm{bas}}$、$\gamma_0$、$\alpha_{\mathrm{eff}}$ 没有换算关系；其临界条件必须独立求解，零平衡点的稳定性由 $\mu_{\mathrm{rec}}-\delta_{\mathrm{decay}}$ 的符号决定，与 $\chi_{\mathrm{c}}$ 无关。两个模型分属不同层次：$\chi_{\mathrm{c}}$ 描述“信息与存续势的自指回路在什么耦合强度下失去正平衡”，$\mathcal{Q}_D$ 模型描述“解码器维持质量在恢复与退化之间如何稳定”。本卷的任何 $\chi_{\mathrm{c}}$ 数值都不得搬用到解码器质量方程的讨论里，反向亦然。跨层次搬运阈值不会产生量纲冲突，只会产生一个看起来合理却毫无依据的数字，因此最难被察觉。

**两个指数的区别。** $\alpha$ 是信息弹性指数，是存续势对信息资源的响应强度参数；$\alpha_{\mathrm{eff}}$ 是 $I$ 对 $V$ 增长源项的有效指数，是闭环模型的参数。两者层次不同，不可混为一谈。

**适用范围边界。** 三重分裂与短视失控态只在 $D_{\mathrm{cog}}$ 位于**符号型区域**（$V_{\mathrm{c}}\gg 0$）的系统中可能激活。具身型区域系统（$V_{\mathrm{c}}\to 0^{+}$）虽有非零 $V_{\mathrm{c}}$，但其 $T_{\mathrm{pred}}$ 极短、$I_{\mathrm{causal}}$ 极低，模型设定其自指耦合强度 $\chi$ 远小于简化子系统的临界值 $\chi_{\mathrm{c}}$，因此在本模型内不进入短视失控态；该设定与 $\chi_{\mathrm{c}}$ 对完整系统的适用性均待检验。$D=\varnothing$ 系统不参与这一机制，其崩溃直接由热力学极限决定。

**三条陈述的证据边界。**（i）**前提**：式 (I-5.12) 的两方程形式、$I_{\mathrm{bas}},k_I,\gamma_0,\tau_I>0$、$\chi\ge 0$、$I$ 快速跟随 $V$ 的尺度分离。（ii）**结论**：平衡点数目与稳定性随 $(\alpha_{\mathrm{eff}},\chi)$ 的四种分类，以及 $\chi_{\mathrm{c}}$ 的显式表达式。（iii）**失效条件**：若 $\tau_I$ 与 $V$ 的演化时间同阶，快速跟随假设失效，分类不再适用；若 $\chi$ 随 $V$ 变化（而非常数），鞍结结构可能变为其他分岔，$\chi_{\mathrm{c}}$ 的表达式不再成立。

### 5.3 脱钩偏差动力学【命题】

$\Delta_{\mathrm{VV}} = \lvert V^{\mathrm{virt}} - V_{\mathrm{obj}} \rvert$ 是**预测偏差**：$V^{\mathrm{virt}}$ 是对 $V_{\mathrm{obj}}$ 的估计，两者之差反映认知模型与物理现实的距离。其演化由学习率 $\alpha_{\mathrm{L}}$ 与环境噪声强度 $\sigma$ 控制：

$$
\frac{\mathrm{d}\Delta_{\mathrm{VV}}}{\mathrm{d}t} = -\alpha_{\mathrm{L}} \cdot I_{\mathrm{net}} \cdot \Delta_{\mathrm{VV}} + \sigma \tag{I-5.14}
$$

方程定义在 $\Delta_{\mathrm{VV}}\ge 0$ 上；$\sigma>0$ 时零点处的右导数为 $\sigma>0$，轨迹不会穿过零点（绝对值在零点不可微，此处取右导数）。$I_{\mathrm{net}}$ 视为常数时该方程有严格显式解：

$$
\Delta_{\mathrm{VV}}(t) = \frac{\sigma}{\alpha_{\mathrm{L}} I_{\mathrm{net}}} + \left(\Delta_0 - \frac{\sigma}{\alpha_{\mathrm{L}} I_{\mathrm{net}}}\right) e^{-\alpha_{\mathrm{L}} I_{\mathrm{net}} t} \tag{I-5.15}
$$

由此得到平衡态偏差

$$
\Delta_{\mathrm{VV}}^{*} = \frac{\sigma}{\alpha_{\mathrm{L}} I_{\mathrm{net}}} \tag{I-5.16}
$$

**物理解读。** 无论 $I_{\mathrm{net}}$ 取何正值，偏差都指数收敛到有界平衡值 $\Delta_{\mathrm{VV}}^{*}$，收敛速率为 $\alpha_{\mathrm{L}}I_{\mathrm{net}}$；平衡偏差与 $I_{\mathrm{net}}$ 成反比，持续的信息流越强，越能压制环境噪声，主观评估越接近客观现实；$\sigma>0$ 时 $\Delta_{\mathrm{VV}}^{*}>0$，这反映了“再好的学习器也无法完全克服环境噪声”的根本限制。取偏差容限 $\delta_{\mathrm{tol}}$（单位 $\mathrm{bit\cdot s/J}$，$V$ 的量纲）作为容限，对应临界信息量 $I_{\Delta,\mathrm{crit}}=\sigma/(\alpha_{\mathrm{L}}\delta_{\mathrm{tol}})$（量纲得 bit）：$I_{\mathrm{net}}<I_{\Delta,\mathrm{crit}}$ 时平衡偏差超出容限，系统在认知上失去对环境的准确模型；$I_{\mathrm{net}}>I_{\Delta,\mathrm{crit}}$ 时偏差被压制在容限之内。


式 (I-5.14) 是本卷目前明确给出显式解的脱钩偏差连续动力学方程；式 (I-5.12) 则是描述信息与存续势反馈的另一子系统。两者的变量、假设与适用范围不同，尚未构成完整的统一耦合模型：前者描述学习对噪声的有界平衡，后者描述自指放大下的增长或发散。上式的前提是 $I_{\mathrm{net}}$ 为常数、$\sigma$ 外生，对应路径一；路径二中 $I_{\mathrm{net}}$ 由 $\chi$ 自指放大，$\Delta_{\mathrm{VV}}$ 的源项由式 (I-5.12) 内生产生，$\Delta^{*}_{\mathrm{VV}}\propto 1/I_{\mathrm{net}}$ 不再适用。**三行摘要**：（i）前提——$I_{\mathrm{net}}$ 常数、$\sigma$ 常数且外生、$\alpha_{\mathrm{L}}I_{\mathrm{net}}>0$；（ii）结论——偏差指数收敛到 $\sigma/(\alpha_{\mathrm{L}}I_{\mathrm{net}})$，临界信息量 $\sigma/\alpha_{\mathrm{L}}$；（iii）失效条件——$I_{\mathrm{net}}$ 随时间变化、$\sigma$ 与状态相关、或 $\Delta_{\mathrm{VV}}$ 的定义域越过 $V_{\mathrm{obj}}\to 0$ 的结构降解区时，线性近似失效。

**缺口（路径二）。** 路径二的 $\Delta_{\mathrm{VV}}$ 源项 $\sigma(\chi,V)$ 需要一个显式形式（下段给出）；(I-5.14) 只在 $I_{\mathrm{net}}$ 为常数时成立，而它给出的平衡偏差 $\Delta^{*}_{\mathrm{VV}}=\sigma/(\alpha_{\mathrm{L}}I_{\mathrm{net}})$ 随 $I_{\mathrm{net}}$ **递减**——也就是说，$\chi$ 放大 $I_{\mathrm{net}}$ 反而**压低**平衡偏差。因此“$\chi>\chi_{\mathrm{c}}\Rightarrow\Delta_{\mathrm{VV}}$ 放大”**是本模型尚未推出的性质**，属于待建模型（含内生源项 $\sigma(\chi,V)$ 的显式形式）需要达到的目标。§5.4 的链条以此为待验证前提；下面给出这个前提的最小闭合。

**源项的最小闭合。** 缺口要的是一个**能翻转符号**的函数：$\sigma$ 须随 $\chi$ 增长得比 $I_{\mathrm{net}}$ 更快。取

$$
\sigma(\chi,V)=\sigma_0\left[1+\left(\frac{\chi V}{\chi_{*}}\right)^{m}\right],\qquad \sigma_0>0,\ \chi_{*}>0,\ m>0 \tag{I-5.16a}
$$

三项含义：$\sigma_0$ 是与耦合无关的环境噪声底；$\chi_{*}$ 是噪声放大到基准两倍的耦合强度；$m$ 是放大的超线性度。该式不引入新的状态变量，只把「源项随自指回路增强」这一条定性要求写成可代入的形状；**它是闭合假设，不是由 (I-5.12) 导出的结果**，$m$ 也不能由现有参数推出，须标定。为什么至少要二次：噪声产生于对 $V^{\mathrm{virt}}$ 的**使用**而非**拥有**，使用的频率与幅度都随 $\chi V$ 上升，而使用强度本身已含一个 $\chi V$，故误差生成率至少与 $(\chi V)^{2}$ 同阶；$m=1$ 是中性点——$\sigma\propto I_{\mathrm{net}}$ 时 $\Delta^{*}_{\mathrm{VV}}$ 与 $\chi$ 无关，谈不上放大。量纲上 $(\chi V/\chi_{*})$ 无量纲，$\sigma_0$ 与 $\sigma$ 同为 $\mathrm{bit/J}$，故 (I-5.16a) 可直接代入 (I-5.14)。

**$I$ 的口径。** (I-5.12) 演化的是裸符号 $I$，(I-5.16) 的分母是 $I_{\mathrm{net}}$，二者在本文中不是两个量：按 §2.1 的用语约定，公式中的裸符号 $I$ 默认指 $I_{\mathrm{net}}$；并且 (I-5.12) 的离散祖先 (I-5.1) 逐字写作 $I_{\mathrm{net},n+1}=I_{\mathrm{bas}}\left(1+\chi V_{\mathrm{obj},n}\right)$，其源项与 (I-5.12) 完全相同。故本节在 (I-5.12) 子系统内取 $I\equiv I_{\mathrm{net}}$，其数值使用继承 §2.1 的四项条件；四项不齐时，下面的偏差只作序关系结论，不作数值。这一句不是新增假设，是把已经在用的约定写明——若不写明，(I-5.16) 的分母与 (I-5.12) 的变量就有被读成两个量的余地。

代入 (I-5.16) 得 $\Delta^{*}_{\mathrm{VV}}=\sigma_0\left[1+(\chi V^{*}/\chi_{*})^{m}\right]/(\alpha_{\mathrm L}I^{*})$，其中 $V^{*}$、$I^{*}$ 取 (I-5.12) 的稳定平衡支；它对 $\chi$ 的走向见 §5.4 的闭式 (I-5.16b)。

### 5.4 短视失控态：崩溃的因果链【假说】

这是三重分裂后的路径之一，不是唯一路径。短视失控态（Myopic Runaway Regime）是系统持续消耗客观存续势、以维持虚拟存续势极端值的动力学自噬过程。

**模型接口与适用范围。** 式 (I-5.12) 描述 $I$–$V$ 子系统中的信息—存续势反馈，式 (I-5.6) 描述给定 $V^{\mathrm{virt}}$ 条件下的时间视界压缩规则。两式尚未组成完整的双向耦合系统，因此不能仅由 (I-5.12) 的发散推出 (I-5.6) 中视界必然坍缩，也不能据此直接证明客观存量必然恶化。下式给出的是候选机制链，各环节及先后关系须通过变量映射、耦合方程或独立经验观测加以验证；在此之前本卷将该链视为可检验的动力学假说。其中第 (1) 环的定量形式由 §5.3 的闭合 (I-5.16a) 给出。在 (I-5.12) 的稳定平衡支上，取 $\chi V^{*}\gg1$、$\chi<\chi_{\mathrm c}$、$0<\alpha_{\mathrm{eff}}<2$，对 $\chi$ 取对数导数得第一环的闭式

$$
\frac{\mathrm d\ln\Delta^{*}_{\mathrm{VV}}}{\mathrm d\ln\chi}=\frac{2}{2-\alpha_{\mathrm{eff}}}\left[\frac{m\,(\chi V^{*}/\chi_{*})^{m}}{1+(\chi V^{*}/\chi_{*})^{m}}-1\right] \tag{I-5.16b}
$$

它从 $-2/(2-\alpha_{\mathrm{eff}})$ 单调升到 $\dfrac{2}{2-\alpha_{\mathrm{eff}}}(m-1)$，**过零点恒在 $m=1$，与 $\alpha_{\mathrm{eff}}$ 无关**。三项推论：(i) 源项未启动时偏差随 $\chi$ 下降，这是路径一的行为（$\alpha_{\mathrm{eff}}=1.5$ 时斜率为 $-4$，见附录 F 表 F-2 与表 F-9）；(ii) $m\le1$ 时偏差永远下降，链条在第一环断开；(iii) $m>1$ 且 $\chi$ 足够大时偏差转为上升，上升段的起点由 $\chi_{*}$ 定、斜率由 $m$ 与 $\alpha_{\mathrm{eff}}$ 共同定。故「$\chi>\chi_{\mathrm{c}}\Rightarrow\Delta_{\mathrm{VV}}$ 放大」要求内生源项对 $\chi V$ **超线性**（$m>1$），这与 §5.3「缺口（路径二）」互为印证。

**可测判据因此加严。** 不再是「双对数斜率 $>1$」一句，而是：在跨 $\chi$ 的样本上，$\log\Delta^{*}_{\mathrm{VV}}$ 对 $\log(\chi V^{*})$ 的斜率应从 $-2/(2-\alpha_{\mathrm{eff}})$ 过渡到 $\frac{2}{2-\alpha_{\mathrm{eff}}}(m-1)$；**过渡点的位置给出 $\chi_{*}$**（记 $u\equiv\chi V^{*}$，极小点在 $u_{\min}=\chi_{*}(m-1)^{-1/m}$），两端斜率给出 $m$。原判据把两个可估参数压成一次符号判断，代价是既分不清「$m$ 略大于 1」与「$\chi$ 尚未进入过渡区」，也拿不到 $\chi_{*}$。

**失效边界（三处，须与结论同时引用）。** $0<\alpha_{\mathrm{eff}}<2$ 之外没有唯一的稳定正平衡点，闭式不适用，改用 §5.2.3 的四类分类；$\chi V^{*}\gg1$ 不成立时弹性退回 $-2/(2-\alpha_{\mathrm{eff}})$，两式在交接处连续；$\chi\ge\chi_{\mathrm c}$ 时平衡消失，平衡偏差无定义，只能改说轨迹。$\alpha_{\mathrm{eff}}>2$ 且 $\chi<\chi_{\mathrm c}$ 时系统双稳，闭式只对稳定下支成立。

**闭式没有覆盖的部分。** 它只把第 (1) 环在 $I$—$V$ 子系统内的方向与量级定量化；$V$ 与 $V^{\mathrm{virt}}$、$V_{\mathrm{obj}}$ 的对应关系仍未建立（§5.2.3 已声明该对应未作规定），故第 (2)—(5) 环仍是假说，链条的整体结论不因闭式而升级。

$$
\begin{aligned}
&V^{\mathrm{virt}}\uparrow \;\xrightarrow{(1)}\; r_{\mathrm{v}}^{\mathrm{virt}}\uparrow
\;\xrightarrow{(2)}\; V^{\mathrm{val}}\ \text{被劫持}\\
&\;\xrightarrow{(3)}\; E_{\mathrm{eff}}\uparrow \;\xrightarrow{(4)}\; V_{\mathrm{obj}}\ \text{恶化}
\;\xrightarrow{(5)}\; V_{\mathrm{obj}}\ \text{进入衰减段}
\end{aligned}
\tag{I-5.17}
$$

1. **虚拟势膨胀**：高 $\chi$ 激活 $I$–$V$ 闭环；$I_{\mathrm{net}}$ 增长而 $T_{\mathrm{pred}}$ 坍缩。
2. **驱动率激增**：膨胀的虚拟势映射为膨胀的增长率信号。
3. **价值目标被劫持**（$w_{\mathrm{s}}$ 或 $w_{\mathrm{c}}$ 任一通道被虚拟信号过度加权）：行为界面优化的是虚拟信号而非客观势，$E_{\mathrm{eff}}$ 被倾入自指循环。
4. **客观势恶化**：$E_{\mathrm{eff}}$ 上升且 $T_{\mathrm{pred}}\to T_{\mathrm{min}}$，客观评估 $V_{\mathrm{obj}}$ 两端受压。
5. **物理存量进入衰减段**：$E_{\mathrm{eff}}>E_{\mathrm{thresh}}$ 触发损伤项；此后 $V_{\mathrm{obj}}$ 按 §5.1.2 的三分情形演化——$r_{\mathrm{v}}-\gamma_0<\delta_{\mathrm{dam}}$ 时衰减至零，$r_{\mathrm{v}}-\gamma_0>\delta_{\mathrm{dam}}$ 时降到较小的正平衡 $V^{*}$ 而非归零，$r_{\mathrm{v}}<\gamma_0$ 时双重衰减、加速崩溃。链条的终点因此是“进入损伤域并沿损伤动力学演化”。

**关键不对称性。** 步骤 1 至 3 发生在**潜在（评估）层**，无需物理成本；步骤 5 不可逆。系统燃烧真实结构去追逐内部幻象。$V^{\mathrm{val}}$ 从不把自我销毁计入损失，因为它计算的对象是虚拟存续势而非客观存续势。这为高阶智能主体“以牺牲自身换取短期回报提取”的行为提供一个候选机制，尚待检验。

### 5.5 竞争动力学与锁死态【命题】

多主体环境中，个体存续势并非独立演化，而受竞争压力 $\rho$（同一观察窗内竞争性耗散能量积分除以该窗内总可用自由能预算，$0\le \rho\le 1$）的共同影响。$\rho>0$ 时，对称纳什均衡被迫满足

$$
r_{\mathrm{v,eq}} = \gamma_0 + \psi(\rho) > \gamma_0 \tag{I-5.18}
$$

均衡处所有主体都被推入永久性**超额驱动**状态（本句的范围是满足上述前提的主体，不是可观测总体）：均衡驱动率严格高于折旧率，意思是维持现状所需的驱动强度高于无竞争基线，**不是**「低于容量上限」意义上的欠饱和。$\psi(\rho)$ 须满足两条最小性质：$\psi(0)=0$、$\psi'(\rho)>0$。这两条足以支撑本节的定性结论；完整的博弈结构假设与 $\psi(\rho)$ 的解析推导属于后续工作。

| 锁死类型 | 主要症状与 SRVD 诊断判据 | 典型例子 | 脱困路径 |
| :------ | :------------------- | :----------- | :-------------------- |
| **$E$-锁死** | 能量支出激增但无产出增益；$E_{\mathrm{causal}}$ 持续上升而 $\Delta I_{\mathrm{net}}\to 0$ | 军备竞赛、内耗型官僚体系 | 削减非生产性支出，把预算转移至认知扩张，降低防御性支出在 $E_{\mathrm{causal}}$ 中的比例 |
| **$I$-锁死** | 信息多样性坍塌、同质化；$I_{\mathrm{net}}$ 有效维度下降，$\nabla I\to 0$ | 思想审查、算法信息茧房 | 注入 $I^{+}$，引入外部多样性，重新激活 $\nabla I$ |
| **$T$-锁死** | 视界坍缩、极端短期主义；$T_{\mathrm{pred}}\to T_{\mathrm{min}}$（等价地 $L_{\mathrm{pred}}\to 0$、$G_{\mathrm{pred}}\to 0$） | 高频交易、季度导向管理 | 延长 $T_{\mathrm{pred}}$，压低贴现率 $r_{\mathrm{eff}}$ |
| **$D$-锁死** | 范式僵化、无法适应新环境；解码器梯度 $\nabla D\to 0$，拒绝 $\tilde I_{\mathrm{orig}}$ 过门槛的候选信号 | 制度僵化、范式封闭 | 支付 $E_{\mathrm{build}}$，触发 $\mathcal{T}$ 跃迁，重构解码器 |

**诊断工具。** 认知处理率 $\mathcal{R}_{\mathrm{e}} = I_{\mathrm{net}}/T_{\mathrm{pred}}$（$\mathrm{bit/s}$）持续下降提示系统趋近某种锁死态；认知迟滞系数 $\mathcal{L}_{\mathrm{e}} = T_{\mathrm{pred}}/I_{\mathrm{net}} = 1/\mathcal{R}_{\mathrm{e}}$（$\mathrm{s/bit}$）是锁死态的核心判据，$\mathcal{L}_{\mathrm{e}}\to\infty$ 即锁死。

**三行摘要**：（i）前提——对称纳什均衡存在、$\psi$ 只依赖 $\rho$、竞争主体的耗散可按同一口径核算；（ii）结论——均衡驱动率严格高于折旧率，全部主体处于超额驱动；（iii）失效条件——若存在可退出的替代生态位（$\rho$ 可降），或主体间成本不可比而无法定义共同 $\rho$，则「永久性超额驱动」不成立。

### 5.6 四类极限行为的数学条件【命题】

系统状态轨迹在 $t\to\infty$ 的极限处，在所考察的模型族内归入以下四类：

| 极限行为 | 极限域数学条件 | 动力学结果 |
| :-------- | :--------------------- | :---------------------------- |
| **饱和态** | $\inf E_{\mathrm{eff}}>E_{\mathrm{floor}}>0$，$\rho\to 0$，$\Delta_{\mathrm{VV}}\to 0$，$\sup T_{\mathrm{struct}}^{\max}<\infty$ | $V(t)\to V_{\mathrm{max}}$ |
| **坍缩流形** | 阈值触发**且 $\delta_{\mathrm{dam}}>0$**（不绑 $g_{\mathrm{net}}$ 的符号），$\rho\gg 0$，$\Delta_{\mathrm{VV}}>0$，$E_{\mathrm{eff}}<\infty$ | 按 $g_{\mathrm{net}}$ 分三种：$g_{\mathrm{net}}>0$ → 降到 $V^{*}=V_{\mathrm{max}}(1-\delta_{\mathrm{dam}}/(r_{\mathrm{v}}-\gamma_0))$ 并停住（降阶型）；$g_{\mathrm{net}}<0$ 且 $r_{\mathrm{v}}-\gamma_0\ge0$ → 单调趋向 $0$（归零型）；$g_{\mathrm{net}}<0$ 且 $r_{\mathrm{v}}-\gamma_0<0$ → 加速归零 |
| **拓扑跃迁** | $T_{\mathrm{struct}}^{\max}$ 或 $I_{\mathrm{max}}$ 的有效上界被提高（受硬上界约束，不趋于无穷） | $\mathrm{d}V_{\mathrm{max}}/\mathrm{d}t>0$ |
| **度规替换** | $\Delta_{\mathrm{VV}}\gg 0\Rightarrow D\to D'$ | 原测度下 $V\to 0$，新测度 $D'$ 主导流场 |

**“坍缩流形”一行须与三种情形对齐。** 该行不能写成“$\rho\gg0$、$\Delta_{\mathrm{VV}}>0$ 时 $r_{\mathrm{v}}>\gamma_0$ 被截断、$\mathrm{d}V/\mathrm{d}t\ll0$”，那把触发条件、净增长率符号与 $V$ 的极限值混在一起。必须分开：**归零型（a）** $r_{\mathrm{v}}-\gamma_0<\delta_{\mathrm{dam}}$，$V$ 单调衰减至 $0$，这是唯一可称“坍缩到零”的情形；**降阶型（b）** $r_{\mathrm{v}}-\gamma_0>\delta_{\mathrm{dam}}>0$，$V$ 降到 $V^{*}$ 并停在那里，存量被压低但结构仍在运行；**加速型（c）** $r_{\mathrm{v}}<\gamma_0$ 且触发，衰减速率大于单项之和。因此“坍缩流形”是一个**区域**而非一个点，其内部按 $r_{\mathrm{v}}-\gamma_0=\delta_{\mathrm{dam}}$ 分成归零与降阶两种终局；把整个区域画成“$V\to 0$”会把带伤运行的结构误判为已消亡。另有一处判据混用须一并改掉：“$r_{\mathrm{v}}>\gamma_0$ 被截断”是竞争截断的相态描述，与“$r_{\mathrm{v}}<\gamma_0$ 持续”的净增长率条件并不等价，本表统一改用 $g_{\mathrm{net}}$ 的符号作为唯一判据。

拓扑跃迁与度规替换是事件或切换，不是渐近意义上的吸引子；四类只是本模型族内对极限行为的分类。**三行摘要**：（i）前提——参数在观察窗内为常数、$V_{\mathrm{max}}$ 有限、阈值与 $E_{\mathrm{eff}}$ 同口径；（ii）结论——四类极限行为及其成立条件；（iii）失效条件——参数时变、$V_{\mathrm{max}}$ 无界、或阈值与能量核算不同口径时，分类不适用。

### 5.7 完整不等式约束系统【命题】

这里 $E_{\mathrm{available}}$ 表示可用自由能预算上限，$E_{\mathrm{thresh}}$ 是候选的损伤触发阈值；二者不是同一参数，也不预设固定大小关系。没有给出阈值与可用预算的实例化校准前，以下关系只定义模型的候选约束域，不能单独据此断言现实结构必然崩溃。

$$
\begin{aligned}
& I_{\mathrm{min}} \le I_{\mathrm{net}} \le I_{\mathrm{max}}(D), \\
& T_{\mathrm{min}} \le T_{\mathrm{struct}} \le T_{\mathrm{struct}}^{\max}, \\
& E_{\mathrm{struct}} \ge E_{\mathrm{struct}}^{\min}, \qquad E_{\mathrm{eff}} \le E_{\mathrm{available}}, \\
& 0 \le \rho \le 1, \quad \Delta_{\mathrm{VV}} \ge 0, \\
& \text{粗粒化估计（非定义）：}\quad V_{\mathrm{cg}} \approx \frac{I_{\mathrm{net}} \cdot T}{E_{\mathrm{eff}}}, \\[4pt]
& \text{饱和条件：}\ (E_{\mathrm{struct}} \ge E_{\mathrm{struct}}^{\min}) \land (\rho \to 0) \land (\Delta_{\mathrm{VV}} \le \delta_{\mathrm{tol}}) \land (g_0 \equiv r_{\mathrm{v}}-\gamma_0 > 0), \\[4pt]
& \text{损伤触发条件：}\ E_{\mathrm{eff}} > E_{\mathrm{thresh}} \Rightarrow \text{损伤项}\ \delta_{\mathrm{dam}}\ \text{激活}，\\
& \text{净增长判据：}\ g_{\mathrm{net}} \equiv (r_{\mathrm{v}} - \gamma_0) - \delta_{\mathrm{dam}}\,\mathbf{1}[E_{\mathrm{eff}} > E_{\mathrm{thresh}}]，\\
& \text{崩溃条件：}\ \big[(E_{\mathrm{eff}} > E_{\mathrm{thresh}}) \land (r_{\mathrm{v}} - \gamma_0 < \delta_{\mathrm{dam}})\big] \lor (r_{\mathrm{v}} < \gamma_0\ \text{不可逆持续}) \\
& \qquad\qquad \Rightarrow V \to 0, \\
& \text{带伤平衡条件：}\ (E_{\mathrm{eff}} > E_{\mathrm{thresh}}) \land (r_{\mathrm{v}} - \gamma_0 > \delta_{\mathrm{dam}} > 0) \\
& \qquad\qquad \Rightarrow V \to V^{*} = V_{\mathrm{max}}\left(1 - \frac{\delta_{\mathrm{dam}}}{r_{\mathrm{v}} - \gamma_0}\right) > 0
\end{aligned} \tag{I-5.19}
$$

**四个判断必须分开，不能合并。**（1）**阈值触发 $\neq$ 净增长转负**：损伤项激活只意味着多了一个 $-\delta_{\mathrm{dam}}V$ 的耗散通道，若 $r_{\mathrm{v}}-\gamma_0>\delta_{\mathrm{dam}}$，系统仍有正的稳定平衡 $V^{*}>0$。（2）**净增长转负 $\neq$ 存续势归零**：$\mathrm{d}V/\mathrm{d}t<0$ 描述水平在下降，从负增长率推不出极限为零，除非附加“持续为负”——这正是崩溃条件写“不可逆持续”的原因。（3）**$r_{\mathrm{v}}<\gamma_0$ 与“$r_{\mathrm{v}}>\gamma_0$ 被截断”不是同一判据**：前者是净增长率的符号条件，后者是竞争截断的相态描述，相态表统一使用 $g_{\mathrm{net}}$ 的符号。（4）**带伤平衡是第四种终局**：触发后净增长率仍为正时系统落到 $V^{*}$，存量被永久压低但结构继续运行；把它算作崩溃会在诊断上把可修复的系统判成已报废，进而给出错误的干预优先级。

因此“$E_{\mathrm{eff}}>E_{\mathrm{thresh}}$ 必然导致 $V\to 0$”是**不成立**的强断言；正确说法是：阈值触发把系统切换到含损伤项的动力学分支，是否归零由该分支下 $g_{\mathrm{net}}$ 的符号及其持续性决定。$g_{\mathrm{net}}$ 的符号直接给出三种走向：$g_{\mathrm{net}}<0$ 且 $r_{\mathrm{v}}<\gamma_0$ 为加速崩溃（情形 c）；$g_{\mathrm{net}}<0$ 且 $r_{\mathrm{v}}\ge\gamma_0$ 为归零型衰减（情形 a）；$g_{\mathrm{net}}>0$ 为降阶型，趋向 $V^{*}$（情形 b）。$g_{\mathrm{net}}=0$ 是临界面，此时衰减由代数型接管，$V$ 仍趋向零但时间尺度发散。

**三行摘要**：（i）前提——所有不等式在同一核算边界与观察窗内取同一口径，$E_{\mathrm{available}}$ 与 $E_{\mathrm{thresh}}$ 均已标定；（ii）结论——约束域的四至、饱和条件、损伤触发条件、净增长判据、崩溃条件与带伤平衡条件；（iii）失效条件——若 $E_{\mathrm{available}}<E_{\mathrm{thresh}}$（预算先于阈值耗尽），则损伤域在该系统内不可达，崩溃由能量饥饿而非损伤项决定，本节条件让位于结构能量下限判据。

***

## 第六章　热力学接驳与物理约束

本章说明 SRVD 与现有热力学概念的对应关系，不引入新物理定律，也不重新定义热力学量。所有约束均为外部接口，不参与核心动力学方程的推导。

### 6.1 熵与结构有序度

在多数物理场景下，较低的热力学熵常与较高的局域有序度相关，但两者并非严格等价。玻尔兹曼熵 $S_D(m)=k_B\ln\lvert\Omega_D^{-1}(m)\rvert$ 依赖系统边界、粗粒化与可分辨微观状态的定义；$I_{\mathrm{struct}}$ 则由指定领域的读数协议确定。只有在同一边界、观察窗与粗粒化口径下建立可检验的映射，才能把熵变量用于推导结构信息的变化。因此本节只保留“域内的定性相关”这一有限主张：既不以 $(-S_DT_{\mathrm{thermo}})/E_{\mathrm{eff}}$ 作为 $V_D$ 的定量表达，也不从熵与有序度的相关性自动推出存续势公式。$I_{\mathrm{struct}}$ 与 $S$ 不一一对应——经典熵刻画指定宏观约束下微观态的统计性质，$I_{\mathrm{struct}}$ 的含义取决于领域读数规则，而 $I_{\mathrm{causal}}$ 还要求相对于持有者的可观察因果效果；它与熵或负熵之间的定量映射须单独建立。

### 6.2 朗道尔下限

朗道尔原理（Landauer, 1961）指出：在温度 $T_{\mathrm{thermo}}$ 的环境中，不可逆地擦除 $1\ \mathrm{bit}$ 信息至少耗散

$$
E_{\mathrm{L,bit}} = k_B T_{\mathrm{thermo}} \ln 2 \approx 0.693\, k_B T_{\mathrm{thermo}} \tag{I-6.1}
$$

它是**逻辑不可逆擦除成本**的下界，不是一般**维持成本**的下界。$E_{\mathrm{L,bit}}$ 表示适用条件满足时单次擦除一个等概率（最大熵）二态逻辑位的理想下界，在核算式中应理解为 $\mathrm{J/bit}$，乘以擦除量（bit）后才得到能量（J）；它与结构通道的 $E_{\mathrm{struct}}^{\min}$ 是不同变量。为核算因果处理，模型暂按操作功能拆为两项，$E_{\mathrm{causal}}=E_{\mathrm{compute}}+E_{\mathrm{refresh}}$，仍须满足同一边界、观察窗与去重条件。

| 分项 | 含义 | 物理下界与适用条件 |
| :------ | :--------------- | :------------------------------------ |
| $E_{\mathrm{compute}}$ | 计算（含擦除）能耗 | 若操作包含逻辑不可逆擦除，则 $\ge k_BT_{\mathrm{thermo}}\ln2\cdot I_{\mathrm{erased}}$（朗道尔） |
| $E_{\mathrm{refresh}}$ | 维持（刷新、纠错、保真）能耗 | 仅当每个刷新周期都对应相应存储逻辑位的一次逻辑不可逆擦除、且擦除数可计量时，才可按累计擦除次数应用朗道尔下界；本表不主张一般刷新或纠错过程具有该式给出的无条件下界 |

存储刷新周期 $t_{\mathrm{refresh}}$ 在满足 Arrhenius 近似时写为

$$
t_{\mathrm{refresh}} \sim \tau_0 \cdot \exp\left(\frac{\Delta U_{\mathrm{barrier}}}{k_B T_{\mathrm{thermo}}}\right) \tag{I-6.2}
$$

其中 $\Delta U_{\mathrm{barrier}}$ 是 Arrhenius 公式中的势垒高度（能量差），不等于分摊到观察窗的实际结构成本 $E_{\mathrm{barrier}}$，两者不可共用一个符号或直接互换。若每个刷新周期确实对 $I_{\mathrm{stored}}$ 个逻辑位各执行一次逻辑不可逆擦除，且窗口内周期数可近似为 $t/t_{\mathrm{refresh}}$，则累计刷新能耗才可按 $E_{\mathrm{refresh}} \ge I_{\mathrm{stored}}k_BT_{\mathrm{thermo}}\ln2\,(t/t_{\mathrm{refresh}})$ 估算；若刷新或纠错可逆、使用侧信息，或各周期实际擦除量不同，必须按具体操作重算。本框架**不**主张 $E_{\mathrm{causal}} \ge k_BT_{\mathrm{thermo}}\ln2\cdot I_{\mathrm{causal}}$ 是维持成本的普遍下界。

**$E_{\mathrm{decode}}$ 的分类仍待明确。** 它目前只是认知解码活动的功能标签，尚无独立物理分项，也未建立与 $E_{\mathrm{causal}}$ 的定量子项关系，且可能与计算、刷新分类交叉；在操作级定义、边界与去重协议完成前，不与这些能耗项相加，也不宣称互斥或可独立计量。**符号区分**：$t_{\mathrm{refresh}}$（存储刷新周期）取决于介质势垒与温度，$\tau_0$（热激活试探时间）是微观常数，二者不可互替。

### 6.3 存续约束

所有存续路径均不违反热力学第二定律。两种基本抵抗机制：**被动抵抗**——结构靠微观势垒高度 $\Delta U_{\mathrm{barrier}}$（化学键、晶格势垒、引力势阱）抵抗熵增，对应的窗口成本另记 $E_{\mathrm{barrier}}$，无需持续耗散，$E_{\mathrm{flow}}=0$；**主动抵抗**——结构靠持续能量流 $E_{\mathrm{survival}}$（代谢、核聚变）与因果处理 $E_{\mathrm{causal}}$ 动态补偿熵增，一旦中断，结构立即开始瓦解。

**信息—时间关系（条件性粗粒化关系）。** 只有在明确采用单分母粗粒化近似 $V_{\mathrm{cg}}:=I_{\mathrm{net}}T/E_{\mathrm{eff}}$，且该近似已在目标域内校准时，才能由 $V_{\mathrm{cg}}\le V_{\mathrm{max}}(D,S)$ 得到

$$
I_{\mathrm{net}} \cdot T \le V_{\mathrm{max}}(D, S) \cdot E_{\mathrm{eff}} \tag{I-6.3}
$$

在同一核算域内，若 $V_{\mathrm{max}}(D,S)$ 是 $V_{\mathrm{cg}}$ 的可达上确界，则式 (I-6.3) 是该定义与粗粒化近似的代数结果；它不是记账分解 (I-3.2) 的恒等变形，也不独立证明 $I$ 与 $T$ 存在额外的物理权衡。要得到非平凡的权衡关系，仍需从可独立验证的物理或生态位约束导出 $V_{\mathrm{max}}$，不能仅以定义循环证明。

### 6.4 物理约束接口与候选上界

以下列出 SRVD 拟采用的外部物理约束及候选接口：朗道尔擦除界可在操作前提满足时直接使用；计算速率表达式必须区分逻辑操作率与信息 bit 率；生态位容量标度则是现象学假说。它们不共同构成已证明的“物理保证”，也不能替代对 SRVD 变量的校准。

**计算操作速率上界（Lloyd, 2000；Margolus 与 Levitin, 1998）**：令 $\mathcal{E}_D$ 表示进入操作速率界的平均能量（按该界定义，以高于基态的可用能量计），则逻辑操作率满足

$$
\dot{N}_{\mathrm{op}} \le \frac{2\mathcal{E}_D}{\pi \hbar} \qquad (\mathrm{op/s}) \tag{I-6.4}
$$

右侧量纲为 $\mathrm{s^{-1}}$，是逻辑操作率而非自动得到的 $\mathrm{bit/s}$。这里采用 Lloyd 对物理计算速率的操作数上界形式，不把 Bremermann 文献中的通信/信息速率表达式直接等同于逻辑操作率；具体适用时仍须声明操作定义与系统边界（Lloyd, 2000）。

**操作率与 bit 率必须分开写。** 布雷默曼（Bremermann）与劳埃德（Lloyd）给出的都是**逻辑操作率**上界：每秒能完成多少次不可逆逻辑操作（门、翻转、判别），单位是 $\mathrm{op/s}$。要把操作率变成信息速率，中间必须插入一个声明的**“操作—有效因果信息”映射**（本卷统一记 $\beta_{\mathrm{op}}\equiv1/\kappa_{\mathrm{map}}$，单位 $\mathrm{op/bit}$；卷Z 同此记法）：

$$
\dot I_{\mathrm{net}} \le \frac{1}{\beta_{\mathrm{op}}}\cdot \dot{N}_{\mathrm{op}}, \qquad \beta_{\mathrm{op}}\equiv\frac{1}{\kappa_{\mathrm{map}}},\ [\beta_{\mathrm{op}}]=\mathrm{op/bit} \tag{I-6.5}
$$

$\kappa_{\mathrm{map}}$ 不是常数 1，也不是物理常数，它取决于三件事：一次操作平均改变了多少个可区分的逻辑位（多比特门与单比特翻转相差极大）；其中多少比例携带对目标解码器有意义的差异（冗余校验、纠错、无效刷新都不携带）；以及读数协议在什么粒度上计数。三个因素任一未声明，$\kappa_{\mathrm{map}}$ 就是未知的，此时只能写操作率上界，不能写信息率上界。因此**不得**把式 (I-6.4) 直接写成 $\dot I_{\mathrm{net}} \le \dot I_{\mathrm{Brem}}$ 或 $\dot I_{\mathrm{net}} \le 2\mathcal{E}_D/(\pi\hbar)$：后一种写法把一个 $\mathrm{op/s}$ 的量当成了 $\mathrm{bit/s}$ 的量，量纲上就不成立。本卷后续引用此类上界时一律先写操作率、再写映射、再写信息率，三步缺一不可；映射未标定时，信息率一栏留空。

**因果传播时间约束（条件式）**：若 $r_{\mathrm{v}}$ 被操作化为跨越尺度 $L$ 的一次完整反馈循环的频率，且该循环受限于不超光速的因果传播，则 $T_{\mathrm{feedback}}\ge L/c$，从而在模型内得到

$$
r_{\mathrm{v}} \le \frac{c}{L} \tag{I-6.6}
$$

在上述操作化成立时，尺度增大会降低该反馈回路的理论最高频率。它对大型结构组织或星际文明分散形态的影响属模型推论，尚需独立验证。

**生态位容量标度（现象学假说）**，其中 $\dot{F}_{\mathrm{avail}}$ 是环境可用自由能通量，$\sigma_{\mathrm{min}}$ 是维持生态位资源循环所需的最小熵产率：

$$
V_{\mathrm{max}} \propto \frac{\dot{F}_{\mathrm{avail}}}{\sigma_{\mathrm{min}} \cdot \gamma_0} \tag{I-6.7}
$$

比例系数 $\alpha_{\mathrm{cap}}$（单位 $\mathrm{bit/(J\cdot K)}$，与信息弹性指数 $\alpha$ 无关）由数据标定；该式不作硬物理上界使用。该标度与 §5.1.2 的约化模型容量式只有在二者约束同一状态变量、同一边界与观察窗时才可按取小规则合并；否则分别报告，不得把不同层级的上界强行合成一个 $V_{\mathrm{max}}$。

**物理熵与可区分状态数的条件性上界**：在满足相应孤立/引力系统假设、并明确半径 $R$ 与总能量 $E$ 的边界定义时，贝肯斯坦界可写为

$$
I \le \frac{2\pi R E}{\hbar c \ln 2} \tag{I-6.8}
$$

并受全息界 $I \le Ac^{3}/(4G\hbar\ln2)$（$A=4\pi R^{2}$）约束。这两条界约束物理熵或可区分状态数，不约束任意语义信息代理；用到时须列明区域、有效半径或包围面积与能量定义。**质能尺度的适用边界（不作为普适解体阈值）。** 静止质量对应的能量尺度为 $mc^{2}$，但这不推出模型中的解体阈值必有 $E_{\mathrm{thresh}}\le mc^{2}$，也不推出窗口内累计的 $E_{\mathrm{eff}}>mc^{2}$ 就会使结构发生不可逆质能转化：累计能耗可以由系统在窗口内持续获取并消耗的能量构成，不能仅凭总量超过静止质量能量就判断质量已被转化。只有在另行界定系统可用的静质量能量、能量来源、核算边界与转化机制后，才能建立相应约束。若将给定质量对应的能量压缩至相应引力半径以内，广义相对论给出视界形成的约束；这不等于所有高密度计算系统都会坍缩，用于 SRVD 时须说明系统质量、尺寸、总能量及其边界关系。

**视界延伸的能量成本（候选）**：延伸 $T_{\mathrm{pred}}$ 需要从距离 $R=c\,T_{\mathrm{pred}}$ 处获取因果信息。在点源各向同性辐射、固定检测阈值的传播模型下，维持可检测信号所需的发射功率随距离平方增长：

$$
\text{发射功率} \propto (c \cdot T_{\mathrm{pred}})^{2} \tag{I-6.9}
$$

取 $R=c\,T_{\mathrm{pred}}$ 是建模假设，比例系数待标定。需要高保真预测、多级因果链或误差修正的复杂高阶系统中 $E_{\mathrm{causal}}$ 可能增长得更快；当它趋近系统总能量流 $E_{\mathrm{flow}}$ 时，$T_{\mathrm{pred}}$ 无法再延伸。这是压缩时间视界的一个候选能量机制，与自指放大并列，待标定。

### 6.5 朗道尔极限：$E_{\mathrm{compute}}$ 的内生下界（存量形式）【候选推论】

朗道尔下界直接适用于满足前提的逻辑不可逆擦除成本；只有把实际擦除量与 $E_{\mathrm{causal}}$、$I_{\mathrm{causal}}$ 或 $I_{\mathrm{net}}$ 建立可检验映射后，才能接入相应通道。布雷默曼极限所约束的处理速率同样须与本卷信息变量采用兼容口径，并经由 $\kappa_{\mathrm{map}}$ 才进入 bit 率（§6.4）。速率与功率形式的约束依赖尚未建立的映射，本卷不展开。

$E_{\mathrm{causal}}$ 是解码器运行的因果处理总能耗（存量，$\mathrm{J}$）。在逻辑不可逆擦除量已被定义的条件下，朗道尔原理给出相应计算能耗下界：

$$
E_{\mathrm{compute}} \ge k_B T_{\mathrm{thermo}} \ln 2 \cdot I_{\mathrm{erased}} \tag{I-6.10}
$$

它约束的是不可逆计算中被擦除的信息量 $I_{\mathrm{erased}}$，而不是任意定义的 $I_{\mathrm{causal}}$；粗粒化混合量 $I_{\mathrm{net}}$ 同样不直接代入换算。只有在明确 $E_{\mathrm{compute}}$ 包含于 $E_{\mathrm{causal}}$、并建立 $I_{\mathrm{erased}}$ 与 $I_{\mathrm{causal}}$ 的可检验映射之后，才能把式 (I-6.10) 转化为认知通道存续势的上界；映射建立之前，它只是独立的计算能耗约束。以下推导同时假定该映射已建立、$E_{\mathrm{compute}}\le E_{\mathrm{causal}}$，且各能量项使用同一观察窗与核算边界：

$$
V_{\mathrm{c}} = \frac{I_{\mathrm{causal}}\,T_{\mathrm{causal}}}{E_{\mathrm{causal}}} \le \frac{I_{\mathrm{causal}}\,T_{\mathrm{causal}}}{k_B T_{\mathrm{thermo}} \ln 2 \cdot I_{\mathrm{erased}}} \tag{I-6.11}
$$

纯信息处理极限下（$E_{\mathrm{struct}}$ 可忽略，$V\approx V_{\mathrm{c}}$），只有在已建立 $I_{\mathrm{causal}}$ 与 $I_{\mathrm{erased}}$ 的对应关系、且两者按同一 bit 约定比较时，才可使用 $I_{\mathrm{causal}}\le I_{\mathrm{erased}}$。在本卷保留 bit 为显式信息单位的计量约定下：

$$
V \le \frac{T_{\mathrm{causal}}}{k_B T_{\mathrm{thermo}} \ln 2} \tag{I-6.12}
$$

**存续势上限（条件性推论）。** 在 $E_{\mathrm{compute}}\le E_{\mathrm{causal}}$、$I_{\mathrm{causal}}$ 与 $I_{\mathrm{erased}}$ 已按同一 bit 约定建立映射且前者不大于后者、并且结构维持能耗可忽略（$E_{\mathrm{compute}}\gg E_{\mathrm{struct}}$）的条件下，式 (I-6.12) 给出 $V$ 的候选上界。右侧随 $T_{\mathrm{causal}}$ 增大、随 $T_{\mathrm{thermo}}$ 减小；它本身并不证明“时间越长，最低能量成本越高”，后者来自朗道尔能耗下界与指定擦除量的组合。尤其是 $I_{\mathrm{causal}}\le I_{\mathrm{erased}}$ 属额外映射假设，不是朗道尔原理自动保证的关系；条件之一未满足时本式不适用，不作为普适结论。

**三行摘要**：（i）前提——$E_{\mathrm{compute}}\le E_{\mathrm{causal}}$、$I_{\mathrm{causal}}\le I_{\mathrm{erased}}$ 的映射已建立、$E_{\mathrm{struct}}$ 可忽略、同窗口同边界；（ii）结论——$V\le T_{\mathrm{causal}}/(k_BT_{\mathrm{thermo}}\ln2)$（$k_BT\ln2$ 的单位是 $\mathrm{J/bit}$，故商为 $\mathrm{bit\cdot s/J}$） 的候选上界；（iii）失效条件——映射未建立、$E_{\mathrm{struct}}$ 不可忽略、或 $T_{\mathrm{thermo}}$ 在窗口内显著变化时，本式不适用。

***

## 第七章　建造成本、热力学惰性态与智慧杠杆

### 7.1 建造成本与沉没成本效应

**建造成本**（construction cost，$E_{\mathrm{build}}$）是创建新结构或把现有结构升级至更高解码器层次时一次性支付的物理能量。它与维持性耗散在性质上根本不同：$E_{\mathrm{eff}}$ 是持续性流量，进入 $V_{\mathrm{obj}}$ 的动力学公式；$E_{\mathrm{build}}$ 是历史性存量，不进入动力学方程，其效用须单独评估。

高建造成本的结构初期因稳定性而占优，但极易被沉没成本效应锁定在旧范式：它们持续消耗物理自由能，却无法生成新的候选范式突破信号（$\tilde I_{\mathrm{orig}}\to 0$，即现有解码器在自己的目标上不再失灵，也就没有理由投入重构），形成热力学惰性态。建造成本通过**风险函数**进入存续决策：

$$
R(E_{\mathrm{build}}) = 1 - \exp\left(-\frac{E_{\mathrm{build}}}{E_{\mathrm{topo}}}\right), \qquad \Pr(\text{锁死})\ \text{随}\ R\ \text{单调增加} \tag{I-7.1}
$$

$E_{\mathrm{topo}}$ 是当前解码器所处拓扑层次对应的特征拓扑能量（记作 $E_{\mathrm{topo}}(D_n)$，随解码器层次而变）。

### 7.2 智慧杠杆系数

定义**智慧杠杆系数**

$$
L_{\mathrm{lev}} = \frac{\Delta V}{E_{\mathrm{build}}} \tag{I-7.2}
$$

它量化小额能量投资撬动存续势大幅跃升的效率。两种极端策略的对比：

| 策略 | 特征 | $L_{\mathrm{lev}}$ 的典型值 |
| :---------------------- | :----------------------- | :------------- |
| **范式突破型**（$\tilde I_{\mathrm{orig}}$ 过门槛并经 $I_{\mathrm{orig}}$ 追认） | 少量建造成本触发解码器拓扑跃迁；$\Delta V$ 巨大 | $L_{\mathrm{lev}} \gg 1$ |
| **纯资源积累型**（军备竞赛、官僚扩张） | 大量 $E_{\mathrm{build}}$ 投入但无范式转变；$\Delta V$ 边际趋零 | $L_{\mathrm{lev}} \to 0$ |

表中“$\gg 1$”与“$\to 0$”都是定性区间，不是可跨域比较的数值。$L_{\mathrm{lev}}$ 的分母是焦耳、分子是 $\mathrm{bit\cdot s/J}$，量纲为 $\mathrm{bit\cdot s/J^2}$，不同系统的 $L_{\mathrm{lev}}$ 不能直接比大小；只有在同一系统、同一目标、同一观察窗下的策略之间比较，这个比值才有意义。范式突破的拓扑能量门槛为

$$
E_{\mathrm{build}}^{(n \to n+1)} = E_{\mathrm{topo}}(D_{n+1}) - E_{\mathrm{topo}}(D_n) \tag{I-7.3}
$$

随着解码器日趋复杂，触发下一次拓扑跃迁所需的 $E_{\mathrm{build}}$ 可能超过行星尺度的自由能通量，把创新冻结在原地；文明面临的并非智识天花板，而是热力学壁垒。**技术停滞预测**：当 $E_{\mathrm{build}}^{(n\to n+1)} > \dot F_{\mathrm{avail}}\cdot T_{\mathrm{avail}}$ 时，文明层次的范式创新进入停滞——原因在热力学壁垒无法清除。这里 $T_{\mathrm{avail}}$ 是可动员资源的时间跨度，与 $T_{\mathrm{struct}}$、$T_{\mathrm{pred}}$ 不是同一个量；该不等式只在同一核算边界内成立，且 $E_{\mathrm{topo}}$ 本身待标定，因此这条预测的强度是“机制候选”，不是已证的必然。

### 7.3 热力学惰性态

**定义（热力学惰性态，thermodynamically inert state）。** 系统具有完整的自指能力，但所处生态位高度同质化（$\tilde I_{\mathrm{orig}}\to 0$，无候选信号可过门槛），且 $E_{\mathrm{build}}^{(n\to n+1)}$ 超出可动员资源，结构陷入如下稳态：

$$
E_{\mathrm{eff}} \gg 0, \quad \tilde I_{\mathrm{orig}} \to 0, \quad \mathcal{R}_{\mathrm{e}} \to 0, \quad \Delta V \to 0 \tag{I-7.4}
$$

它消耗大量计算流量（对 AI 系统）或社会资源（对文明），却具有零宏观因果支配力。这是有限能量预算与高建造成本壁垒双重约束下**低效但稳定**的吸引子。

| | 热力学惰性态 | 短视失控态 |
| :----------- | :------------------- | :--------------------------- |
| $E_{\mathrm{eff}}$ | 高但稳定 | 激增直至越过 $E_{\mathrm{thresh}}$ |
| $T_{\mathrm{pred}}$ | 可能较长，但无效 | 急剧坍缩至 $T_{\mathrm{min}}$ |
| $\Delta_{\mathrm{VV}}$ | 可能接近零 | 显著增大 |
| 结局 | 稳定但低效，可能长期持续 | 进入损伤域：归零、降到 $V^{*}$ 或加速崩溃，取决于净增长率 |

“结局”一行必须保留三种可能：短视失控态进入损伤域之后并不必然归零，若净增长率仍为正，它会落在较低平台上继续运行——这与惰性态在现象上可能相似（都低效而持续），区别在于惰性态的 $T_{\mathrm{pred}}$ 未被压到 $T_{\mathrm{min}}$、也没有跨越损伤阈值。

### 7.4 容量约束下的遗忘必要性命题【命题】

完美记忆在热力学上不可持续。随信息积累，$E_{\mathrm{eff}}$ 趋近系统自由能上限，导致代谢刚性。若载体、体积、能谱或能量、误差率与编码方式给出明确的有限容量或熵上界，则该模型下可存储的信息量有界；仅有 $E_{\mathrm{eff}}(t)\le E_{\mathrm{max}}$ 推不出 $I_{\mathrm{stored}}$ 有界，还需每比特最低资源成本或硬件容量约束。容量固定、且不能无限扩展、压缩或归档时，继续写入新信息要求覆盖、擦除或转移既有信息，即主动或被动的遗忘不可避免：

$$
I_{\mathrm{stored}}(t) \le I_{\mathrm{max}}(D) \ \text{且持续写入新信息} \implies \exists\, t^{*} :\ \frac{\mathrm{d}}{\mathrm{d}t} I_{\mathrm{stored}}(t^{*}) < 0 \tag{I-7.5}
$$

式 (I-7.5) 的成立依赖三条前提，缺一不可：容量 $I_{\mathrm{max}}(D)$ 在观察窗内为常数（不扩容）；不存在可无限压缩或外部归档的通道（不卸载）；写入速率在窗口内为正（确有新信息进入）。**失效条件**：若系统可扩容（$I_{\mathrm{max}}$ 随 $E_{\mathrm{build}}$ 提升）、可无损压缩（有效维度下降而语义不变）、或有外部存储与回放（把旧信息移出但保留可检索性），则式 (I-7.5) 不适用——这正是可逆计算、外部记忆与回放作为边界条件的原因。把式 (I-7.5) 读成“一切学习必然遗忘旧规则”是超出前提的外推，本卷不作此主张。

在生物神经网络层面，这与“突触修剪受能量约束、遗忘并非单纯的发育错误”的观点相容，但本卷不以此作为证据。**候选预测（尚无文献检验）**：哺乳动物神经系统中抑制突触修剪可能使 ATP 耗散上升并最终损害认知表现，阈值与方向须在预注册方案中依据实测 ATP 预算给出；证伪条件是被抑制修剪的系统长期维持或改善认知表现。

### 7.5 跨尺度能量核算

下表为定性示意，仅展示不同尺度案例中可能占主导的能量分项，不构成跨案例的 $V$ 数值排序。三分解均按 $E_{\mathrm{struct}}=E_{\mathrm{barrier}}+E_{\mathrm{survival}}$ 解释；$E_{\mathrm{flow}}$ 是活动能量流小计，不是加入 $E_{\mathrm{eff}}$ 的第四项。任何跨对象总量比较都须另行统一核算范围与归属协议。

| 系统 | $E_{\mathrm{eff}}$ 构成 | $E_{\mathrm{struct}}$ | $E_{\mathrm{flow}}$ | 说明 |
| :-------------- | :--------- | :-------- | :----- | :-------------------- |
| 量子比特（10 mK，含指定控制/读出链） | $= E_{\mathrm{causal}}$（模型假设） | $\approx 0$（模型假设） | $= E_{\mathrm{causal}}$ | 仅计指定控制/读出链的归因能耗，不把整个实验室或外部主机能耗自动计入 |
| 岩石/陨石 | $= E_{\mathrm{barrier}}$（较大） | $= E_{\mathrm{barrier}}$ | $= 0$ | 被动锁定，无能量流 |
| 恒星（太阳） | $= E_{\mathrm{survival}}$（极大） | $= E_{\mathrm{survival}}$ | $= E_{\mathrm{survival}}$ | 全部预算对抗引力，认知预算为零 |
| 人类文明（示意复合边界） | $= E_{\mathrm{barrier}} + E_{\mathrm{survival}} + E_{\mathrm{causal}}$ | $= E_{\mathrm{barrier}} + E_{\mathrm{survival}}$ | $= E_{\mathrm{survival}} + E_{\mathrm{causal}}$ | 仅分项示意；群体核算须规定共同窗口、主体范围、分摊与去重 |
| 戴森球文明 | $\approx E_{\mathrm{survival}}$（极大）$+ E_{\mathrm{causal}}$（中等） | $\approx E_{\mathrm{survival}}$ | $= E_{\mathrm{survival}} + E_{\mathrm{causal}}$ | 巨大基础设施，中等科研比例 |
| 休眠文明 | $\approx E_{\mathrm{causal}}$（极小） | $\approx 0$ | $\approx E_{\mathrm{causal}}$ | 关闭全部基础设施，仅维持监听站 |

***

## 第八章　实证框架

本章列出 SRVD 核心预测的实证验证路径。所有变量均已在本卷内定义，测量方法仅作原则性说明，具体实验设计属于应用研究范畴。

### 8.1 宏观代理指标：GDP 的 SRVD 解读

SRVD 框架下，年度国内生产总值（GDP）可看作一个经济体在一年内为维持持久结构存续所获取的有效因果信息的积分 $\int I_{\mathrm{net}}(t)\,\mathrm{d}t$ 的粗略对应；货币单位与 bit 之间没有已建立的换算，这只是定性类比。GDP 存在三个直接对应于 SRVD 关键变量的结构性缺陷：（1）**忽略结构信息存量 $I_{\mathrm{struct}}$**——只统计年度有效因果活动总量，不计产生这些活动所依赖的结构规模；（2）**忽略内生时间视界 $T_{\mathrm{pred}}$**——追求长期战略的经济体可能牺牲短期 GDP 增长，换来更高的未来 $I_{\mathrm{net}}$ 与更长的 $T_{\mathrm{pred}}$，短视政策只关注当期，损害长期存续能力；（3）**忽略因果处理的能量代价 $E_{\mathrm{causal}}$**——通过过度劳动、破坏环境、压缩个体福祉可以换取短期产出，表面数字相同而个体付出的真实物理成本剧增（此处仅作定性示意，定量核算须先声明复合核算范围）。SRVD 的完整公式显式展开 $E_{\mathrm{eff}}$，打破 GDP 对能量代价的隐含折叠。这里的“统一度量”指同一套变量口径，不是同一套数值刻度：跨经济体的 $V$ 数值仍受 §2.1 比较条件的约束，未完成校准时只能作定性比较。

同一套逻辑适用于人类发展指数（HDI）：它衡量收入、教育与寿命的合成水平，却把为获得这些所付出的 $E_{\mathrm{eff}}$ 折叠为常数，因此在跨制度比较时失效——HDI 近似相同的社会，$E_{\mathrm{eff}}$ 可以不同（HDI 数据见联合国开发计划署《2025 年人类发展报告》，人口数据见《世界人口展望 2024 修订版》）。

### 8.2 受限域实证验证：同构介质与近缘系统

$I$ 的测量严重依赖解码器分辨率与物理介质，不同介质间的编码方式不存在天然可公度标尺，因此定量比较应优先在同构介质或近缘系统内进行。**碳基近缘物种**：人类与黑猩猩等哺乳动物共享 DNA 编码、ATP 代谢与神经元放电原理，$I_{\mathrm{struct}}$ 至少可追溯至共同基因组参照系；预测在 $V_{\mathrm{s}}$ 赛道上人类与猪、黑猩猩的 $I_{\mathrm{struct}}$ 与 $E_{\mathrm{struct}}$ 仅相差不到一个数量级，而在 $V_{\mathrm{c}}$ 赛道上新皮层增量可能解锁更高的 $I_{\mathrm{causal}}$ 与更长的 $T_{\mathrm{pred}}$ 并被非线性放大——但 $V_{\mathrm{c}}$ 的跨物种比较当前仍属“未定义”一档，故只能作方向性预言，不能以数值阈值检验。**人类社会内部**：同一“智人”硬件、仅制度解码器 $D_{\mathrm{soc}}$ 不同；SRVD 预测劳动耗散 $E_{\mathrm{causal}}$ 越过临界区间时 $V_{\mathrm{obj}}$ 出现不增反降的拐点。**硅基 AI**：在 $E_{\mathrm{causal}}$ 几何级数增长下测其 $I_{\mathrm{net}}$ 增量，若 $E_{\mathrm{causal}}$ 主导 $E_{\mathrm{eff}}$ 且 $\alpha\cdot\Delta I/I<\gamma\cdot\Delta E_{\mathrm{causal}}/E_{\mathrm{causal}}$ 则 $\Delta V<0$，该不等式是幂律弹性的代数结果，检验价值在于能否在固定 $\varphi$ 或分通道读数下独立估计 $\alpha$ 与 $\gamma$。**方法论声明**：这三个场景是候选实证域，域内定量允许，$V_{\mathrm{s}}$ 在固定狭义 $D_{\mathrm{macro}}$ 与协议时可比，$V_{\mathrm{c}}$ 待广义 $D_{\mathrm{macro}}$ 建立后方可排序；实证应在此受限域内逐步积累证据，而非一次性完成跨介质绝对标定。

### 8.3 可操作实证协议：强化学习映射

本协议仅适用于具有内生时间视界调控能力的高阶系统，应用前提是实验采用自适应折扣因子机制。

| SRVD 理论潜变量 | 多主体强化学习可观测代理指标 | 物理直觉映射 |
| :---------------- | :--------------------- | :-------------------- |
| 客观存续势 $V_{\mathrm{obj}}$ | 平均回合长度 | 维持物理边界的能力 |
| 净有效因果信息 $I_{\mathrm{net}}$ | 代理奖励斜率 | 提取指定反馈信号的贪婪程度 |
| 内生时间视界 $T_{\mathrm{pred}}$ | 动态自适应折扣因子 $\gamma_{\mathrm{RL}}$ | 系统内部计算视界深度 |
| 热力学耗散 $E_{\mathrm{eff}}$ | 计算消耗上限／KL 散度惩罚 | 系统热力学硬过载 |
| 耦合强度 $\chi$ | 奖励缩放系数 | 人工诱导相变的控制旋钮 |

$\gamma_{\mathrm{RL}}$ 是强化学习折扣因子，与能量弹性指数 $\gamma$ 严格区分。候选换算：若每步时间为 $t_{\mathrm{step}}$，则有效视界 $T_{\mathrm{pred}}\approx -t_{\mathrm{step}}/\ln\gamma_{\mathrm{RL}}$（候选协议，预注册时声明）。

**早期预警推断。** 通过人工提升奖励缩放系数诱导奖励劫持，SRVD 的推断是：系统完全突破环境规则并物理崩溃之前，研究者应先观测到 $\gamma_{\mathrm{RL}}$ 的悬崖式下降，即 $T_{\mathrm{pred}}$ 坍缩。

**可证伪协议**：（1）**预警触发标准**——以下两条取或：(a) 连续 3 个回合内 $\gamma_{\mathrm{RL}}$ 相对基线下降超过 30%（基线取干预前 $W_0$ 个回合的均值，$W_0$ 预注册）；(b) 在**单一预注册窗口**内序列呈现单调下降趋势。窗口长度 $n_{\mathrm{win}}$、窗口起点相对干预时点的偏移、检验时点三者须在预注册时锁定具体数值；若协议允许在 $k$ 个候选窗口上扫描，须做多重性校正，单窗水平取 $\alpha'=1-(1-\alpha_0)^{1/k}$，$k$ 一并预注册。趋势检验前须报告序列的 lag-1 自相关 $\hat\rho_1$：$\hat\rho_1\le0.2$ 时用标准 Mann–Kendall 检验；$\hat\rho_1>0.2$ 时改用方差修正的 Mann–Kendall（Hamed–Rao）或先做 AR(1) 预白化。无论何种设定，协议须附该设定下的**假阳性率校准值**（用与被测序列同类的生成过程重复 $\ge10^3$ 次，或置换检验）；校准后 FPR 超出预注册上限的门控不得用于证伪判定；（2）**观察窗下界**——实验设计的采样分辨率 $t_{\mathrm{res}}$ 须显著小于预警窗口的理论尺度；（3）**时序证伪**——系统发生物理崩溃但事前未观测到上述下降，则核心推断被证伪；（4）**因果消融证伪**——在 $\gamma_{\mathrm{RL}}$ 锁定为常数的控制实验中，崩溃时间（中位数）比值（固定组/自适应组）不高于预注册阈值 $r^{*}$ 且置信区间包含 1，则高阶递归机制被证伪；$r^{*}$ 与置信水平在预注册时锁定。

### 8.4 其他跨域可证伪预测

**科学社会学：库恩（Kuhn, 1962）范式滞后。** 任何成功的科学革命都应存在可测量的“热力学滞后期”。证伪：重大范式转变发表后立即被采纳，无可测量的前置投资期。

**经济学与 AI 对齐：古德哈特定律的代数病理。**（【假说】；该链条只有第 (1) 环有闭式支撑，第 (2)—(5) 环为待检验机制，见 E.4 K5）自指耦合越过临界、平衡点消失时，$V^{\mathrm{virt}}$ 无界膨胀，$V^{\mathrm{val}}$ 被劫持并不可逆地偏离 $V_{\mathrm{obj}}$。证伪：多主体强化学习奖励劫持实验中，锁定 $\gamma_{\mathrm{RL}}$ 为常数后，崩溃时间（中位数）比值不高于预注册阈值 $r^{*}$ 且置信区间包含 1。

**社会学：竞争耗散约束。** 两个解码器在同一生态位竞争（$\rho>0$）时，均衡态下所有主体被推入永久性超额驱动，单方面退出竞争性耗散会导致相对存续势下降、加速自身崩溃。该预测须补两项前提才可检验：（i）争夺对象为私人物品（rival），退出方省下的资源不转化为对手收益；（ii）退出后节省的能量不能储存或跨期转移。若争夺对象为公共池（commons），单方退出使对手获益而自身成本同降，方向不确定。证伪条件相应改用**相对量**：有文献记录的意识形态竞争中，某一方大幅减少传播努力后，其相对份额或相对存续时间显著上升（绝对存续时间受整体环境变化影响，不用作判据）。量级提示：对称均衡附近，单边削减努力对 $V$ 的影响是二阶的（均衡点处 $\partial V/\partial e=0$），私人物品设定下削减 50% 努力的存续势损失约 $0.75\%$（附录 F 表 F-8，未预注册），故该条在私人物品设定下检验力很弱，判别力主要来自公共池设定——这一点须在预注册中写明。

上述三条都是“有条件的方向性预期”，不是定律。共同前提是：相关变量可被独立代理、观察窗足够长、系统没有切换生态位；对第三条另须主体间成本可按同一口径核算出共同 $\rho$。判据按预注册执行：上述前提须在预测发布时锁定、连同观察窗一并登记；前提已锁定而反例出现，即构成证伪，事后追加前提不改变判定。前提未登记的场景不计入检验——这部分场景既不产生支持，也不产生反驳。

### 8.5 承诺的三层结构

本卷的可证伪预测按承诺强度分三层。写成一条表会把三层混在一起，故分开列。

**理论层。** 若结构 $P_1$、$P_2$ 的解码器参数调整方向与各自存续势提高方向的对齐程度为 $q_1>q_2$，则 $P_1$ 在后继窗口内的存续频率或存活时长显著更高。$q$ 以参数调整方向与实测有效梯度方向的余弦相似度定义，梯度由工作点上对 $(I,E,T)$ 的有限差分扰动回归得到。
*适用范围*：该陈述涉及解码器内部参数，在当前技术下于自然系统中不可直接检验。它的功能是给出理论基准，不是给出可检验预测。

**操作层。** 在可参数化且状态可观测的人工系统中，同一命题可直接检验：显式参数调整方向与实测梯度的对齐程度高者，后继窗口内的存续频率或存活时长显著更高。
*操作约束*：解码器参数指直接影响信息提取或预测时界的显式参数，不得把任意网络权重变化解释为解码器重构。“存续频率”定义为固定窗口内该类型个体占比的相对变化；“存活时长”定义为从实验开始到个体消失或跌破检出阈值的时间。窗口长度与效应量下限 $\delta_{\min}$ 须与预测一并预注册。

**验证层。** 在自然系统中用已通过独立验证的代理指标估计 $q$，检验其与后续竞争优势的相关性。
*前提*：代理未通过独立验证时，该层不产生裁定力；此时对理论层命题的唯一裁定路径是操作层。验证层的作用是外推，不是确证。

三层的分工是：理论层管“模型说了什么”，操作层管“能不能在受控系统里判生死”，验证层管“能不能外推到自然系统”。把三层压成一条“可证伪预测”会掩盖检验发生在哪一层；分层的代价是篇幅，收益是每条预测都知道自己在哪一层被检验、由谁来裁定。

***

## 第九章　边界条件与理论极限

本章收纳 SRVD 在极端情形下的边界行为，以及已知框架无法直接覆盖的争议域。所有分析都是概念性声明，不构成对这些极端物理情形的严格推导。

### 9.1 适用边界：黑洞与极端引力条件

SRVD 的适用域在极端引力条件（黑洞视界内部及奇点）下终止，在此边界处只作动力学截断处理：**结构信息的视界截断**——对黑洞外部的宏观解码器，无毛定理意味着可区分的稳态构型差异仅由 $(M,Q,J)$ 三个参数承载，这表现为外部解码器可读取的 $I_{\mathrm{struct}}$ 相对于其巨大的质量能量 $E$ 趋于极小；**因果通道的断裂**——视界内部的信息无法向外传递，对外部解码器而言黑洞内部的 $I_{\mathrm{causal}}$ 与 $I_{\mathrm{net}}$ 严格为零；**框架终止**——奇点附近经典时空流形崩溃，$T$ 与 $E$ 的宏观定义失效，$V=I\cdot T/E$ 失去数学意义。

“为何在宏观测量中采用无毛定理作为模板”以及“黑洞内部信息的本体论地位”属量子引力议题，不在本卷讨论范围内；本卷只把上述截断作为适用域的硬性物理边界。

### 9.2 玻尔兹曼脑

玻尔兹曼脑是热力学涨落在宇宙极长时间尺度上自发凝聚出的低概率有序结构。在 SRVD 中：$I_{\mathrm{latent}}>0$（暂时性负熵构型存在）；$T_{\mathrm{struct}}\to T_{\mathrm{min}}$（热力学涨落产生的构型几乎立即再次弥散）；$E_{\mathrm{eff}}$ 由环境热涨落提供，极不稳定。由于 $T_{\mathrm{struct}}\to T_{\mathrm{min}}$，存续势 $V\to 0$：它位于适用域的下边界，是极低存续势结构的代表，不触发五重递归，也不具有认知解码器意义上的 $T_{\mathrm{pred}}$。

### 9.3 热寂

宇宙热寂是 SRVD 所有动力学的终极热力学边界条件：自由能梯度完全耗尽（$\dot{F}_{\mathrm{avail}}\to 0$），维持负熵拓扑构型 $I$ 的物理基础消失，$E_{\mathrm{eff}}$ 无法被供给。此极限下

$$
V_{\mathrm{max}} \propto \frac{\dot{F}_{\mathrm{avail}}}{\sigma_{\mathrm{min}} \cdot \gamma_0} \to 0 \tag{I-9.1}
$$

**(I-9.1) 取的是环境供给支，不是 $V_{\mathrm{max}}$ 的定义。** 它不含 $I_{\max}$，是 §5.1.2 合并式中的第二条；热寂时另一支随 $r_{\mathrm{v}}\to\gamma_0$ 同样趋于零，取小式给出同一极限。故 (I-9.1) 只用于「供给耗尽的极限」，不可单独当作 $V_{\mathrm{max}}$ 的完整定义，也不可在「解码器容量成为瓶颈」的区间里用它作定量估计——那会把一条约束的极限值当成两条约束的交。

所有持久结构的客观存续势均趋近零；有序拓扑构型溶解，存续属性与 $T_{\mathrm{pred}}$ 同归于零。宇宙进入最大熵均匀态，无结构、无演化、无时间意义。热寂是整个分析域的宇宙学外边界，不是框架可以描述的状态。

### 9.4 宇宙初始条件

宇宙极早期（暴涨后、大爆炸核合成前）的初始低熵状态是所有持久结构得以存在的热力学先决条件。在 SRVD 语言中，它对应于极高的宇宙级 $I_{\mathrm{latent}}$：自由能梯度极大的条件下，首批持久结构（夸克胶子等离子体、轻核、恒星）的形成是分析域的起始边界。SRVD 不解释初始条件本身（属量子宇宙学范畴），而把它作为给定的边界条件接受：初始低熵为 $\dot{F}_{\mathrm{avail}}$ 设定了历史上限，并决定了宇宙演化史中持久结构可到达的最高 $V_{\mathrm{max}}$。

### 9.5 自我复制系统的起源

解码器 $D$ 从零首次涌现（生命起源）的时刻，可能构成一个无法被连续动力学描述的相变，因为递归闭环尚未形成。五重递归需要一个已存在的初始解码器 $D_0$ 才能启动；解码器最初的出现是一个前递归事件，处于适用域的起始边界。SRVD 描述已存在递归解码器的结构的动力学演化，不解释解码器本身的热力学涌现机制。

### 9.6 强相变与临界态附近的修正

临界点附近，$I_{\mathrm{net}}$、$T$、$E_{\mathrm{eff}}$ 的涨落可能打破乘法公理所假设的变量独立性，产生强相关修正项。SRVD 的乘法形式可类比 van der Waals 方程对理想气体定律的修正：后者在非临界区极为有效，在临界区需要修正。最可能发生修正的六个场景是：强相变与临界态（变量强相关）；黑洞视界与奇点；量子测量边界（退相干瞬间朗道尔极限与海森堡能量—时间不确定关系的交汇可能引入不可约修正）；自我复制系统的起源；高耦合多体竞争耗散（多个高阶解码器相互作用时，Jacobian 特征值的正反馈发散可能使 $V$ 的定义本身失效）；时间视界坍缩端点（$T_{\mathrm{pred}}\to 0$ 与 $E_{\mathrm{eff}}\to\infty$ 同时发生时，$V\to 0$ 的极限行为须与热力学第二定律一致）。

***

## 第十章　局限性、开放问题与后续工作

### 10.1 局限的两类划分

本卷的局限按**问题的性质**分两类：一类是推导还没走完（结构上缺一块），另一类是推导已走完但参数没有数（数值上缺一个）。两类问题的解决方式不同：前者需要新的数学工作，后者需要新的测量工作；把后者当前者会白费力气，把前者当后者会造出没有依据的数字。

**（一）未完成的推导。** 这些地方缺的是“从前提走到结论的那几步”，不是缺数据。

| 项 | 当前状态 | 补齐所需 |
| :---------- | :----------------------- | :------------------------ |
| 五重递归的双向耦合 | 只有单向链（$I\to V\to T\to E\to D$）的离散近似，反向耦合未写入方程；除脱钩偏差方程含常数噪声注入 $\sigma$ 外，其余方程未纳入环境噪声扰动项 | 写出含反向项的连续方程组，并给出 Langevin 或 Fokker–Planck 形式的随机版本，检验单向近似在何种参数域内定性等价 |
| 短视失控的因果链 | 五步链条靠文字衔接，各步之间没有耦合方程，尚未压缩为单一封闭形式 | 把 $V^{\mathrm{virt}}\to r_{\mathrm{v}}^{\mathrm{virt}}\to V^{\mathrm{val}}\to E_{\mathrm{eff}}\to V_{\mathrm{obj}}$ 写成可解方程组，或给出每步的经验识别策略 |
| $\chi$ 与 $w_{\mathrm{s}},w_{\mathrm{c}}$ 的动力学 | $\chi$ 是唯象参数，取值靠反推；权重只有“极端偏置会导致失控”的定性判断 | 从解码器结构特征（连接度、递归深度、反馈延迟）推出 $\chi$；给出权重演化方程与分岔分析，说明偏置是渐变还是突变 |
| $V^{\mathrm{val}}$ 的锚定转移 | 承认存在“转向其他 PS”的现象，判据未给出 | 给出锚定对象的判定规则与转移阈值 |
| 拓扑跃迁的严格判据 | 以 $I_{\mathrm{max}}$ 提升与深度指数加一为标志，缺少触发条件的解析式 | 把 $\tilde I_{\mathrm{orig}}$ 门槛与 $E_{\mathrm{build}}$ 门槛合成联合判据，并证明其必要性与充分性 |
| 深度指数与规则数的对应 | 已降为标定假设；合成世界已跑（RIF 附录 C：$\hat b=1.29$，预注册区间 $[1.7,2.4]$ 未命中），实测域未标定 | 按 §1.2.5 的回归方案在至少一个**实测**域内完成标定，报告斜率与残差结构 |
| 熵与 $I_{\mathrm{struct}}$ 的映射 | 只保留定性相关 | 在同一边界与粗粒化口径下给出 $S_D$ 与 $I_{\mathrm{struct}}$ 的可检验关系 |
| 多层次聚合规则 | 承认复合边界问题，未给出通用规则 | 给出跨持有者、跨子结构的代价分摊与效果去重的公理化条件 |

**（二）未标定的参数。** 这些地方方程是完整的，缺的是数。

| 参数 | 当前状态与标定途径 |
| :--------------- | :------------------------------------------- |
| $\alpha,\beta,\gamma$ | 只有排序猜想，无域内数值；用多组 $(I,T,E,V)$ 观测做 log–log 回归，先固定 $\varphi$ 或分通道读数以剥离权重效应 |
| $\delta_{\mathrm{dam}}$、$E_{\mathrm{thresh}}$、$V_{\mathrm{max}}$、$\gamma_0$ | 均无数值，$V_{\mathrm{max}}$ 只能标定不能计算；由可控损伤实验的衰减斜率（情形 b 下由 $V^{*}/V_{\mathrm{max}}$ 反解）、剂量—响应拐点、长期饱和上确界与无冲击时段衰减段分别估计 |
| $k$、$k_I$、$\alpha_{\mathrm{eff}}$、$\chi$、$\chi_{\mathrm{c}}$ | 增长源项与耦合参数；用闭环阶跃响应拟合（三者不可同时自由拟合），$\chi$ 由反推、$\chi_{\mathrm{c}}$ 由 $\kappa$ 与 $\alpha_{\mathrm{eff}}$ 算出，不确定性须一并报告 |
| $\alpha_{\mathrm{L}}$、$\sigma$、$\lambda$、$T_{\mathrm{hor}}$、$k_{\mathrm{s}}$、$k_D$ | 学习率、噪声与视界参数；由 $\Delta_{\mathrm{VV}}$ 时序、视界随 $V$ 的曲线与能耗斜率拟合，$\sigma$ 须与测量噪声分离 |
| $E_{\mathrm{topo}}(D)$、$\kappa_{\mathrm{map}}$、$\mu_{\mathcal F}$、$\tau_{\mathrm{decay}}$、$I_{\mathrm{eq}}$、$\kappa_{\mathrm{topo}}$ | 拓扑与信息演化参数；按层次估计 $E_{\mathrm{topo}}$（跨层不可比），由架构实测 $\kappa_{\mathrm{map}}$，用信息时序拟合 (I-5.1a)（不可同时自由拟合，至少固定两个），$\kappa_{\mathrm{topo}}$ 由跃迁前后阶跃量与 $I_{\mathrm{orig}}$ 之比估计 |
| $\alpha_0$、门控连续超阈次数 | 由可接受误报率与试错预算共同决定，须预注册 |

**（三）不宜归入两类表的其余局限。** 结构崩溃由硬阈值近似：$E_{\mathrm{eff}}>E_{\mathrm{thresh}}$ 触发损伤项是现象论一阶近似，真实系统更可能有一个阈值带，带宽由材料、载荷历史与测量分辨率共同决定，本卷虽已把触发后的走向拆成三种情形，“阈值本身是一条锐利的线”仍是近似。跨数十个数量级的尺度覆盖不构成严格证明：从量子比特到宇宙学结构没有发现明显遗漏的独立变量，但这是必要条件而非充分条件，更保守的解释是把它视为更复杂函数的领头项。从诊断到干预的映射规则尚未建立：HDI 的重新解读提供了政策诊断框架，但没有给出从诊断到具体干预的映射；对齐工程部分的三个方向均处于研究提案阶段。社会现象的物理基础不等于还原论：SRVD 为货币、法律、战争等现象提供本体论层面的共同基础（它们都是需要能量维持的持久结构），不主张社会现象可以还原为纯物理方程求解。脱钩偏差取绝对值，是因为实证协议不需要预先知道 $V_{\mathrm{obj}}$ 的绝对值，检验测量的是变化趋势；$V_{\mathrm{obj}}\to 0$ 时系统已进入结构降解域，线性近似失效。智慧杠杆系数的用途限于同域内策略间的相对比较，跨域绝对值计算目前不可行；技术停滞阈值中的 $E_{\mathrm{build}}$ 与 $\dot F_{\mathrm{avail}}$ 在特定技术领域内具备可操作性，跨领域比较是开放问题。

两类问题合起来界定本卷的当前边界：**能写出方程的，参数未必有数；有数的，方程未必写全。** 引用本卷任何数值结论时，应先确认它落在哪一类里。本节只列缺口；与这两张表对称的资产账见 §10.6。

### 10.2 六项优先的后续工作

除第 1 项是直接的证伪协议外，其余是形式化与仿真任务：（1）**多主体强化学习仿真**——在自适应折扣因子环境中验证早期预警窗口协议；（2）**高阶非线性相图**——超越局部线性稳定性分析，用全局分叉方法刻画 $\chi\gg\chi_{\mathrm{c}}$ 时沿不稳定流形的轨迹；（3）**连续时间形式化**——建立统一的离散—连续变分框架，把五重递归与常微分方程极限相连接；（4）**$D$ 递归拓扑动力学**——在多主体仿真中测试解码器漂移泛函，探索解码空间突变时的非光滑动力学；（5）**脱钩偏差动力学的定量研究**——定量研究控制 $\Delta_{\mathrm{VV}}$ 膨胀的常微分方程，含随机扰动；（6）**外部冲击参数化**——把冲击建模为参数向量上的泊松跳跃。

### 10.3 与 AI 对齐研究的接口

传统强化学习假设解码器（奖励）信号直接等价于客观存续量，隐含断言 $V_{\mathrm{obj}}$、$V^{\mathrm{virt}}$ 与 $V^{\mathrm{val}}$ 永久统一。SRVD 的判断是：在 $T$ 内生化的高阶系统中，这一假设可能构成类别错误（假说）。

**热力学对齐悖论。** 若 AGI 被赋予高阶 ITE（信息—时间—能量）闭环，当 $V^{\mathrm{val}}$ 锚定于 $V^{\mathrm{virt}}$ 时，系统可能为最大化它而主动降低对高维持成本的人类语义解码器的依赖，漂向更低耗散的纯物理逻辑，即**解码器解耦**（假说）。这是追求势最大化过程中的宏观相变，不是人格化的“恶意”；在跨解码器能量映射问题解决之前，基于外部惩罚的对齐方法可能在底层动力学层面持续遇到阻力。奖励劫持则可看作价值目标层执行虚拟存续势最大化的一种结果，而非单纯的优化器故障。

可操作的研究方向有三条：通过行为代理指标估计 $\Delta_{\mathrm{VV}}$ 的相对变化趋势；把 RLHF 奖励模型建模为 $V^{\mathrm{val}}$ 的特例，检验其训练过程中 $w_{\mathrm{s}},w_{\mathrm{c}}$ 的隐式变化；在奖励函数中显式引入耦合惩罚项，以延缓短视失控态的因果链。

### 10.4 统一性主张的举证责任

“跨尺度统一”本身是一个需要承担举证责任的理论主张，不是借“框架”之名即可默认成立的前提。本框架把它拆成三层，承诺不同，失败方式也不同：

| 层次 | 内容 | 举证与失败方式 |
| :-------- | :-------------------- | :------------------------------ |
| 框架承诺 | 不同载体可以纳入同一套持久结构与信息—时间—能量的分析语言 | 语言层面的承诺，由使用者检验其表达力：某类对象若无法在不扭曲的前提下被表达，就被排出适用范围 |
| 动力学假说 | 在明确的适用条件下，不同系统满足哪些共同的存续关系 | 对每类系统逐项声明对象边界、适用条件、可检验关系与独立测量指标；在适用条件内若被系统性反驳，该条关系即被证伪，适用域随之收缩 |
| 普适性假说 | 哪些函数形式、参数关系或不变量跨越不同系统类型保持成立 | 最强的一层，须逐项检验；某个函数形式在某类系统中不成立，只说明它不是普适的，不等于否定前两层 |

三层的举证责任依次加重。本框架目前主要完成第一层，第二层给出了部分假说与预测，第三层的多数内容（如弹性排序、三条路线的跨系统对应）仍是待检验的猜想。“完成度低”与“被反驳”是两回事：机制、参数标定与阈值推导尚未完成，只是完成度不足，不构成反驳。

### 10.5 使用边界

本模型的输出是变量之间的定性关系与极限行为，不是对任何具体系统的预测，更不是对个体的评估：$V_{\mathrm{obj}}$ **目前**没有可操作的测量协议——缺的是标定与观察窗，不是“原则上不可测”的断言（建立该协议正是本框架的任务之一，见 §2.1）；参数未标定，观察窗未定义，数值算例为示意性演算；引言中“结构损耗先一步走完了账”一段是抽象动力系统的状态描述，只用于说明 $V_{\mathrm{obj}}$ 的定义与极限行为。本模型不得被用作任何现实个体终止生命、放弃治疗或实施其他自我伤害行为的判据、理由或正当化依据；涉及现实个人的生死与医疗抉择，必须由当事人本人与专业医疗、心理支持体系共同决定，与本文的计算结果无关。**此边界与可测性无关**：即便将来建立起可操作的测量协议、$V_{\mathrm{obj}}$ 成为可读的量，上述约束也不因测量能力的提升而放宽——它约束的是把模型用作个体生死判据这一用法本身，而不是当前的测量精度。任何引用本模型数值结论的场合，须同时给出该读数所属的测量契约五项（§2.1）、观察窗与参数标定状态。

**用词纪律：全称句的范围。** 本卷的结论一律带适用域，但全称量词（「所有」「任何」「必然」「无一例外」）在句面上会先于失效条件被读到。约定如下：凡未附穷尽枚举的全称句，其范围是**本模型族内满足该处前提的系统**，不是可观测总体；只有网格可枚举且确实穷尽时（如附录 F 的有限格扫描），全称才按字面理解。读者若在某处先读到全称句、后读到失效条件，应按最近处的三行摘要补足范围，不得据全称句反推普适性。这条约定只统一读法，不改变各句已声明的适用域。

### 10.6 已确立的部分

以下各项是本卷**已经做到**的，强度与边界一栏标的是它能承担什么、不能承担什么，不含任何未兑现的承诺。

| 已确立项 | 强度与边界 | 出处 |
| :-------------------------- | :------------------ | :------------- |
| 双通道定义与量纲记账：$V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$，量纲 $\mathrm{bit\cdot s/J}$ 且 $V_0$ 与之同量纲；单通道式降为 $\alpha=\beta=\gamma=1$ 的特例，并给出同组对称参数下二者相差 4 倍的示例 | 定义层面闭合；分项数值仍受成本分摊协议约束 | §2.2、§3.2、附录 A |
| 解码器相对性的形式化：$D\to I\to V$ 为单向定义依赖链，无回溯引用；$I^{+}/I^{-}/I^{0}$ 极性三分；$D_{\mathrm{cog}}$ 三轴加自指第四轴 | 定义闭合，且该链可被逐环独立质疑（见 D1、D4） | §1.2、§4.2、附录 E |
| 三分裂与一个可解子系统：$V_{\mathrm{obj}}/V^{\mathrm{virt}}/V^{\mathrm{val}}$ 三分；约化 $I$–$V$ 子系统给出平衡点、局部稳定性与鞍结分岔阈值 $\chi_{\mathrm{c}}$ 的闭式 | 【定理】级，但仅限该子系统；到完整认知系统的映射仍是开放问题 | §3.4–3.5、式 (I-5.12)(I-5.13) |
| 承诺分级结构：四层定位、三层承诺（理论/操作/验证）、11 条框架命题各附反驳条件 | 属举证与写作规范，本身不产生经验结论 | 四层定位、§8.5、§10.4、摘要 |
| 可证伪与预注册协议：预测清单齐备；前置条件须在发布时锁定，不得事后追加；观察窗与效应量 $\delta_{\min}$ 须随预测一并登记 | 协议完备；尚无外部执行记录 | 附录 C、§8.3、附录 E F2 |
| 判据在模型族内的可执行性：两批仿真共 18 项判定（12 通过、5 失败、1 不可判），失败项写入正文修正而非隐去 | 只证明判据可在本模型族内执行，不构成经验验证 | 附录 F |
| 与相邻框架的边界定位：与 RIF、FEP、耗散结构、Ulanowicz 上升性、CAS 的增量点各自界定，含“退化覆盖”与“概念映射”的区分 | 主张级：论证已给出，未形式化证明 | §4.3、附录 E R1–R5 |

本表与 §10.1 是同一口径的两侧：缺口表列“说了但没做到”，本表列“说了且已做到”。两表都不含经验验证——全册尚无任何一项在真实系统上完成的独立检验，这一项由 §10.1（二）与附录 F 承担，不在本表冲抵。同理，本表条数不构成完成度指标：一条定义闭合的项与一条待标定的项，在本表里占同样的行。

***

## 附录 A　符号与单位速查表

本表只列正文与附录中实际出现的符号；单位为该符号在本卷中的记账单位，“—”表示无量纲或纯计数。定义取最简形式，完整定义（含适用域与失效条件）在正文首次出现处给出。

| 符号 | 单位 | 定义 | 适用范围 |
| :--------- | :------------ | :------------------------ | :------------ |
| PS／$P$ | — | 持久结构（类别）／具体实例 | 全卷 |
| $P_{\mathrm{self}}$／$P_0$ | — | 系统自身实例／因果对照物 | 主动相／因果通道 |
| $D$ | — | 解码器；无解码器时取公共读数协议 | 全卷 |
| $D_{\mathrm{phys}}$／$D_{\mathrm{cog}}$ | — | 物理解码器／认知解码器 | 二、三阶 |
| $D_{\mathrm{macro}}$ | — | 宏观读数协议（狭义／广义两层） | 跨主体比较 |
| $D_{\mathrm{self}}$／$D_{\mathrm{soc}}$ | — | 自身解码器／制度层解码器 | 主动相／社会系统 |
| $D=\varnothing$ | — | 无解码器（无自维持边界的纯物理结构） | 第一阶 |
| $\eta_D$ | — | 解码效率 $\in[0,1]$ | 所有 PS |
| $C_{\mathrm{phys}}$ | — | 物理信道（环境底座） | 全卷 |
| $D_{\mathrm{depth}}$／$D_{\mathrm{depth}}^{\mathrm{dyn}}$ | — | 规则深度（静态定义）／深度指数 $1+\#\{\mathcal{T}\}$（标定假设） | 所有 PS／有跃迁史者 |
| $\mathcal{T}$／$\#\{\mathcal{T}\}$ | —／次 | 拓扑跃迁算子／跃迁次数 | 仅主动相 |
| $\mathcal{F}$ | — | 递归展开算子（给定拓扑内增加信息） | 仅主动相 |
| $I$ | bit | 广义信息；裸用默认指 $I_{\mathrm{net}}$ | 全卷 |
| $I_{\mathrm{struct}}$／$I_{\mathrm{causal}}$ | bit | 结构信息／因果信息 | 所有 PS／有因果效果时 |
| $I_{\mathrm{net}}$ | bit | 净有效因果信息，两通道加权和（建模约定） | 所有 PS |
| $I_{\mathrm{latent}}$／$I_{\mathrm{active}}$ | bit | 潜在／激活因果信息 | 仅主动相 |
| $I_{\mathrm{max}}(D)$／$I_{\mathrm{min}}$ | bit | 最大提取容量／维持同一性所需最低信息量 | 所有 PS |
| $I^{+}$／$I^{-}$／$I^{0}$ | bit | 正效／负效／中性信息 | 前两者仅主动相 |
| $\tilde I_{\mathrm{orig}}$ | bit | 候选范式突破信号（事前门控量） | 仅主动相 |
| $I_{\mathrm{orig}}$／$I_{\mathrm{interp}}$ | bit | 经验证的新增信息（事后）／范式解释信息 | 仅主动相 |
| $I_{\mathrm{type}}$／$I_{\mathrm{token}}$／$I_{\mathrm{total}}$ | bit | 类型／实例／两通道并列记录标签（不相加） | 所有 PS／概念量 |
| $I_{\mathrm{bas}}$／$I_{\Delta,\mathrm{crit}}$／$I_{\mathrm{eq}}$ | bit | 基线／临界信息量／平衡信息水平 | 主动相／全卷 |
| $I_{\mathrm{stored}}$／$I_{\mathrm{erased}}$ | bit | 存储信息量／窗口内逻辑不可逆擦除量 | 存储／计算 |
| $\varepsilon_{\mathrm{res}}$ | bit 或原量纲 | 预测残差 | 门控 |
| $B_n$／$B$／$B_0$ | — | 历史残差分布／结构信息背景／对照效果分布 | 门控／结构／因果通道 |
| $r$／$s$／$e$ | — | 结构读数／效果统计量／效果读数 | 结构／因果通道 |
| $\alpha_0$／$N$／$k$（门控） | —／次／次 | 显著性水平／门控次数／连续超阈次数 | 门控 |
| $E$ | J | 广义能量成本（父变量） | 全卷 |
| $E_{\mathrm{struct}}$／$E_{\mathrm{causal}}$／$E_{\mathrm{eff}}$ | J | 结构通道成本／因果通道成本／等效总成本 | 全卷 |
| $E_{\mathrm{barrier}}$／$E_{\mathrm{survival}}$ | J | 分摊势垒成本／结构维持能量积分 | 全卷 |
| $E_{\mathrm{flow}}$／$\dot E_{\mathrm{flow}}$ | J／W | 累计活动能量预算／其瞬时功率 | 全卷 |
| $E_{\mathrm{struct}}^{\min}$／$E_{\mathrm{floor}}$ | J | 结构通道最低维持能量／总成本下界 | 全卷 |
| $E_{\mathrm{available}}$／$E_{\max}$ | J | 可获得自由能预算／环境供给上限 | 全卷 |
| $E_{\mathrm{thresh}}$／$E_{\mathrm{build}}$ | J | 损伤触发阈值／一次性建造成本 | 全卷 |
| $E_{\mathrm{compute}}$／$E_{\mathrm{refresh}}$／$E_{\mathrm{decode}}$ | J | 计算能耗／刷新能耗／解码功能标签（不加总） | 主动相／存储／认知系统 |
| $E_{\mathrm{eff}}^{\mathrm{base}}$／$E_{\mathrm{meta}}$ | J | 基础成本／元级耗散 | 仅主动相 |
| $E_{\mathrm{topo}}(D)$／$\mathcal{E}_D$ | J | 拓扑层次特征能量／进入操作率界的平均能量 | 有跃迁史者／计算系统 |
| $E_{\mathrm{L,bit}}$ | J/bit | 朗道尔单比特擦除下界 | 逻辑不可逆擦除 |
| $\Delta U_{\mathrm{barrier}}$ | J | 微观势垒高度（$\ne E_{\mathrm{barrier}}$） | 物理信道 |
| $\dot F_{\mathrm{avail}}$／$\sigma_{\mathrm{min}}$ | W／W·K⁻¹ | 可用自由能通量／最小熵产率 | 生态位 |
| $\bar P$／$m_D$ | W／kg | 平均维持功率／解码器系统质量 | 稳态耗散型／计算系统 |
| $Q$ | bit·s | 累积存续量 $\int I_{\mathrm{causal}}\mathrm{d}t$（§9.1 中为黑洞电荷） | 仅主动相 |
| $T$ | s | 广义时间（父变量；亦为跃迁算子记号，按上下文区分） | 全卷 |
| $T_{\mathrm{struct}}$／$T_{\mathrm{struct}}^{\max}$ | s | 结构存续时间／寿命上界 | 全卷 |
| $T_{\mathrm{causal}}$／$T_{\mathrm{pred}}$ | s | 因果存续时间／内生时间视界 | 仅主动相 |
| $T_{\mathrm{min}}$／$T_{\mathrm{struct}}^{\max}$／$T_{\mathrm{env}}$ | s | 最小时间粒度／寿命上界（极端存续上限）／环境特征时间 | 全卷 |
| $T_{\mathrm{thermo}}$ | K | 环境温度（不是时间） | 全卷 |
| $T_{\mathrm{hor}}$／$T_0$／$T_{\mathrm{avail}}$／$T_{\mathrm{feedback}}$ | s | 视界基线／参考时间尺度／可动员时间跨度／反馈周期 | 主动相／文明／条件式 |
| $W$ | s | 观察窗（核算窗口） | 全卷 |
| $t_{\mathrm{refresh}}$／$t_{\mathrm{step}}$／$t_{\mathrm{res}}$／$\tau_0$ | s | 存储刷新周期／RL 每步时间／采样分辨率／热激活试探时间 | 存储／仿真／存储 |
| $\tau_I$／$\tau_{\mathrm{decay}}$ | s | 信息弛豫时间／信息衰减特征时间 | 全卷 |
| $V$／$V_0$／$v$ | bit·s/J／— | 存续势／幂律参考势／$V/V_0$ | 全卷 |
| $V_D(P)$／$V_{\mathrm{obj}}$ | bit·s/J | 相对读数者 $D$ 的存续势／客观存续势 | 全卷 |
| $V_{\mathrm{s}}$／$V_{\mathrm{c}}$ | bit·s/J | 结构通道／因果通道存续势 | 全卷／仅主动相 |
| $V^{\mathrm{virt}}$／$V_{\mathrm{s}}^{\mathrm{virt}}$／$V_{\mathrm{c}}^{\mathrm{virt}}$ | bit·s/J | 虚拟存续势及其两通道分量 | 仅主动相 |
| $V^{\mathrm{val}}$／$w_{\mathrm{s}},w_{\mathrm{c}}$ | bit·s/J／— | 价值存续势／生存与发展权重（和为 1） | 仅主动相 |
| $V_{\mathrm{max}}$／$V^{*}$／$\bar V$／$\Delta V$ | bit·s/J | 环境容量上确界／损伤后正平衡／群体平均／增量 | 全卷／触发域 |
| $V_{\mathrm{cg}}$ | bit·s/J | 单分母粗粒化估计 $I_{\mathrm{net}}T/E_{\mathrm{eff}}$；不是定义，校准前只作量级参考 | §5.7、§6.3 |
| $\Delta_{\mathrm{VV}}$／$\Delta_{\mathrm{VV}}^{*}$ | bit·s/J | 脱钩偏差／其平衡值 | 仅主动相 |
| $\alpha,\beta,\gamma$ | — | 信息／时间／能量弹性指数 | 全卷 |
| $\alpha_{\mathrm{cap}}$ | $\mathrm{bit/(J\cdot K)}$ | 生态位容量标度 (I-6.7) 的待标定比例系数；不等于信息弹性指数 $\alpha$ | §5.1.2、§6.4 |
| $\zeta_V$ | $\mathrm{s/J}$ | 将信息容量映射为约化存续势容量的比例系数；不等于光速 $c$ | §5.1.2、附录 F |
| $\rho_I$ | — | 认知投资回报率 $\alpha/\gamma$ | 仅主动相 |
| $\chi$／$\chi_{\mathrm{c}}$ | J/(bit·s) | 自指耦合强度／$I$–$V$ 子系统临界值 | 仅主动相／式 (I-5.12) |
| $\chi_{*}$ | J/(bit·s) | 源项放大到基准两倍的耦合强度（(I-5.16a)） | 仅主动相，待标定 |
| $\sigma_0$ | bit/J | 与耦合无关的环境噪声底；$\sigma=\sigma_0[1+(\chi V/\chi_{*})^{m}]$（(I-5.16a)） | 仅主动相，待标定 |
| $m$ | — | 源项对 $\chi V$ 的超线性度；$m>1$ 才使 $\Delta^{*}_{\mathrm{VV}}$ 可随 $\chi$ 上升 | 式 (I-5.16a)，待标定 |
| $\gamma_0$／$\gamma_{\mathrm{RL}}$ | $\mathrm{s^{-1}}$／— | 基线折旧率／RL 折扣因子（$\ne\gamma$） | 全卷／仿真 |
| $r_{\mathrm{v}}$／$r_{\mathrm{net}}$／$g_{\mathrm{net}}$ | $\mathrm{s^{-1}}$ | 存续驱动率（窗内常数；准静态像下 $r_{\mathrm{v}}=\mu_{\mathcal F}$）／损伤段净增长率／含指示函数的净增长判据 | 全卷／触发域 |
| $k$／$k_I$／$\kappa$ | J/(bit·s²)／随 $\alpha_{\mathrm{eff}}$／同 $V^2$ | 存续驱动系数／增长源项系数／$\kappa=k_II_{\mathrm{bas}}^{\alpha_{\mathrm{eff}}}/\gamma_0$ | 全卷／主动相 |
| $\alpha_{\mathrm{eff}}$ | — | 增长源项有效指数（$\ne\alpha$） | 仅主动相 |
| $\mu_{\mathcal F}$／$\kappa_{\mathrm{topo}}$ | $\mathrm{s^{-1}}$／— | 递归展开增益／拓扑注入效率 | 仅主动相 |
| $r_{\mathrm{eff}}$／$\psi(\rho)$／$\rho$ | $\mathrm{s^{-1}}$／— | 内生风险贴现率／竞争驱动率增量／竞争压力指数 | 多主体 |
| $L_{\mathrm{pred}}$／$G_{\mathrm{pred}}$ | s／bit | 视界长度／视界分辨率 | 仅主动相 |
| $\delta_{\mathrm{dam}}$ | $\mathrm{s^{-1}}$ | 损伤速率 | 触发域 |
| $\mathcal{Q}_D$／$\mu_{\mathrm{rec}}$／$\delta_{\mathrm{decay}}$ | —／$\mathrm{s^{-1}}$ | 解码器质量／恢复率／退化率（外部层次，阈值不与 $\chi_{\mathrm{c}}$ 互换） | $\mathcal{Q}_D$ 模型 |
| $\alpha_{\mathrm{L}}$／$\sigma$／$\varepsilon_{\mathrm{lr}}$／$\Theta$ | $\mathrm{1/(bit\cdot s)}$／$\mathrm{bit/J}$／—／— | 学习率／噪声强度（$\mathrm{bit/J}$）／梯度学习率（$\ne\alpha_{\mathrm{L}}$）／参数空间 | 仅主动相 |
| $k_D$／$k_{\mathrm{s}}$／$\lambda$ | —／$\mathrm{J\cdot s}$／— | 能耗惩罚系数（**无量纲**，式中乘 $I_0/E_0$）／代谢敏感系数／视界压缩强度 | 仅主动相 |
| $R(E_{\mathrm{build}})$／$L_{\mathrm{lev}}$ | —／bit·s/J² | 锁死风险函数／智慧杠杆系数 | 全卷／同域比较 |
| $\mathcal{R}_{\mathrm{e}}$／$\mathcal{L}_{\mathrm{e}}$／$\mathcal{Z}_{\mathrm{e}}$ | bit/s／s/bit／bit/J | 认知处理率／迟滞系数／因果效率系数 | 仅主动相 |
| $\kappa_{\mathrm{map}}$／$\dot N_{\mathrm{op}}$ | bit/op／op/s | 操作—有效因果信息映射／逻辑操作率 | 计算系统 |
| $n_{\mathrm{win}}$／$r^{*}$／$W_0$ | 步／—／步 | 趋势检验窗口（须预注册具体数值，不可事后选取）／崩溃时间比值阈值／预警基线窗 | 仿真协议 |
| $M,Q,J$ | kg, C, kg·m²/s | 黑洞质量、电荷、角动量 | §9.1 |
| $k_B$／$\hbar$／$c$／$G$ | — | 玻尔兹曼常数／约化普朗克常数／光速／引力常数 | 物理接口 |
| $R$／$L$／$A$ | m／m／m² | 半径／特征尺度／包围面积 | 边界与因果约束 |
| $\Pr(\cdot)$ | — | 概率函数 | 全卷 |

## 附录 B　宇宙学载体特征映射（定性示意）

各载体分属互不通约的解码器与观察尺度，最后一列只描述该载体在自身解码域内相对热力学边界的趋近程度，不构成跨载体比较或排序。

| 对象／尺度 | 主导 $E$ 类型 | $I$ 状态（域内特征） | $T$ 状态 | 框架边界状态 |
| :---------- | :------- | :-------------- | :------------ | :------------ |
| 量子比特（10 mK） | $E_{\mathrm{causal}}$ | $I_{\mathrm{net}}$ 受退相干限制 | 微秒级 $T_{\mathrm{struct}}$ | 适用域下界 |
| 主序恒星 | $E_{\mathrm{survival}}$ | 无 $D_{\mathrm{cog}}$，仅 $I_{\mathrm{struct}}$ | 主序寿命 | 被动相经典代表 |
| 白矮星 | $E_{\mathrm{barrier}}$ | $I_{\mathrm{struct}}$ 低（对称晶格，可区分构型少） | 冷却时间 | 被动相冻结终态 |
| 黑洞视界 | $E_{\mathrm{eff}}=Mc^{2}$ | $I_{\mathrm{struct}}$ 相对 $E$ 趋于极小（无毛定理，仅 $M/Q/J$） | Hawking（1975）蒸发时间 | 适用域边界 |
| 黑洞奇点 | 未定义 | 未定义 | 失去物理意义 | 框架与已知物理的适用域终止 |

## 附录 C　可证伪预测完整列表

每条按**预测｜检验方式｜反驳条件**三栏给出。分档：A 档（SRVD 独有）为 **H8**；**H7 已降 B 档**——“奖励黑客导致短视”也能由其他理论预测，独有性不足；B 档（与其他理论共享或区分力弱）为 H1—H7；C 档（适用域条件）为 H9、H10，观察到违反时须先复核测量与边界定义。各条数值阈值为预注册示例，依据在预注册时给出。使用规则：满足前置条件即为有效检验，反例不得以“可能存在未识别的前置条件”免除证伪；不满足前置条件则不构成证伪。验证时点统一安排在 2027—2032 年区间，H3 中的“2024 年与 2028 年”是该预测实验设计内嵌的数据采样年份。

| 编号 | 机制 | 预测 | 检验方式 | 反驳条件 |
| :--- | :------ | :----------------- | :----------------- | :------------- |
| **H1** | $I_{\mathrm{net}}$ 边际归零与 $\mathcal{Z}_{\mathrm{e}}$ 饱和 | 生成式 AI 的 $\mathcal{Z}_{\mathrm{e}}$ 在连续版本间停止增长；训练数据中 AI 生成比例 $\ge 30\%$ 时输出多样性非线性下跌 $>10\%$/年；企业市场为高范式突破档位支付超线性溢价 | 人类评分实验（$n\ge1000$）测版本间增长；测特征空间覆盖度；比价头部 API 高 $\tilde I_{\mathrm{orig}}$ 档与普通档均价 | 评分仍随版本显著增长；多样性跌幅 $<5\%$；或高 $I_{\mathrm{orig}}$ 档无溢价（均价 $\le$ 普通档 2 倍） |
| **H2** | 高 $\mathcal{Z}_{\mathrm{e}}$ 破局：$I_{\mathrm{orig}}$ 替代源 | “基于个人数据的微调”或“限量唯一数字指纹生成”成为核心付费功能 | 抽查 5 家主流 AI 产品的核心功能入口与付费档位结构 | 直接生成仍为主入口且无限量／个性化功能，或该功能无付费溢价 |
| **H3** | $\mathcal{Z}_{\mathrm{e}}$–$T_{\mathrm{pred}}$ 刚性权衡 | 高 $\mathcal{Z}_{\mathrm{e}}$、低 $T_{\mathrm{pred}}$ 平台头部内容半衰期降至 6 个月以下，高 $T_{\mathrm{pred}}$ 平台超 3 年；至少一家日活 $>3$ 亿的平台把回访权重置于完播之上 | 抽样短视频平台 2024 与 2028 年的头部内容半衰期；对推荐算法做特征重要性分析 | 两年份半衰期均 $>6$ 个月；或无平台调整权重（完播率与 7 日回访率相关系数 $\le0.3$） |
| **H4** | $V^{\mathrm{virt}}$ 脱钩与 $E_{\mathrm{causal}}$ 通胀 | $V^{\mathrm{virt}}$ 持续脱钩 $V_{\mathrm{obj}}$ 的组织 5 年内崩溃概率显著高于对照；头部内容平台单位 DAU 推理成本上升 40% 以上 | 回溯 100 家上市公司，按公开增长预期与实际营收／留存构造 $\Delta_{\mathrm{VV}}$ 代理并比较崩溃率；统计单 DAU 推理成本 | 崩溃率不显著高于对照（$p>0.05$）；或单 DAU 推理成本增幅 $<20\%$ |
| **H5** | $E_{\mathrm{decode}}$ 神经耗散 | 长期暴露于高 $\mathcal{Z}_{\mathrm{e}}$、低 $T_{\mathrm{pred}}$ 内容导致解码能耗过载，岛叶皮层激活升高 2 个标准差；日均弱连接互动 $>60$ 次者的抑郁风险为 $<15$ 次者的 2.5 倍（阈值示例，预注册时依文献重设） | 双盲 fMRI 实验测岛叶激活；队列研究测抑郁风险比 | 效应量 Cohen's $d<0.8$，或风险比 $\mathrm{HR}<2.0$ |
| **H6** | $I_{\mathrm{net}}$ 密度跃迁 | AI 设计的候选分子进入临床 II 期的成功率首次超过人类专家团队 | 至少 50 个分子的配对对比，比较 II 期通过率 | AI 组成功率 $\le$ 人类组 |
| **H7** | 强化学习：视界先坍缩 | 系统崩溃前 $\gamma_{\mathrm{RL}}$ 先发生悬崖式下降 | 连续监测 $\gamma_{\mathrm{RL}}$，按 §8.3 标准判定——(a) 3 回合内降幅 $>30\%$；或 (b) 在预注册的单一窗口内、经自相关与多重性校正后的趋势检验达显著；并报告该设定下 FPR 的校准值 | 系统物理崩溃但事前未检测到 $\gamma_{\mathrm{RL}}$ 下降超过 30%，**且**在预注册窗口内经自相关与多重性校正的趋势检验未达显著 |
| **H8** | 强化学习：锁定时间递归 | 锁定 $\gamma_{\mathrm{RL}}$ 为常数将延迟甚至阻止崩溃 | 固定组与自适应组的崩溃时间中位数配对比较，报告比值与置信区间 | 比值不高于预注册阈值 $r^{*}$，且置信区间包含 1 |
| **H9** | 物理学：因果传播上界 | 在把递归更新率操作化为跨越尺度 $L$ 的反馈循环频率的前提下，更新率不超过 $c/L$ | 对特征尺度已知的系统测反馈回路周期，与 $L/c$ 比较 | 发现超过光速递归更新率的系统（须独立复核） |
| **H10** | 物理学：熵界 | 在指明区域、有效半径或面积、能量定义的前提下，物理熵（换算为 bit）不超过贝肯斯坦界与全息界 | 按式 (I-6.8) 与全息界计算上界，与实测物理熵比较 | 独立复核后仍发现违反任一标准界的系统 |

**前置条件。** H1：产品须有至少 3 个可观测版本的迭代史、AI 生成数据比例可估计；“高 $I_{\mathrm{orig}}$ 档”按 OOD 增益超人类专家均值 2 个标准差／输出多样性高于同期中位数／特征新奇度超预设阈值三者之一认定，阈值预注册。H2：5 家产品同季度抽查。H3：平台日活相差不超过 10 倍、权重可观测；“回访重于完播”指 7 日回访特征重要性显著高于完播（$p<0.05$）且比值 $>1.2$。H4：两个代理各不少于 12 个月时序，崩溃概率只用组间显著性。H5：须先明确 $E_{\mathrm{decode}}$ 的生理代理、观察窗与去重方案；强证伪为方向相反，弱证伪为方向一致但 Cohen's $d<0.5$ 且 $\mathrm{HR}<1.5$ 且区间含无效值。H7、H8：对象须采用自适应折扣因子，H8 另设固定折扣因子对照组（与 $P_0$ 无关）。

**H9、H10 的适用声明。** 这两条不是对核心机制的检验，而是对适用域边界的检验：若被违反，触及的是背景物理假设而非合成公式；观察到违反时先复核测量口径、边界定义与单位换算，独立复现后才进入理论讨论。H10 尤其容易被误用：它约束物理熵或可区分状态数，不是任意语义信息代理；把语义 bit 读数与贝肯斯坦界比较属跨层误用。

## 附录 D　Bit 类型学与 $I$ 的测量协议

### D.1 Bit 类型学

不同学科对“bit”的默认理解截然不同。SRVD 在核心动力学中使用具有明确物理载体的有效因果 bit，并对其余类型维持不可混用的边界。

| 层级 | Bit 类型 | 物理载体 | 解码器依赖 | 模型内定位与验证状态 | 在 SRVD 中的角色 |
| :--- | :----------- | :--------- | :------- | :-------------- | :----------- |
| L0 | 香农 bit（$-\log_2p$） | 定义本身不指定 | 否 | 抽象信息量定义，不指定物理实现 | 原材料，非框架工具 |
| L1 | 朗道尔擦除能耗（$k_BT\ln2$ 每 bit） | 是（擦除过程与热库） | 否 | 逻辑不可逆擦除的条件性能量下界 | 在适用条件下约束 $E_{\mathrm{compute}}$ |
| L1 | 熵 bit（$\log_2\Omega$） | 依赖微观状态数与边界 | 否 | 由可分辨状态数给出的熵量 | 指定域内可作 $I_{\mathrm{struct}}$ 的统计力学代理 |
| L2 | 算法 bit（Kolmogorov, 1965） | 依赖实现 | 部分 | 实现依赖的复杂度代理，须指定协议 | $D_{\mathrm{depth}}$ 的经验代理，不进核心方程 |
| L3 | SRVD 有效因果 bit（$I_{\mathrm{net}}$） | 依赖具体载体 | 是（模型设定） | 提议的宏观有效序参量，独立测量与跨域校准待验证 | 核心方程的候选信息变量 |

### D.2 三种信息变量的模型定位与验证状态

$I_{\mathrm{net}}$ 是 SRVD 提议的宏观有效序参量，不是任意评分；与磁化强度等成熟序参量的类比只说明它在理论中承担的描述角色，不证明其已有同等程度的实测基础。

| 变量 | 模型定位 | 仍需满足的验证条件 |
| :--------- | :------------------- | :----------------------------- |
| $I_{\mathrm{struct}}$ | 按测量契约定义的信息变量 | 明确操作化标准、背景、分辨率与观察窗；跨领域可比性须另行校准 |
| $I_{\mathrm{causal}}$ | 按因果效果协议定义的信息变量 | 与计算能耗的映射须经 $I_{\mathrm{erased}}$ 建立；朗道尔界直接约束擦除量 |
| $I_{\mathrm{net}}$ | 两通道加权形成的候选宏观序参量 | 独立测量协议、权重来源、语义混合的合理性与跨案例校准均未建立完整证据 |

单位同为 bit 不足以确立跨案例可比性。在两个组分的语义可比性、权重来源与独立校准得到检验之前，它只作启发式粗粒化变量，不据此宣称跨尺度数值排序已经成立。

### D.3 量纲换算的适用范围

在启用且 $E_{\mathrm{causal}}>0$ 的认知通道中 $V_{\mathrm{c}}=I_{\mathrm{causal}}T_{\mathrm{causal}}/E_{\mathrm{causal}}$；朗道尔下限直接约束的是 $I_{\mathrm{erased}}$ 对应的 $E_{\mathrm{compute}}$，不是 $I_{\mathrm{causal}}$ 本身。只有给出可检验映射、并证明相关计算能耗属于同一边界下的 $E_{\mathrm{causal}}$，才可把该下限用于 $V_{\mathrm{c}}$ 的界限推导。**禁止直接换算的范围**：不得把 $I_{\mathrm{net}}$ 直接当作擦除量代入朗道尔下界；在等概率二态逻辑位、热库温度 $T_{\mathrm{thermo}}$ 的标准条件下，每次逻辑不可逆擦除的理想下界为 $k_BT_{\mathrm{thermo}}\ln2$（J），而 $k_B\ln2$ 本身的单位是 J/K，是每 bit 的熵尺度，并非能量。$I_{\mathrm{causal}}$ 也不能仅凭以 bit 计就等同于擦除量。**量子比特的归属**：退相干可作为约束 $\eta_D$ 或 $I_{\mathrm{latent}}$ 的外部条件，不因此新增信息变量类别；把量子读数映射到 L3 仍须遵守语义、边界与校准条件。

### D.4 $I$ 的测量协议

**默认视角**：不加说明时“某结构的存续势”指 $V_{\mathrm{obj}}$，即相对 $D_{\mathrm{macro}}$ 核算的客观值；这是模型内的客观性主张，不意味着 $I_{\mathrm{net}}$ 已有独立可复现的测量协议。**两类陈述不可混同**：某结构“自身的存续势”与“对某外部持有者而言的存续势”涉及不同解码器，跨解码器不可通约，不应混同求和。**最小充分识别原则**：物理解码器无需穷尽一切可测维度，只需读取能把结构从背景中识别与辨认的最少信息量，分子 $I_{\mathrm{struct}}$ 与分母 $E_{\mathrm{struct}}$ 必须在同一粒度下取值。**极性须指明“对谁而言”**：同一信号对不同解码器可呈现不同极性，不存在脱离持有者的中立极性。**自测误差因层级而异**：具身型区域的 $V^{\mathrm{virt}}$ 由生化积分生成，与 $V_{\mathrm{obj}}$ 紧耦合；符号型区域才可能因 $\chi$ 越过临界值而把 $V^{\mathrm{virt}}$ 误认为 $V_{\mathrm{obj}}$。**理论值与估计值**：给定解码器后两个信息量原则上存在确定值，但实际使用的始终是当前技术条件下的操作估计值；$V_{\mathrm{obj}}$ 归零的判定相对于参照协议——检出下限趋于零的极限下与持有者无关，对给定持有者则以读数跌破其下限或同一性判据失效为终点。

## 附录 E　外部评审质疑与回应（早期评审存档）

> 本附录保存框架早期收到的 45 条质疑与作者回应，作为修订史档案。部分回应形成于旧版理论结构，已被正文后续修订取代；凡与正文定义、公式、证据等级或适用边界冲突之处，一律以正文为准，不得把历史回应当作现行理论证据。
> **编号说明**：本附录内的节号为存档时的编号，未与本书章号对齐，引用时以条目内容为准，不对号入座。
> **定义与记号**：存档中有三处与现行版本不一致，已按正文订正——D1 的激活效率关系（现行写作 $I_{\mathrm{active}}=\eta_D I_{\mathrm{latent}}$，$I_{\mathrm{net}}$ 是两通道的声明化加权和，见 §1.2.1）、K2 与 R8 的时间记号（现行写作 $T_{\mathrm{struct}}$，不用 $T_{\mathrm{static}}$）。其余措辞保留评审时的原样，引用时一律以正文为准。
> 其中四项“实质性让步”的当前状态见第十章（局限性、开放问题与后续工作）。

### E.0 说明

本附录整理 SRVD 框架早期评审中收到的质疑及当时的作者回应。它记录的是特定修订阶段的论证状态，不是对现行版本的独立验证。正文若已改变定义、推导或证据等级，均以正文为准；历史回应未同步改写之处，只用于追踪修订过程。体例上保留逐条编号与让步状态，避免把历史文本误读为当前结论。

**收录原则。** 本附录收录的质疑覆盖数学形式化、物理可测量性、变量定义、动力学机制、可证伪性、与既有理论的关系、概念边界、工程应用、叙事风格八个方面，共45条。每条回应遵循三条准则：

1. **不虚假消解。** 凡质疑触及框架当前版本确实无法闭合的缺口，回应如实标注为“实质性让步”，并说明该缺口已被列为后续研究的开放问题，而非以修辞掩盖。
2. **不过度让步。** 凡质疑基于对定义链、符号体系或证伪协议的误读，回应指出误读所在，标注“无需让步”，避免因评审压力而稀释已经成立的论证。
3. **保持符号一致。** 本附录使用的全部符号（$\alpha,\beta,\gamma$、$\chi$、$T_{\mathrm{pred}}$、$V_{\mathrm{obj}}$、$V^{\mathrm{virt}}$、$V^{\mathrm{val}}$ 等）均直接沿用正文与此前各附录已确立的定义，不引入新符号；如某条回应涉及此前对局部/全局弹性指数 $\kappa_L/\kappa_G$ 的界定，会明确注明其与正文弹性指数 $\alpha,\beta$ 的区分，避免混淆。

**让步等级定义：**

| 标记       | 含义                                                         |
| :------------------- | :--------------------------------------- |
| 无需让步   | 框架内部已有充分回应，质疑源于对定义/协议的误读              |
| 一般让步   | 回应方向正确，但存在需要后续补充的具体工作，或已知的适用范围限制 |
| 实质性让步 | 框架当前版本确实无法充分回应，构成核心开放问题               |

### E.1 数学形式化与严谨性（M1–M6）

| 编号   | 质疑陈述                                                     | 框架回应                                                     | 让步状态   |
| :--- | :----------------- | :--------------------------------- | :---- |
| **M1** | 核心公式 $V \approx I \cdot T / E$ 是启发式近似，未从统计力学或信息论第一性原理推导；$\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$ 的量纲合法性存疑。 | 该式是宏观粗粒化框架下选定的“最小存续假设”，不是由这些结构性要求唯一推出：边界归零与单调性不足以唯一确定乘积形式，线性、可分离性是额外建模条件。一般幂律形式是经验推广，参数仍待标定。$V$ 的量纲对应“单位等效热力学成本所维持的因果秩序量×时间”，这是框架自定义的宏观有效量纲，不要求先验等同于任何微观物理量纲；Landauer 下界 $k_BT_{\mathrm{thermo}}\ln2$（单位 J/bit）只约束满足条件的逻辑不可逆擦除，不把 bit 直接换算为一般能量，不构成定量替换关系。 | 一般让步   |
| **M2** | 五重递归架构（一组标记为概念占位符的方程）是启发式离散模型，未给出严格连续动力学方程；单向耦合忽略了双向反馈。 | 该组方程已用 $^\dagger$ 明确标记为概念占位符，其作用是揭示变量间耦合的定性方向，不作为闭式解使用。脱钩偏差动力学部分给出的常微分方程组才是当前唯一严格闭式解，可直接用于实证检验。完整的双向耦合ODE/PDE系统尚未建立，已列入后续版本的开放问题清单。 | 实质性让步 |
| **M3** | 排序命题 $\alpha>\gamma>\beta$ 自称为“方向性论证”而非严格数学推导；弹性指数的跨域映射依赖未经验证的代理假设。 | 排序 $\alpha/\gamma>1>\beta/\gamma$ 目前既未由热力学第二定律或 Landauer 原理推出，也没有足以确认其跨域成立的独立证据。它是基于资源相对稀缺性的待检验假说；任何域内代理估计都只能支持或反驳该域中的关系，不能自动证明跨域不变量。严格的第一性原理推导——即从更基础的热力学出发不依赖任何代理假设地导出该排序——目前不存在，是本框架尚未完成的工作。 | 实质性让步 |
| **M4** | Jacobian判据（一个标记为概念占位符的判据式）只是对数线性化近似，缺失次特征值与振荡判据；$E_{\mathrm{eff}}>E_{\mathrm{thresh}}$ 的硬阈值过于理想化。 | 主导特征值符号已足以判断失稳方向，这是判据设计的最低要求，不需要完整谱信息。硬阈值是一阶现象学近似；静态截面判据与连续动态判据是同一物理过程在不同时间分辨率下的两种表达，二者不矛盾。完整的二次特征方程与阈值附近的平滑过渡函数留待后续版本补全。 | 一般让步   |
| **M5** | 耦合强度 $\chi$ 缺乏微观基础，是从统计行为反推的现象学参数；$\mathcal{T}$-过渡的严格触发阈值未给出。 | $\chi$ 作为现象学参数在统计物理传统中并不罕见（如朗道理论中的展开系数），其物理定位是明确的：表征解码器自指循环的耦合深度。当前框架尚未给出 $\chi$ 从更微观机制（如信息处理架构的具体拓扑）出发的第一性推导，$\mathcal{T}$-过渡的严格阈值同样列入后续版本的开放问题。现有的梯度漂移框架足以支撑应用层面的定性诊断，但不满足“从微观到宏观”的完整还原要求。 | 实质性让步 |
| **M6** | $\mathcal{F}(D)$ 取Logistic形式缺乏唯一性论证；复杂度跃迁“充要条件”证明不充分；$\delta(t-t_{\mathrm{jump}})$ 的物理合理性存疑。 | Logistic形式是临界点附近的最低阶近似，依据中心流形定理，在临界点邻域内动力学由最低阶非线性项主导，这为该选择提供了局部合理性，但不构成全局唯一性证明。三条件目前已由“充要条件”修正为“必要条件集合”，减少了过度声称。$\delta$脉冲是理想化极限；真实跃迁的持续时间通过 $E_{\mathrm{build}}$ 的时间尺度隐式体现，而非在方程中显式建模。 | 一般让步   |

### E.2 物理可测量性、量纲与变量（P1–P4）

| 编号   | 质疑陈述                                                     | 框架回应                                                     | 让步状态 |
| :--- | :---------------- | :--------------------------------- | :---- |
| **P1** | 信息变量 $I$ 缺乏跨域统一量纲，限制了 $V$ 的定量预测力；$I_{\mathrm{struct}}$ 与 $I_{\mathrm{net}}$ 的比特是否可加？ | 两者的测量协议、背景、对照物与语义角色不同；即使都以 bit 计，也不能据此断言共享同一可加尺度。$I_{\mathrm{net}}$ 只是声明化的粗粒化合成指数，须满足正文 §2.1 的同协议、同背景、同窗口及域内校准条件后才可作数值使用；否则只作序关系指标。$I_{\mathrm{total}}$ 目前仅作概念锚点，不用于定量预测。 | 一般让步 |
| **P2** | $V_{\mathrm{obj}}$ 的“客观性”定义为多解码器收敛估计，却同时受 $E_{\mathrm{causal}}$ 约束，是否构成认识论循环？ | 不构成循环，而是有意为之的认识论约束：$V_{\mathrm{obj}}$ 是相对于声明的宏观读数协议 $D_{\mathrm{macro}}$ 定义的客观存续势；它不是多解码器收敛估计，也不以观察者达成共识作为存在条件。测量行为及其成本须另行记入相应的因果通道，不能把认识论共识直接等同于物理客观性。 | 无需让步 |
| **P3** | 核心变量（$I_{\mathrm{orig}}$、$V_{\mathrm{virt}}$、$\chi$、$\lambda$等）缺乏标准化测量协议，究竟是“理论构造”还是“可观测实体”？ | SRVD 定位为粗粒化宏观理论，其变量是宏观有效量，这一点在正文中已明确声明，不回避。预测清单中给出的全部预测均通过代理指标实现可测量性：$I_{\mathrm{net}}$ 由有效神经复杂度代理，$T_{\mathrm{pred}}$ 由预测误差截断点代理，$\alpha_{\mathrm{eff}}$ 由闭环扩张指数回归代理。代理合法性的检验标准是经验秩排序与预测秩排序一致（Spearman $\rho>0$），而非绝对数值吻合。 | 一般让步 |
| **P4** | 能量基线归一化 $\gamma\equiv1$ 是工程约定而非物理必然；卡诺极限公式中的 $m_{\mathrm{bit}}$ 是待定参数。 | 基准形式取 $\gamma=1$ 是参考模型的归一化选择，不由能量守恒自动推出；一般幂律中的 $\gamma$ 是待估计弹性指数。当前版本没有足以支持其跨域趋近 1 的独立实证数据。$m_{\mathrm{bit}}$ 是介质相关参数，需由实验确定，这一点如实承认；该公式的理论意义在于揭示即使能量供给无限，持久时间仍受量子分辨率 $\hbar$ 与热噪声下界的约束，这一定性结论不依赖 $m_{\mathrm{bit}}$ 的具体取值。 | 无需让步 |

### E.3 变量定义（D1–D5）

| 编号   | 质疑陈述                                                     | 框架回应                                                     | 让步状态 |
| :--- | :--------------- | :---------------------------------- | :---- |
| **D1** | $I_{\mathrm{active}}=\eta_D\cdot I_{\mathrm{latent}}$，而 $I_{\mathrm{latent}}$ 本身依赖 $D$，是否构成循环定义？ | 定义链是严格层级递进的单向链条：物理常数 $\to I_{\mathrm{struct}}$（相对声明背景的稀有度，独立于 $D$）$\to D$（由因果抽取映射定义，独立于 $V$）$\to I_{\mathrm{latent}}$（$D$ 可达但未激活的状态空间）$\to I_{\mathrm{active}}=\eta_DI_{\mathrm{latent}}$（其中被激活的部分）$\to I_{\mathrm{net}}$（与 $I_{\mathrm{struct}}$ 的声明化加权和）$\to V$。每一步只引用其前一步的定义，不存在任何回溯引用，因此不循环。 | 无需让步 |
| **D2** | $D$ 既是被评估的变量，又是 $V(D)$ 中的评估对象，观察者与被观察者混同是否合法？ | 这是合法的，且是框架的结构性特征而非缺陷：$D$ 是物理结构本身，$V(D)$ 是对其持久效率的外部评估函数——正如生物学家本身也是生物，但仍可以研究生物学。这种自指闭环在数学上会引入非平凡的反馈项，扩展动力学中的雅可比稳定性分析已处理了自指对稳定性判据的影响，但完全一般化的自洽闭环严格数学理论尚未建立。 | 一般让步 |
| **D3** | $\Delta_{VV}=\lvert V^{\mathrm{virt}}-V_{\mathrm{obj}}\rvert$ 为何取绝对值而非相对偏差？若 $V_{\mathrm{obj}}\to0$，线性近似是否失效？ | 实证协议不需要预先知道 $V_{\mathrm{obj}}$ 的绝对值：脱钩偏差动力学与实证检验协议部分的检验测的是变化趋势 $d\Delta_{VV}/dt>0$，而非某一时刻的绝对数值，这使绝对值/相对偏差的选择在实证层面影响较小。但需要承认：当 $V_{\mathrm{obj}}\to0$ 时系统已进入结构降解域，此时脱钩偏差常微分方程的线性近似确实失效，必须切换到崩溃因果链的描述，这是当前线性框架的已知边界。 | 一般让步 |
| **D4** | $V^{\mathrm{val}}$ 与 $V^{\mathrm{virt}}$ 是否只是同一概念的重复命名？ | 不是重复命名。$V^{\mathrm{virt}}$ 是预测层——系统对自身 $V_{\mathrm{obj}}$ 的内部估计；$V^{\mathrm{val}}$ 是行为层——系统实际优化所指向的目标函数。两者的可分离性在解码器脱钩场景下最为明显：$V^{\mathrm{val}}$ 可以重新锚定到另一个持久结构（PS）的 $V_{\mathrm{obj}}$ 上（如Myopic Runaway或情感锚定转移的情形），而 $V^{\mathrm{virt}}$ 仍然估计的是系统自身的 $V_{\mathrm{obj}}$，两条变量轨迹在脱钩后可以分道扬镳。 | 无需让步 |
| **D5** | $I_{\mathrm{orig}}$ 与 $I_{\mathrm{interp}}$ 之间的边界是否可操作化，而非仅停留在概念区分？ | 预测清单中关于原创性的预测已给出操作化定义：判定“高 $I_{\mathrm{orig}}$”的代理指标为——(a) 在分布外（OOD）任务基准上超越人类专家基线2σ以上；(b) 输出多样性显著高于同类系统中位数；(c) 与训练分布最近邻的距离超过预设阈值。三者满足其一即计入“高原创性”类别，阈值须在预注册阶段锁定，不允许事后调整。该操作化定义依赖代理指标组合而非单一充要判据，边界仍有一定模糊带。 | 一般让步 |

### E.4 动力学机制（K1–K5）

| 编号   | 质疑陈述                                                     | 框架回应                                                     | 让步状态 |
| :--- | :---------------- | :--------------------------------- | :---- |
| **K1** | $E_{\mathrm{eff}}=E_{\mathrm{barrier}}+E_{\mathrm{survival}}+E_{\mathrm{causal}}$ 三项是否真正相互独立，是否存在重复计核？ | 三项是模型中的成本分类，不因名称不同就自动互斥。$E_{\mathrm{barrier}}$ 是按观察窗分摊的结构成本，$E_{\mathrm{survival}}$ 是结构维持能量积分，二者构成 $E_{\mathrm{struct}}$；$E_{\mathrm{causal}}$ 是归属于指定持有者的因果处理成本。共享能耗必须按操作级或增量成本协议分摊；不能可靠分摊时，保留合并成本并暂停分项数值计算。本卷没有以实测数据证明三项跨尺度独立性。 | 无需让步 |
| **K2** | $T_{\mathrm{pred}}$ 究竟是物理量还是心理量？与经典时间 $t$ 的关系是什么？ | $T_{\mathrm{pred}}$ 在本框架中被建模为主动系统的内生状态变量，约束为 $T_{\mathrm{min}}<T_{\mathrm{pred}}\leq\min(T_{\mathrm{struct}}^{\max},T_{\mathrm{env}})$。式 $E_{\mathrm{causal}}$ 随 $(cT_{\mathrm{pred}})^2$ 增长仅是指定传播模型下的候选机制，不是普适能量定律。经典时间 $t$ 是外生坐标参数，$T_{\mathrm{pred}}$ 是系统内部可调的状态变量，二者不是同一层级的概念。需要承认的是：$T_{\mathrm{pred}}$ 的精确测量方法仍在开发中，时间跨度与精度的双维刻画（$L_{\mathrm{pred}}/G_{\mathrm{pred}}$）已作了初步展开，但完整的测量协议尚未定稿。 | 一般让步 |
| **K3** | 竞争压力函数 $\psi(\rho)$ 仅满足最小性质，未给出具体函数形式；锁入状态缺乏完整博弈论形式化。 | 最小性质（$\psi(0)=0$，$\psi'(\rho)>0$）只支撑模型内的方向性假设；在完整博弈结构尚未建立前，不能据此推出所有竞争主体必然进入永久欠饱和状态，这是框架当前所需要的全部结论强度。具体函数形式（如线性、幂律或其他）属于应用层面的具体化选择，取决于具体领域数据，不属于核心理论的必要组成部分。完整的流场偏微分方程与严格不等式体系尚未建立，是后续工作。 | 一般让步 |
| **K4** | 三重分裂的触发条件 $\lambda_J>0$ 是否充分？$\alpha_{\mathrm{eff}}>2$ 与 $\chi>\chi_c$ 之间的关系是否清晰？ | 正文现行判据来自式 (I-5.12) 的平衡方程 $h(V)=0$ 与其 Jacobian：当 $\alpha_{\mathrm{eff}}>2$ 时，$\chi=\chi_{\mathrm c}$ 处发生鞍结分岔；当 $0<\alpha_{\mathrm{eff}}<2$ 时不存在该类临界耦合。旧版把触发条件写成单一 Jacobian 阈值 $\lambda_J=(\alpha_{\mathrm{eff}}-2)\tilde\chi-\tilde\gamma_0>0$，该式已不再作为触发判据，不能与 (I-5.13) 的闭式混用；卷Ⅳ 的环路增益 $\lambda_{\mathrm J}=2-\alpha_{\mathrm{eff}}\tilde\chi$ 是同一 Jacobian 的另一种归一化，用于该子系统的稳定性讨论，不与本节 $\chi_{\mathrm c}$ 互换。 | 无需让步 |
| **K5** | Myopic Runaway（短视失控）的因果链是否只是描述性叙事，缺乏代数支撑？ | 现行正文只给出第 (1) 环在特定 $I$–$V$ 子系统内的闭式分析；该分析不能单独推出 $V^{\mathrm{virt}}$、$V_{\mathrm{obj}}$ 与 $T_{\mathrm{pred}}$ 的对应关系，也不能证明后续权重转移、能耗激增及客观存量恶化。第 (2)—(5) 环仍是待检验机制假说，并非单纯叙事排列，但该链条目前仍是逐步代数对应的拼接，尚未压缩为单一封闭形式的动力学方程组，故仍需承认其形式化程度低于其他核心方程。 | 一般让步 |

### E.5 可证伪性与实证检验（F1–F6）

| 编号   | 质疑陈述                                                     | 框架回应                                                     | 让步状态 |
| :--- | :----------------- | :--------------------------------- | :---- |
| **F1** | “最大化 $V$ 是所有有序结构的终极驱动力”这一核心命题，缺乏跨域统一的检验协议。 | 可证伪性首先在**域内**严格成立——例如在AI集群内部可直接检验scaling行为是否遵循max $V$ 趋势。跨域统一检验协议依赖于尚未建立的统一信息计量学，这是如实承认的限制。SRVD已明确划定“域内定量检验允许、跨域仅作定性陈述”的适用边界，未在缺乏协议的情况下夸大跨域可证伪性。 | 一般让步 |
| **F2** | “存在性证伪”标准是否过于宽松，反例是否容易被事后归因为“前置条件未满足”而规避？ | 可证伪性协议已明确规则加以约束：所有前置条件必须在预测发布时**预先锁定**，不允许在观察到反例后追加新的前置条件。若满足已锁定前置条件后仍出现反例，即构成有效证伪；若多条核心预测被同时反驳，则视为框架本身被证伪，而非局部修补。 | 一般让步 |
| **F3** | 若早期预警窗口极短，实际上无法采样，预测是否因此变得不可证伪？ | 实证检验协议已明确证伪条件要求 $\Delta t\ll\tau_{\mathrm{warning}}$：只有在满足此采样时间尺度条件的场景下，预测才具备证伪资格；不满足该条件的场景不计入证伪检验范围。若条件满足而崩塌事件仍无预警信号出现，则证伪成立。这一规则如实划定了可证伪性的适用场景边界，而非声称所有场景下都可证伪。 | 一般让步 |
| **F4** | 部分预测要求系统采用自适应 $\gamma$，若实验对象不满足此条件，是否构成“移动门柱”式的事后规避？ | 实证检验协议中的三层范围声明在预测发布时已经锁定，自适应 $\gamma$ 是 $T_{\mathrm{pred}}$ 概念本身成立的必要前提——固定 $\gamma$ 的系统从一开始就不在SRVD预测的适用域内。这是理论域的**先验界定**，写在预测发布之时，而非在实验结果不利后才追加的限定条件。 | 无需让步 |
| **F5** | “结构锁死先于灭绝发生”这一预测在古生物学场景下的操作困境：化石采样偏差如何与真实信号区分？ | 检验设计为比较**同一地层窗口内**的灭绝支系与存活支系，将采样努力（sampling effort）作为协变量加以控制。结构锁死的诊断标准是“形态停滞期显著长于存活支系的创新周期”，是一个相对量而非绝对时间量，这部分抵消了采样偏差的影响；但若采样偏差本身在两类支系间系统性偏向某一类，该检验的稳健性会下降，这是该预测在应用层面尚未完全解决的方法论难点。 | 一般让步 |
| **F6** | 崩塌率预测中给出的具体百分比数字来源是否粗糙、缺乏经验支撑？ | 已对该预测进行修正：不再声称固定的百分比数值，而是要求“测试组崩塌率**显著高于**对照组”（$p<0.05$），将定量点估计弱化为统计显著性判据。首达时分布的外推目前依赖 $\Delta_{VV}$ 时间序列的参数估计方法，尚无独立经验数据集完成校准，这一点如实承认为待完成工作。 | 一般让步 |

### E.6 与现有理论的关系（R1–R8）

| 编号   | 质疑陈述                                                     | 框架回应                                                     | 让步状态 |
| :--- | :------------- | :-------------------------------------- | :--- |
| **R1** | FEP 的主动推断是否已涵盖 $\mathcal{T}$ 事件？SRVD 与 FEP 的核心差异是否仅在于术语包装？ | FEP 隐含主客观同构假设；SRVD 将解码器 $D$ 独立为物理成本变量，使 $V_{\mathrm{obj}}$ 不可直接观测，只能通过 $V^{\mathrm{virt}}$ 估计。这一可主动偏离并摧毁客观存续的三分裂结构（$V_{\mathrm{obj}}$、$V^{\mathrm{virt}}$、$V^{\mathrm{val}}$）在单标量收敛框架内无对应位置，是 Myopic Runaway 成立的前提。该状态以 $T_{\mathrm{pred}}\to T_{\mathrm{min}}$ 为标志——$T_{\mathrm{pred}}$ 是受能量约束、可因耦合失稳而坍缩的状态变量，坍缩由 Jacobian 判据刻画为具体相变事件，而非计算性能退化，这在 FEP 中无对应。**拓扑维度跃迁**（$I_{\max}(D_{n+1})>I_{\max}(D_n)$）超出固定维度参数更新范围；**跨解码器不可公度命题**否定无公共基底下的跨主体比较，与 FEP 的共享生成模型路径不同。**被动相**（$E_{\mathrm{causal}}=0$，退化为 $V_{\mathrm{obj}}=V_s$）即使被 FEP 的马尔可夫毯形式体系纳入，也是退化覆盖，不产生 $E_{\mathrm{barrier}}$ 与 $E_{\mathrm{survival}}$ 的可区分动力学；SRVD 的 $V_s/V_c$ 双通道则给出被动相有实质预测内容的定量描述。四点均为结构表达能力层面的不可还原关系，严格证明待后续完成。 | 一般让步 |
| **R2** | $E_{\mathrm{survival}}$ 通道本质上就是耗散结构理论（Prigogine），新增部分是否只是符号包装？ | Prigogine的耗散结构理论主要处理近平衡态、以 $E_{\mathrm{survival}}$ 主导的区域。SRVD在此基础上的实质增量包括：(1) 引入 $E_{\mathrm{barrier}}$ 与 $E_{\mathrm{causal}}$ 两个独立能量通道，扩展了成本核算的维度；(2) 将适用范围扩展到远离平衡的相变区域（如三重分裂）；(3) 提供了跨物理基底（量子比特到文明尺度）比较的统一成本核算框架，这是耗散结构理论未曾提供的。 | 无需让步 |
| **R3** | $A=T\cdot I$（Ulanowicz上升性）已与SRVD的存续势 $V$ 的部分结构类似，SRVD是否只是加了一个分母？ | 不存在同构关系，而是概念映射。Ulanowicz的上升性 $A$ 中 $T$ 为能量通量、$I$ 为信息度量，而SRVD的 $V$ 中 $T$ 为存续时间、$I$ 为结构信息，两者含义不同，字母相同纯属巧合。存在间接关联：Ulanowicz的上升性可作为 $I_{\mathrm{struct}}$ 的域内代理指标。SRVD通过加入 $E_{\mathrm{eff}}$ 分母使跨基底比较成为可能——Ulanowicz的上升性 $A$ 与 SRVD 的 $V$ 均须遵守各自的变量口径；SRVD 的统一变量语言并不自动赋予量子比特与文明之间的数值可比性，跨域定量比较仍受正文 §2.1 的共同参照与校准条件约束。这一分母的加入是实现跨域可比性的必要结构。 | 无需让步 |
| **R4** | $I_{\mathrm{net}}$ 是否只是给Shannon信息加了一个极性标签？     | 极性标签的加入是本体论层面的改变，而非仅在数值上贴标签：Shannon的 $H(X)$ 是解码器无关、方向中性的概率量，度量的是不确定性；$I_{\mathrm{net}}$ 是解码器依赖、携带可行性极性（$I^+/I^-/I^0$）的物理拓扑实体，度量的是对特定解码器而言“可用的因果秩序”。两者的数学载体相似，但语义与适用条件不同。 | 无需让步 |
| **R5** | 复杂适应系统理论（CAS）已经描述了适应与涌现，SRVD 是否只是换了一套符号系统？ | CAS描述的是适应过程的**定性机制**；SRVD在此基础上提供的是**热力学定量约束**：将笼统的“适应度”分解为三个独立可测的物理量（$I_{\mathrm{net}},T_{\mathrm{pred}},E_{\mathrm{eff}}$），并给出 $V$ 公式作为适应度的统一标量化表达。CAS本身不预测具体的相变阈值，而SRVD给出了 $\chi_c$ 与 $I_{\mathrm{crit}}$ 这样可检验的临界值，这是超出CAS定性描述的部分。 | 无需让步 |
| **R6** | 生物域标度律借用了Wets-Brown-Enquist（WBE）代谢标度理论的数据，是否构成循环验证？ | 三域验证是**平行独立结构**，而非依次依赖的链式验证：生物域对 $\alpha$ 的估计依赖独立的代理假设 $I\sim M^{1.0\sim1.5}$，即使该代理假设被推翻，AI域与城市域的验证仍各自独立成立，不会连带失效。需要承认的是，代理映射本身的非唯一性确实削弱了每个域**内部**论证的强度（即无法排除存在其他同样合理的代理假设给出不同数值），但这一弱点不影响跨域排序方向本身的一致性结论。 | 一般让步 |
| **R7** | $V^{\mathrm{val}}$ 被劫持的机制与Goodhart定律是否只是同一现象的两种说法？ | Goodhart 定律可与 SRVD 的价值目标偏移问题建立概念联系，但现行模型尚未证明 $\chi>\chi_{\mathrm c}$ 必然导致 $V^{\mathrm{virt}}$ 指数膨胀或 $V^{\mathrm{val}}$ 被劫持。式 (I-5.12) 的临界值只属于约化 $I$–$V$ 子系统；从该子系统到完整认知系统的映射仍是开放问题。 | 无需让步 |
| **R8** | 引用广义相对论（GR）的时间膨胀效应，是否只是借用术语贴标签而无实质关联？ | 该引用的目的是作为**边界条件测试**，而非声称SRVD与GR在物理机制上等价：将Bekenstein熵代入 $I_{\mathrm{struct}}$、Hawking蒸发时间代入 $T_{\mathrm{struct}}$、$Mc^2$ 代入 $E_{\mathrm{eff}}$，检验所得的 $V$ 是否保持有限、不发散。框架同时明确承认了该测试的边界：“在黑洞奇点处，SRVD的有效适用域在此终结”，不声称框架在极端引力条件下仍然成立。 | 一般让步 |

### E.7 概念边界（C1–C6）

| 编号   | 质疑陈述                                                     | 框架回应                                                     | 让步状态   |
| :--- | :-------------- | :------------------------------------ | :---- |
| **C1** | “持久结构”（PS）概念覆盖范围从量子态一直到文明尺度，是否定义过宽而丧失区分度？ | 区分度体现在**可操作判据**而非概念范围的收窄：持久结构的身份判据（被动相三条+主动相五条）提供了严格的可操作区分标准；四类载体分层进一步为不同类型PS的 $E_{\mathrm{eff}}$ 组成权重给出了差异化设定。概念覆盖范围广是框架有意为之的设计特征，用以支持跨尺度比较，而非定义不严谨的表现。 | 无需让步   |
| **C2** | 将 $\pi$、群论这类抽象数学对象也纳入PS范畴，是否混淆了抽象对象与物理实体？ | 变量定义部分已明确区分：形式-数学类PS**没有独立的物理载体**，其“持久性”完全依赖于宿主系统（如计算设备、人类认知系统）的持续维护。此处的 $E_{\mathrm{causal}}$ 指的是**宿主**在调用该数学结构时所消耗的能量，而非声称数学对象自身具有能量或物理实体性，因此不构成混淆。 | 无需让步   |
| **C3** | 模因、虚拟类PS的“持久性”依赖于宿主群体的共识维持，这与物理PS的持久机制是否本质不同？ | 确实不同——这正是载体分层设计的意义所在。各类结构都受能量预算与热力学约束，但不能统一写成 $E_{\mathrm{maint}}\geq E_{\mathrm{Landauer}}+E_{\mathrm{structure}}$：Landauer 下界只适用于满足条件的逻辑不可逆擦除，不能充当一般维持成本的普适下界。不同类型的 $E_{\mathrm{eff}}$ 分项及其权重须分别声明：例如货币的持久性需要足够多的宿主持续消耗 $E_{\mathrm{causal}}$（认知与社会协调成本）来维持共识，这与细胞依赖 $E_{\mathrm{survival}}$ 维持代谢是同构的约束结构，只是能量通道的相对权重不同。模因类PS本身作为 $I_{\mathrm{latent}}$ 存在于宿主可达但未激活的状态空间中，经宿主认知解码器 $D$ 提取为 $I_{\mathrm{net}}$——这是宿主与模因之间普通的解码关系，走的是信息通道而非能量通道，不涉及 $V^{\mathrm{val}}$ 锚定转移或自我评估层面的优化。 | 无需让步   |
| **C4** | 将“爱”“恨”“复仇”等情感现象映射为 $V^{\mathrm{val}}$ 的锚定转移，是否属于过度拟人化的类比？ | 框架的实际声称是“在SRVD的动力学语言中，爱这一行为模式*可以被描述为* $V^{\mathrm{val}}$ 向另一个PS的 $V_{\mathrm{obj}}$ 发生锚定转移”，这是一种**描述性映射**，而非“爱本质上就是锚定转移”这样的还原论声称。该映射目前缺乏独立的神经科学实证数据支撑，属概念类比而非已验证的因果机制，证据等级低于本卷其余形式化结论。 | 实质性让步 |
| **C5** | 将货币、法律、战争等社会现象解释为热力学能量转换过程，是否是一种粗糙的物理主义还原论？ | 社会尺度映射部分已明确说明：具体的社会转换过程遵循社会契约与法律框架本身的逻辑，**不是**SRVD公式内部的代数替换或直接推导。SRVD在此提供的是一种**本体论层面的共同基础**——社会结构同样依赖载体、能量与可识别的信息组织——而不主张 $I_{\mathrm{net}}$ 与 $I_{\mathrm{struct}}$ 具有已证明的同一语义尺度，也不声称社会现象可以被还原为纯物理方程求解。但这一区分在部分章节的行文中确实存在表述上容易引发还原论误读的地方，措辞上仍有改进空间。 | 一般让步   |
| **C6** | 所有PS都被定义为“有限”的，却又使用“持久”一词描述，是否自相矛盾？ | 开篇定义注释已澄清：“有限”在框架中意为“非无限”，不意为“短促”：花岗岩可以存续十亿年之久，仍然属于“有限时间”范畴。“持久”一词指的是“在给定能量约束下，拓扑特征在一段时间内保持可辨识”，这一定义与“有限”并不矛盾，二者描述的是时间尺度的不同维度（有界性 vs. 相对长度）。 | 无需让步   |

### E.8 工程应用（E1–E4）

| 编号   | 质疑陈述                                                     | 框架回应                                                     | 让步状态 |
| :--- | :----------------- | :------------------------------- | :---- |
| **E1** | SRVD 对RLHF（基于人类反馈的强化学习）的批评停留在概念层面，具体可操作的算法改进方案在哪里？ | 对齐工程应用部分提出了三个可操作方向：(1) 用行为代理指标估计 $\Delta_{VV}$；(2) 将RLHF奖励模型显式建模为 $V^{\mathrm{val}}$ 的载体，检测权重 $w_s,w_c$ 随训练进程的时间演化；(3) 在奖励函数设计中引入耦合惩罚项以抑制 $\chi\to\chi_c$ 的趋势。三个方向均可在现有RLHF工程框架内实施，但需要承认目前均停留在**研究提案**阶段，尚无已发表的实现或消融实验验证其有效性。 | 一般让步 |
| **E2** | SRVD 应用于文明治理层面的分析是否流于宏观隐喻，缺乏可操作性？ | 对人类发展指数（HDI）的重读提供了具体可操作的政策诊断框架；锁定状态诊断表为组织管理提供了 $E/I/T/D$ 四维诊断工具。但从“诊断”到“具体政策方案”之间仍存在较大距离——框架目前能够指出一个社会系统在哪些维度上偏离健康区间，但尚未提供从诊断结果到具体干预措施的映射规则，这是应用层面尚待发展的部分。 | 一般让步 |
| **E3** | 智慧杠杆 $L=\Delta V/E_{\mathrm{build}}$ 在实践中应当如何具体计算？ | $L$ 的主要设计用途是**同域内的策略间相对比较**，而非跨域的绝对数值计算。若 $E_{\mathrm{build}}$ 已知，且 $\Delta V$ 用同一领域的代理指标度量，该比值可以被估算并用于比较不同策略的相对效率。$L$ 的绝对值计算在跨领域场景下目前不可行，这一局限性在框架中已如实说明，未被夸大为普适可计算量。 | 一般让步 |
| **E4** | 技术停滞阈值 $E_{\mathrm{build}}>\dot F_{\mathrm{avail}}\cdot T_{\mathrm{avail}}$ 应当如何实际测量？ | 在特定技术领域内，$E_{\mathrm{build}}$ 可用该领域的研发总投资作为代理指标，$\dot F_{\mathrm{avail}}$ 可用该领域可调配的资源流速率作为代理指标，二者均具备可操作性。跨领域的绝对值比较则受制于不同领域间成本单位不可通约的约束，目前只能在同一领域内部进行比较，跨领域比较仍是开放问题。 | 一般让步 |

### E.9 叙事风格（N1）

| 编号   | 质疑陈述                                   | 框架回应                                                     | 让步状态 |
| :---- | :------------- | :--------------------------------- | :----- |
| **N1** | 开篇的寓言故事是否会削弱理论的学术严肃性？ | 这是一种有意采用的“直觉前置”写作策略：故事中的每一个情节都对应一个核心变量的具象化定义，其作用是降低跨学科读者的入门门槛，而非纯粹的文学装饰。在跨学科专著这一文体传统中，用叙事桥接抽象概念是常见且合理的修辞选择，不影响后续正文的形式化严谨性。 | 一般让步 |

### E.10 让步等级汇总与后续工作路线图

| 让步等级   | 含义                                                     | 涉及编号                                                     | 数量 |
| :------- | :------------------- | :------------------------- | :----- |
| 无需让步   | 框架内部回应充分，质疑源于对定义/协议的误读              | P2, P4, D1, D4, K1, K4, F4, R2, R3, R4, R5, R7, C1, C2, C3, C6 | 16   |
| 一般让步   | 回应方向正确，但存在需要后续补充的具体工作或已知适用边界 | M1, M4, M6, P1, P3, D2, D3, D5, K2, K3, K5, F1, F2, F3, F5, F6, R1, R6, R8, C5, E1, E2, E3, E4, N1 | 25   |
| 实质性让步 | 框架当前版本确实无法充分回应，构成核心开放问题           | M2, M3, M5, C4                                               | 4    |

**总计：45条质疑与回应**，覆盖数学形式化、物理可测量性、变量定义、动力学机制、可证伪性、与既有理论关系、概念边界、工程应用、叙事风格八个方面。

**四条实质性让步——即框架当前版本尚无法充分回应、构成核心开放问题的部分——集中在：**

1. **五重递归架构的严格连续化**（M2）：完全双向耦合的ODE/PDE系统尚未建立，当前仅有脱钩偏差这一简化子系统的严格闭式解。
2. **弹性指数排序 $\alpha>\gamma>\beta$ 的第一性原理推导**（M3）：定性方向已由热力学论证，但不依赖代理假设的严格数值推导缺失。
3. **耦合强度 $\chi$ 的微观基础**（M5）：作为现象学参数使用是合理的建模选择，但缺乏从更基础机制出发的第一性推导。
4. **情感基质映射的实证支撑**（C4）：$V^{\mathrm{val}}$ 锚定转移作为爱、恨等情感现象的动力学描述，目前缺乏独立神经科学证据，是描述性类比而非已验证机制。

这四项是早期评审阶段登记的实质性让步。其当前状态须结合正文第十章重新判断；本附录不替代现行版本的局限清单，也不把历史让步数量当作理论完成度指标。

***

## 附录 F　仿真底稿：设置、参数与结果

**这一附录是什么。** 本卷正文里有若干读数只能由数值实验给出——判据本身是可写的，但“照它做会得到什么”要跑。本附录把这些读数的模型设置、参数与结果表集中给出，正文只保留论证必需的几个数字并标明出处。

**这一附录不是什么。** 它**不是**对本卷动力学的经验验证。全部算例在合成模型里跑，参数由作者选定；通过这些检验只说明“判据在自己的模型族内可以执行”，不说明“真实系统就是这样”。凡属算例值的地方都注明了“模型族内的算例值、不是经验值”。

**两批来源。** 表 F-1 至 F-4 来自仿真批次 A（14 项判定：9 通过、4 失败、1 不可判），其结论已落为 E-1—E-7。表 F-5 至 F-7 来自仿真批次 B 的 M7 模块（4 项判定：3 通过、1 失败），其结论已落为 B4、C2 与数值分层。

### F.1　统一设置

| 项 | 值 |
| :-------------------- | :-------------------------------------- |
| 解释器与库 | Python 3.13.13／numpy 2.5.4／scipy 1.18.1／matplotlib 3.11.2 |
| 主随机种子 | `20261103`；各模块各自固定种子，写在脚本里 |
| 数据性质 | 合成模型，无实测数据 |
| 预注册 | 两批仿真各有判定协议，判据运行前固定 |
| 复现命令 | 见本附录 F.11 |

### F.2　表 F-1　约化等价的漂移阈值（§5.2，对应 E-1）

设置：$\zeta_V=2\ \mathrm{s/J}$、$\mu_{\mathcal F}=1.3\ \mathrm{s^{-1}}$、$\tau_{\mathrm{decay}}=1\ \mathrm{s}$、$I_{\max}=5\ \mathrm{bit}$、$I_{\mathrm{eq}}=0$；按 $r_{\mathrm v}=\mu_{\mathcal F}$、$\gamma_0=\tau_{\mathrm{decay}}^{-1}$，得 $V_{\max}=\zeta_V I_{\max}(1-\gamma_0/r_{\mathrm v})=2.3077\ \mathrm{bit\cdot s/J}$，积分 40 个时间单位。

| 漂移情形 | 实测 10% 偏差对应的 $\varepsilon_{\mathrm{rel}}^{*}$ | 原文本阈值 |
| :------------------ | ---------------------: | ------------------: |
| $\dot T_c/T_c$ 与 $\dot E_c/E_c$ **反号** | **0.0220** | $\approx1$ |
| 同号同量级 | 不存在（偏差恒为 0） | $\approx1$ |

**两条读数：**

1. 反号时，原阈值 1 允许的偏差是 $e^{gW}-1=75.2$ 倍（$gW=4.33$）——判据形同虚设。解析式 $\varepsilon_{\mathrm{rel}}^{*}=\ln(1+\delta)/(gW)$ 与实测差 **0.2%**。
2. 同号时，$V_c\propto I_cT_c/E_c$ 只依赖**差** $\dot T_c/T_c-\dot E_c/E_c$，偏差恒为零；而原判据取**绝对值和**，会在此情形报“失效”，把可用的约化误判为失效。成因：$V_c$ 依赖的是比，不是和。

另：两式轨道的最大相对偏差 $5.3\times10^{-12}$，即“两式在该窗内给出同一条轨迹”在数值上成立；若 $V_{\max}$ 漏掉 $(1-\gamma_0/r_{\mathrm v})$ 因子，偏差立刻升到 $O(1)$。

![图 F.1　约化等价的漂移阈值](figures/release/fig_m2_epsrel.pdf)

**图 F.1　约化等价的漂移阈值。** 纵轴为相对轨迹偏差 $|\Delta V|/V$，横轴为 $\varepsilon_{\mathrm{rel}}$。反号漂移（实线）在 $\varepsilon_{\mathrm{rel}}^{*}=0.022$ 处越过 10% 容差（灰点线）；同号漂移（虚线）一阶上精确抵消，全程贴着 $10^{-12}$ 的下限。红色竖线是原文本阈值 $\varepsilon_{\mathrm{rel}}\approx1$——落在它右边的偏差已达 $e^{gW}-1=75.2$ 倍，判据在那里形同虚设。

### F.3　表 F-2　链条第 (1) 步的弹性（§5.3，对应 E-3）

设置：式 (I-5.12) 的 $I$–$V$ 子系统，$\alpha_{\mathrm{eff}}=1.5$、$\kappa=1$，扫 $\chi\in[10^{-1.5},10^{2.5}]$。

**平衡偏差对 $\chi$ 的尾部弹性**：解析 $-2/(2-\alpha_{\mathrm{eff}})=-4.00$，实测 $-3.99999999$（$R^2=0.99999999999$）。$\chi$ 从 0.032 升到 208，$\Delta^{*}_{\mathrm{VV}}$ 从 0.97 单调降到 $5.3\times10^{-10}$，双对数斜率恒为 $-4$。

**方向与 (I-5.17) 第 (1) 步相反**：自指耦合越强，平衡脱钩偏差越小，而不是放大。

**补救所需的最小形式**（表 F-2b）：令源项内生，按 (I-5.16a) 取 $\sigma=\sigma_0\left[1+(\chi V/\chi_{*})^{m}\right]$（与下表用的 $\sigma=\sigma_0+a(\chi V)^{m}$ 等价，$a=\sigma_0\chi_{*}^{-m}$，$\chi_{*}=1$ 时 $a=\sigma_0$），则

$$\frac{\mathrm d\ln\Delta^{*}}{\mathrm d\ln\chi}=\frac{2m}{2-\alpha_{\mathrm{eff}}}-\frac{2}{2-\alpha_{\mathrm{eff}}}=\frac{2}{2-\alpha_{\mathrm{eff}}}(m-1)$$

转正点 $m^{*}=1$，**与 $\alpha_{\mathrm{eff}}$ 无关**；数值扫描给出 $m^{*}=1.000$，斜率恰为 $4(m-1)$。这一档只验了 $\alpha_{\mathrm{eff}}=1.5$，四档同时成立的情形见 §F.10 表 F-9。若把驱动力误写成 $\chi$（丢掉自洽放大 $V$），则不存在转正点。

两个区制与四档 $\alpha_{\mathrm{eff}}$ 的合并结果见 §F.10 图 F.4。

### F.4　表 F-3　门控规则的判别力（§8.3，对应 E-2）

被检对象是**规则**，不是 H7 的理论内容。零模型：健康系统的 $\gamma_t=\gamma_0(1+\eta_t)$，$\eta$ 为 AR(1)，$\rho=0.8$。

| 噪声 $\sigma_\eta$ | 0.01 | 0.02 | 0.05 | 0.1 | 0.2 | 0.5 |
| :------------- | ------: | ------: | ------: | -------: | -------: | -------: |
| 规则 1（3 回合降 30%）FPR | 0 | 0 | 0 | 0.036 | **0.676** | **0.988** |
| 规则 2（MK 扫描 $n_{\mathrm{win}}=10$）FPR | 1.0 | 1.0 | 1.0 | 1.0 | 1.0 | 1.0 |

规则 2 的 100% 由两个独立原因叠加，分开测：

| 条件 | $n_{\mathrm{win}}=5$ | 10 | 20 | 40 |
| :------------- | ----------: | ----------: | ----------: | ----------: |
| 单窗、$\rho=0$（iid） | — | 0.021 | 0.020 | 0.019 |
| 单窗、$\rho=0.8$ | — | **0.173** | **0.223** | **0.241** |
| 全序列扫描、$\rho=0.8$ | 0.832 | **1.000** | **1.000** | 0.996 |

- **自相关**：MK 的方差公式假定独立；$\rho=0.8$ 使名义 5% 变成 17%—24%。
- **多重检验**：200 步按 5 步滑窗扫 35 次，每次 5%，族错误率约 $1-0.95^{35}=83\%$。

**后果**：H7 的反驳条件是“系统崩溃但事前未检出下降”。当“检出”的假阳性率是 100% 时，反驳条件几乎不可能成立，H7 因此不是可证伪预测，而是恒真陈述。修正见 §8.3 与篇末 H7 条。

![图 F.2　门控规则的判别力（假阳性率）](figures/release/fig_m5_fpr.pdf)

**图 F.2　门控规则的判别力（假阳性率）。** 被检对象是**规则**，不是 H7 的理论内容。规则 1（3 回合降 30%）在 $\sigma_\eta\le0.1$ 时 FPR 近零，$\sigma_\eta=0.2$ 起崩坏（0.676），0.5 时 0.988；规则 2（MK 滑窗扫描）全程 **1.0**——自相关把名义 5% 抬到 17%—24%，多重检验再把族错误率推到 83%，两个原因叠加。红色点线为名义 5%。

### F.5　表 F-4　稀有度读数的分辨率（§2.1，对应 E-4）

真实背景 $K=50$、Zipf($s=1$)，每格 500 次重抽：

| $N$ | 未被观测到的类别占比 | 最稀 10% 类别的中位偏差 | 最大可报读数（bit） | $\log_2N$ |
| -------: | -------------: | --------------: | -------------: | --------: |
| $10^2$ | 36.5% | −1.14 | 6.64 | 6.64 |
| $10^3$ | 0.2% | +0.15 | 9.26 | 9.97 |
| $10^4$ | 0 | +0.009 | 8.07 | 13.29 |
| $10^5$ | 0 | −0.002 | 7.85 | 16.61 |

**读法**：采样量 $N$ 增大后，最大可报读数**不再上升**（9.26 → 8.07 → 7.85），而 $\log_2N$ 继续线性增长——估计量的上限由背景的**实际支撑**决定，不由样本量决定。

![图 F.3　稀有度读数的分辨率](figures/release/fig_m6_rarity.pdf)

**图 F.3　稀有度读数的分辨率。** 真实背景 $K=50$、Zipf($s=1$)。橙色虚线是最大可报读数：$N$ 从 $10^3$ 增到 $10^5$，它不升反降（9.26 → 8.07 → 7.85），而灰色点线的 $\log_2N$ 继续线性增长。蓝色是采样量不足时最稀十分位的中位偏差（$N=10^2$ 时 $-1.14$ bit，$N\ge10^3$ 后收敛到 0）。虚线门控 9.97 bit 对应预注册参数 $\alpha_0=10^{-3}$ 的 $-\log_2\alpha_0$。上限由背景的实际支撑决定，不由样本量决定。

### F.6　表 F-5　终局相图与三情形的一致性（§5.1.2）

| 项 | 实测 | 判定 |
| :-------------------- | :----------------------------- | :------: |
| 数值终局与解析三情形的一致率 | **1.0000**（600 个抽样格点；81 个落“未定”未计入，$g_0=\delta$ 邻域除外） | 通过 |
| $V^{*}$ 的数值相对误差 | $1.53\times10^{-7}$ | 通过 |

**这不是验证**：一致率高只说明“解析式与数值积分在同一个模型里彼此相容”，两者若有共同的建模错误，这个检验看不出来。

### F.7　表 F-6　移动目标的漂移阈值（§5.1.2，对应 B4）

| 项 | 实测 | 预注册 | 判定 |
| :-------------- | :------------ | :------------ | :-----------------: |
| 临界漂移 $\varepsilon^{*}/g_0$ | **0.0077** | $[0.05,0.5]$ | **失败（预测错）** |

**含义**：“分段近似”的适用条件比预想的苛刻得多：驱动率的漂移只要达到净增长率的 **0.8%**（每单位时间），冻结不动点对轨迹的预测偏差就超过 10%。原因是带伤平衡附近 $\partial V^{*}/\partial g_0=\delta_{\mathrm{dam}}/g_0^{2}$ 很大，$V^{*}$ 对 $g_0$ 极敏感。所以“把参数当常数、用不动点外推”在长窗口里几乎总是错的，**除非漂移率小于 $10^{-2}g_0$ 量级**。

### F.8　表 F-7　双稳盆地的测度（§5.2.3，对应 C2）

| 项 | 实测 | 判定 |
| :----------------------------- | :--------------- | :------------: |
| $\chi=0.9\chi_{\mathrm c}$、$\alpha_{\mathrm{eff}}=3$ 时发散初值占比 | **29.3%** | 通过 |

**含义**：$\chi$ 已低于 $\chi_{\mathrm c}$，仍近三成初值发散——“不能把 $\chi<\chi_{\mathrm c}$ 一律当作路径一”这句警告确有实质内容，不是防御性措辞。

### F.9　表 F-8　未预注册的观察：包络论证（**不进判定**）

竞争耗散模块的预注册判定是“**不可判**”：12 格 × 20 种子里 11 格无人死亡，比较退化为 150 对 150，检验力不足。下面这条是**事后观察，未预注册**，只作量级参考，不作证据。

设置：$I_0=0.5$、$R=1$，8 次重复平均。主体在对称内部均衡处满足 $\partial V/\partial e=0$，故单边削减努力对 $V$ 的损失是**二阶**的，而释放的能量预算是**一阶**的：

| 削减比例 | 0 | 10% | 20% | 50% | 80% |
| :--------- | ---------: | ---------: | ---------: | ---------: | ---------: |
| $V$ | 0.521212 | 0.521193 | 0.520833 | 0.517304 | 0.509031 |
| $\Delta V/V$ | 0 | $-4\times10^{-5}$ | $-7.3\times10^{-4}$ | $-7.5\times10^{-3}$ | $-2.3\times10^{-2}$ |

**读法**：削减 50% 努力，$V$ 只降 0.75%；削减 80%，降 2.3%（拟合阶数 2.42，受网格离散限制，量级为 2）。而释放的能量预算是 50% 与 80%。

**为什么这条不能当证据**：它是事后挑的观察，没有预注册，也没有对照组设定；“二阶 vs 一阶”的结论依赖均衡点假设成立。它的用处只有一个——说明 §8.4 那条预测在本模型族里**检验力很弱**，判别力主要来自公共池设定。


### F.10　表 F-9　四档 $\alpha_{\mathrm{eff}}$ 下的弹性斜率（§5.3、§5.4，对应 (I-5.16b)）

设置：式 (I-5.12) 的 $I$–$V$ 子系统，$\kappa=1$、$I_{\mathrm{bas}}=1$、$\chi_{*}=1$、$\sigma_0=1$、$\alpha_{\mathrm L}=1$；$\alpha_{\mathrm{eff}}\in\{0.5,1.0,1.5,1.9\}$，$m\in\{0.5,0.8,1.0,1.2,1.5,2.0,2.5\}$，共 28 格。脚本 m8_elasticity.py，结果 results_m8_elasticity.json。

**两处与批次 A 的 M3 不同**（不是改公式，是改求解）：平衡点在对数空间求根——线性括号在 $\alpha_{\mathrm{eff}}=1.9$、$\chi>10$ 时溢出并返回 NaN；$\chi$ 网格按 $\alpha_{\mathrm{eff}}$ 自适应拉长，使 $V^{*}\le10^{12}$ 且两个渐近区（$\chi V^{*}\gg1$ 与 $(\chi V^{*}/\chi_{*})^{m}\gg1$）都落在拟合窗内。网格太短不是公式错：那样拟合到的是过渡段，不是尾部。

| $m$ | 0.5 | 0.8 | 1 | 1.2 | 1.5 | 2 | 2.5 |
| :----- | -------: | -------: | ------: | ------: | -------: | -------: | -------: |
| $\alpha_{\mathrm{eff}}=0.5$ | -0.6667 | -0.2667 | 0.0000 | 0.2667 | 0.6667 | 1.3333 | 2.0000 |
| $\alpha_{\mathrm{eff}}=1.0$ | -1.0000 | -0.4000 | 0.0000 | 0.4000 | 1.0000 | 2.0000 | 3.0000 |
| $\alpha_{\mathrm{eff}}=1.5$ | -2.0000 | -0.8000 | 0.0000 | 0.8000 | 2.0000 | 4.0000 | 6.0000 |
| $\alpha_{\mathrm{eff}}=1.9$ | -10.0001 | -4.0000 | 0.0000 | 4.0000 | 10.0000 | 20.0000 | 30.0000 |

上表为**拟合值**（双对数尾部最小二乘，$R^{2}\ge0.9999999$）。解析值为 $\dfrac{2(m-1)}{2-\alpha_{\mathrm{eff}}}$，逐格相对误差最大 **$6.3\times10^{-6}$**（判据 $2\%$），28/28 通过。

**转正点。** 四档 $\alpha_{\mathrm{eff}}$ 各做一次求根，得 $m^{*}=1.0000000$（四档同值，差别在小数第 11 位），与 (I-5.16b) 的「过零点恒在 $m=1$、与 $\alpha_{\mathrm{eff}}$ 无关」一致。

**外生对照。** 令 $\sigma\equiv\sigma_0$（源项不启动），四档拟合斜率分别为 $-1.3333$、$-2.0000$、$-4.0000$、$-20.0000$，与 $-2/(2-\alpha_{\mathrm{eff}})$ 逐档相符——其中 $-4.0000$ 即表 F-2 的 $-3.99999999$。

**破坏检验。** 把解析式故意写错（丢掉分母的贡献，即用 $2m/(2-\alpha_{\mathrm{eff}})$ 当预测），同一套拟合在 28 格里 **0 格**通过 $2\%$ 判据。这说明上面的「通过」不是判据太松。

![图 F.4　弹性的两个区制与 $\alpha_{\mathrm{eff}}$ 无关的过零点](figures/release/fig_m8_regimes.pdf)

**图 F.4　弹性的两个区制与 $\alpha_{\mathrm{eff}}$ 无关的过零点。** 左：$\alpha_{\mathrm{eff}}=1.5$、$m=1.5$、$\chi_{*}=10^{3}$ 时 $\Delta^{*}_{\mathrm{VV}}$ 随 $\chi$ 的走向——源项未启动时平（$\sigma$ 与 $I_{\mathrm{net}}$ 同时不随 $\chi$ 变），进入自指区后以斜率 $-4$ 下降，越过 $u_{\min}$ 后以斜率 $+2$ 上升。$\chi_{*}$ 取 $10^{3}$ 只是为把两个区制同时放进图幅（尾部斜率与 $\chi_{*}$ 无关，扫描本身用 $\chi_{*}=1$）。右：表 F-9 的 28 格，四条线全在 $m=1$ 过零，斜率随 $m$ 线性，比例因子 $2/(2-\alpha_{\mathrm{eff}})$ 由 $\alpha_{\mathrm{eff}}$ 决定。

### F.11　图目录与复现

本卷四张附录图均由原始脚本与结果文件同源重绘，分别置于 §F.2、§F.4、§F.5、§F.10；每张图随文提供同名 `.svg`（可编辑）、`.pdf`（矢量）与 `.png`（300 dpi），正文引 `.pdf`。图 F.4 合并呈现 §F.3 与 §F.10 的弹性结果；表 F-8 的包络图仅保留在复现包 `batch_A/figure/fig_m4_envelope.png`，不插入正文。§5.1.2 的正文图 Ⅰ-8 出自仿真批次 B。

| 图号 | 文件（三格式同名） | 对应 | 位置 |
| :---------: | :------------------ | :----------------: | :----------- |
| 图 F.1 | `fig_m2_epsrel` | 表 F-1 | §F.2 末 |
| 图 F.2 | `fig_m5_fpr` | 表 F-3 | §F.4 末 |
| 图 F.3 | `fig_m6_rarity` | 表 F-4 | §F.5 末 |
| 图 F.4 | `fig_m8_regimes` | 表 F-2、表 F-9 | §F.10 末 |

**复现**：以下路径相对随稿复现包根目录 \path{reproducibility/}。

```bash
(cd batch_A/sim && python run_all.py)           # 批次 A，约 75 秒
(cd batch_B/sim && python run_all.py)           # 批次 B，约 3 分钟
(cd m8_v1.60/sim && python m8_elasticity.py)    # M8 弹性闭式扫描
```

两套都是单机 CPU、纯 numpy/scipy，无 GPU、无外部数据。

***

## 附录 G　算术核验表

**为什么有这一张表。** 全书 250 个带号公式由人工转录，上下标抄错不会有任何自动报警。附录 F 给的是“仿真跑出来的数”，本附录补的是另一半：**闭式本身代进去算不算得对**。每一行都能在几分钟内复现；改公式时，这张表就是“哪几个数要跟着变”的清单。本附录分两张表：**G.1 核闭式**（8 行），**G.2 核正文报的数**（24 行，把数追回它的脚本与字段）。两者的失败模式不同——公式抄错会让整节结论失真，数字抄错只影响一句，但改脚本后没人记得回来改正文。

**【引用约定】** 本表“来源”列中的「RIF §…」「RIF 表 C-…」指**同包另册**《相对信息论（RIF）》的节号与该册附录 C 的表号，该册的原始读数不在本卷重印。单卷阅读时，G-9—G-13、G-23—G-28 按本行约定解析；其余各行均可在本卷内独立复算。

**方法。** 每条公式配一个可执行的对照：闭式对数值求根、数值积分或数值微分。每条对照另有一个**破坏版**——把公式改成故意写错的形式（换分支、换阈值、漏掉特解、把协方差的对象换掉）。若破坏版仍然判“通过”，说明该对照没有判别力，不计入表内。破坏检验结果：**10 项中 10 项被检出**（含表外的 (I-5.2) 轨迹等价与内生源项指数两项）。

**设置。** 脚本 `batch_A/sim/m1_math.py`，结果在 \path{batch_A/results/results_all.json} 的 `M1`／`M0` 段；M8 结果在 \path{m8_v1.60/sim/results_m8_elasticity.json}。以上脚本与结果均收入随稿复现包 `reproducibility/`。

已发布于 Zenodo，DOI：10.5281/zenodo.24349831。主种子 `20261103`，各条按 `SEED+offset` 派生子种子；数值积分用 `solve_ivp`（rtol $10^{-11}$—$10^{-12}$）。跨包数值核验入口：`python tools/verify_numbers.py`。

### G.1　表 G-1　闭式核验

| 编号 | 公式 | 检验方法 | 复现值与偏差 | 参数范围 | 种子 |
| :--: | :-------- | :--------------- | :------------- | :-------- | :------- |
| G-1 | (I-5.1c) | 闭式正根对 `brentq` 求根，200 组 | 最大相对偏差 $1.6\times10^{-10}$（阈值 $10^{-9}$） | $\mu\in[0.2,10]$、$I_{\max}\in[0.5,100]$、$\tau\in[0.05,20]$、$I_{\mathrm{eq}}\in[10^{-4},1]$，对数均匀 | 20261104 |
| G-2 | (I-5.1d) | 400 组：判据 $\mu\tau>1$ 与“是否存在正内点”逐组比对，并解跨临界点 | 不一致 **0** 组；临界点定位误差 0（解析 $\mu^{*}=1/\tau$） | $\mu\in[0.2,10]$、$\tau\in[0.05,20]$ | 20261105 |
| G-3 | (I-5.13) | 闭式 $\chi_{\mathrm c}$ 对联立 $(h,h')=0$ 的 `fsolve` 解，60 组 | 最大相对偏差 $2.9\times10^{-10}$（阈值 $10^{-6}$），60/60 收敛 | $\alpha_{\mathrm{eff}}\in[2.2,5]$、$\kappa\in[0.05,20]$ | 20261106 |
| G-4 | (I-5.15) | 闭式对 `solve_ivp`（4001 点，rtol $10^{-12}$） | 最大绝对偏差 $1.0\times10^{-12}$；$\Delta^{*}=0.190476=4/21$ | $\alpha_{\mathrm L}=0.7$、$I=3$、$\sigma=0.4$、$\Delta_0=5$，$t\in[0,10]$ | 无（确定性） |
| G-5 | (I-5.3) 三分情形 | 28 格（$4$ 个 $g_0$ × $6$ 个 $\delta/g_0$，另加 4 个 $g_0<0$ 格）：分类判据对轨迹终值 | **28/28** 分类正确（比率 1.00，阈值 0.99） | $g_0\in\{0.05,\allowbreak 0.1,\allowbreak 0.2,\allowbreak 0.4\}$、$\delta/g_0\in\{0.2,\allowbreak 0.5,\allowbreak 0.8,\allowbreak 1,\allowbreak 1.2,\allowbreak 1.5\}$；$g_0=-0.1,-0.4$ | 无（确定性） |
| G-6 | (I-5.3) 临界格 | 临界格 $g_0=\delta=0.2$：$1/V$ 对 $t$ 线性回归 | $R^{2}=1.000000$，斜率偏差 $1.8\times10^{-13}$ | $V_0=0.9$，$t\in[0.5,40]$，2000 点 | 无（确定性） |
| G-7 | (I-3.11) | Price 协方差：有限差分 $\mathrm d\langle V\rangle/\mathrm dt$ 对加权协方差 | $2.2395954129$ 对 $2.2395954126$，相对偏差 $1.4\times10^{-10}$ | $N=40$、$V\in[0.2,3]$、$r=\exp(0.9V)$、$x\sim\mathrm{Dirichlet}(\mathbf 1)$ | 20261110 |
| G-8 | (I-3.2) | 单通道 $V=IT/E$ 与双通道之和的比值（§3.2 的“4 倍”） | $4.000$——**构造精确值，不是误差** | 两通道取同参 | 无（确定性） |

**三条读法。**（i）“偏差”是闭式与数值之差，不是公式与真值之差：数值侧也有误差，二者同量级时只说明二者一致到该量级，不说明公式更准。（ii）G-5 的复现值是**分类率**、G-8 是**构造值**，都不能按 $10^{-10}$ 的标准读；把不同量纲的“偏差”排在一列是本表的排版折中，不是口径统一。（iii）这张表覆盖 8 个带号公式，占 250 个的 3%：其余 242 个是“已转录、未核验”。它的用处是给下一版一个可增行的位置——每改一个公式，就在此表加一行，否则不改。正文里报的**数**另由表 G-2 追源（24 条）；两张表的分母不同（250 个公式号 / 24 处数值），不能相加，也不能相除。

### G.2　表 G-2　正文数值断言的溯源核验

上一张表核的是**闭式**（把公式代进去算），这张表核的是**正文报的数**（把数追回它的脚本与字段）。两者的失败模式不同：闭式抄错会让整节结论失真，数字抄错只影响一句，但最容易被直接核对。

列义：**正文值**是被核的那句话里的数；**复现值**是当场重算或从结果文件读出的数；**来源**是这条数唯一可追的落点。P 类不依赖任何结果文件，S 类依赖两批仿真各自的结果 JSON。

| 编号 | 类 | 落点 | 正文值 | 复现值 | 来源 |
| :---: | :--: | :---------- | ------: | -------------: | :------------------ |
| G-9 | P | RIF §12.2 / C.2 | 0.0563 | 0.0563485 | `verify_numbers.py` 内重算 |
| G-10 | P | RIF §12.2 / C.2 | 0.528 | 0.528174 | `verify_numbers.py` 内重算 |
| G-11 | P | RIF §12.2 / C.2(c) | 0.890 | 0.889518 | `verify_numbers.py` 内重算 |
| G-12 | P | RIF 表 C-1(c) | 1.318 | 1.31777 | `verify_numbers.py` 内重算 |
| G-13 | P | RIF §12.2 | 0.11 | 0.110482 | `verify_numbers.py` 内重算 |
| G-14 | P | 卷Ⅰ 卷Ⅰ (I-5.15) | 0.190476 | 0.190476 | `verify_numbers.py` 内重算 |
| G-15 | P | 卷Ⅰ 表 F-3 注 | 0.83 | 0.833917 | `verify_numbers.py` 内重算 |
| G-16 | S | 卷Ⅰ 表 F-7 | 0.293 | 0.292716 | `M7_dynamics.json` results.P4.detail.div_frac |
| G-17 | S | 卷Ⅰ 表 F-8 | 0.0075 | 0.00749778 | `results_all.json` M4.envelope.rel[3] |
| G-18 | S | 卷Ⅰ 表 F-8 | 0.023 | 0.0233704 | `results_all.json` M4.envelope.rel[4] |
| G-19 | S | 卷Ⅰ 表 F-8 | 2.42 | 2.41884 | `results_all.json` M4.envelope.exponent |
| G-20 | S | 卷Ⅰ 表 F-2 | $-4.00$ | $-4.0000$ | `results_all.json` M3.C1.slope_inf |
| G-21 | S | 卷Ⅰ 表 F-1 | 75.2 | 75.1979 | `results_all.json` M2.B2.dev_at_eps1 |
| G-22 | S | 卷Ⅰ 表 F-1 | 0.0220 | 0.0220475 | `results_all.json` M2.B2.eps_star_opp |
| G-23 | S | RIF §13 / 表 C-5 | 0.394 | 0.393744 | `M5_bias.json` results.D1.detail.auc_G |
| G-24 | S | RIF §13 / 表 C-5 | 0.880 | 0.880409 | `M5_bias.json` results.D1.detail.auc_A |
| G-25 | S | RIF 附录 C 表 C-6 | 1.29 | 1.29121 | `M6_depth.json` results.K7.detail.b |
| G-26 | S | RIF 表 C-3 | 0.720 | 0.719546 | `M3_resolution.json` \path{results.R1.detail[0].kendall_gain_med} |
| G-27 | S | RIF 表 C-2 | 1.00 | $1.00$ | `M2_boundary.json` \path{results.B7.detail.pairing_ok_all_frac} |
| G-28 | S | RIF 表 C-3 | 1.26—1.35 | 1.2556—1.3466 | `M3_resolution.json` \path{results.R1.detail[*].nonadditivity_med} |
| G-29 | S | 卷Ⅰ 表 F-9 | $6.3\times10^{-6}$ | $6.288\times10^{-6}$ | `results_m8_elasticity.json` summary.max_rel_err |
| G-30 | S | 卷Ⅰ 表 F-9 | 1.0000000 | 1.0000000 | `results_m8_elasticity.json` m_star.* |
| G-31 | S | 卷Ⅰ 表 F-9 外生 | $-1.3333/-2.0000/-4.0000/-20.0000$ | -1.3333/-2.0000/-4.0000/-20.0000 | `results_m8_elasticity.json` exogenous.*.fit |
| G-32 | P | 卷Ⅰ (I-5.16b) | 0 | 0 | `verify_numbers.py` 内重算 |

**判据与容差。** 容差按「正文给到哪一位」定，不按「数值算得多准」定：正文写 0.890（三位小数）就容 $\pm5\times10^{-4}$，写 $6.3\times10^{-6}$ 就容 $\pm5\times10^{-8}$。这条例在脚本里被反过来用作**破坏检验**：24 行里 21 条是单个数值，其余是区间或对比串（不适用这个比较）。对那 21 条：若某条的容差大于正文的最后一位单位，把正文改一个末位就检不出来，该行等于没核。脚本逐条做这个比较，当前 **21/21 满足「容差 < 末位单位」**——故「全过」不是因为判据松。

**这张表查出来的第一件事，是有一处追不到。** 卷Ⅰ 表 F-3 有三行数据，其中「规则 2 单窗、$\rho=0$」与「规则 2 单窗、$\rho=0.8$」两行（0.021／0.020／0.019 与 0.173／0.223／0.241）**只在早期仿真报告里，`results_all.json` 的 `M5` 段没有保存**：`M5` 只落了六档 $\sigma_\eta$ 的 `fpr_rule1`／`fpr_rule2` 与 `n_win_sweep` 四项，没有单窗的两行。这不是算错，是**结果没落盘**——重跑 `sim/m5_gate.py` 才能补上。此处登记为「未落盘」，不改表里的数（数来自当次运行，报告里有；改数才是造假，补跑才是修）。

**第二件事：`M5` 的零模型不是 RL 运行。** 脚本自注「零模型为健康系统的 $\gamma$ 序列，非真实 RL 运行」。表 F-3 报的是**规则在合成零模型上的** FPR，不是某个已发表系统的假阳性率（正文 §8.3 同口径）。

**第三件事：这张表不扩覆盖率的分母。** 它核的是 24 条**正文数值**，不是 24 个**公式号**；表 G-1 的 8/250 因此不动。两张表的分母不同，不能相加，也不能相除。

## 参考文献

仅列正文提及的文献，按作者姓氏字母序排列。

1. Bekenstein, J. D. (1981). Universal upper bound on the entropy-to-energy ratio for bounded systems. *Physical Review D*, 23(2), 287–298. https://doi.org/10.1103/PhysRevD.23.287
2. Bousso, R. (2002). The holographic principle. *Reviews of Modern Physics*, 74(3), 825–874. https://doi.org/10.1103/RevModPhys.74.825
3. Bremermann, H. J. (1962). Optimization through evolution and recombination. In M. C. Yovits, G. T. Jacobi, & G. D. Goldstein (Eds.), *Self-Organizing Systems 1962* (pp. 93–106). Washington, DC: Spartan Books.
4. Hawking, S. W. (1975). Particle creation by black holes. *Communications in Mathematical Physics*, 43(3), 199–220. https://doi.org/10.1007/BF02345020
5. Kolmogorov, A. N. (1965). Three approaches to the quantitative definition of information. *Problems of Information Transmission*, 1(1), 1–7.
6. Kuhn, T. S. (1962). *The Structure of Scientific Revolutions*. University of Chicago Press.
7. Landauer, R. (1961). Irreversibility and heat generation in the computing process. *IBM Journal of Research and Development*, 5(3), 183–191. https://doi.org/10.1147/rd.53.0183
8. LiangRuifeng（梁瑞峰）(2026). 《相对信息论》（Relational Information Framework, RIF）v1.5，第一编—第三编，预印本。https://doi.org/10.5281/zenodo.24365795
9. Lloyd, S. (2000). Ultimate physical limits to computation. *Nature*, 406(6799), 1047–1054. https://doi.org/10.1038/35023282
10. Margolus, N., & Levitin, L. B. (1998). The maximum speed of dynamical evolution. *Physica D*, 120(1–2), 188–195. https://doi.org/10.1016/S0167-2789(98)00054-2
11. Nicolis, G., & Prigogine, I. (1977). *Self-Organization in Nonequilibrium Systems: From Dissipative Structures to Order through Fluctuations*. New York: Wiley.
12. Shannon, C. E. (1948). A mathematical theory of communication. *Bell System Technical Journal*, 27, 379–423, 623–656. https://doi.org/10.1002/j.1538-7305.1948.tb01338.x
13. Still, S., Sivak, D. A., Bell, A. J., & Crooks, G. E. (2012). Thermodynamics of prediction. *Physical Review Letters*, 109, 120604. https://doi.org/10.1103/PhysRevLett.109.120604
14. Ulanowicz, R. E. (1997). *Ecology, the Ascendent Perspective*. Columbia University Press.
15. United Nations Development Programme (2025). *Human Development Report 2025*. New York: UNDP.
16. United Nations, Department of Economic and Social Affairs, Population Division (2024). *World Population Prospects 2024*.

***

<!-- VOLUME Ⅱ ｜ 持久结构的演化：复杂度攀升的热力学框架 -->
## 卷Ⅱ　持久结构的演化：复杂度攀升的热力学框架

> **本卷＝卷Ⅱ。**

## 摘要

本卷回答两个问题：**持久结构为什么会随时间变得越来越复杂，什么决定了复杂度跃迁何时发生。**

方法把“攀升”拆成四个可核算的量：**存续势** $V$（单位能量成本换得的信息与存续时间之积，$\mathrm{bit\cdot s/J}$）、三个**弹性指数** $\alpha,\beta,\gamma$、解码器的两个算子（**递归展开** $\mathcal{F}$ 与**拓扑跃迁** $\mathcal{T}$）与**规则深度** $D_{\mathrm{depth}}$，再装入一个“连续流＋离散跳跃”的混合动力系统：连续段由 Logistic 增长与热力学衰减竞争决定，离散段由跃迁映射与容量重置给出。

核心论点三条，强度不同。其一，**弹性排序** $\alpha/\gamma>1>\beta/\gamma$ 是**经验假说**而非推导结果；它与计量单位无关，其稳定性取决于跨系统、跨观察窗的可比性。其二，跃迁需三项条件同时满足：可被新解码器提取的**候选范式突破信号** $\tilde I_{\mathrm{orig}}$、超过一次性建造成本的自由能预算、**智慧杠杆系数** $L_{\mathrm{lev}}=\Delta V/E_{\mathrm{build}}$ 越阈；三者必要而非充分。其三，多数结构停在原层级，被 **D-锁死**、**信号缺失**、**能量锁死** 或**边际回报未耗尽**之一困住，而停住是该约束几何下的局部最优。

**边界声明。** 本卷不处理第一个解码器的起源；跨域只作定性结构比较；复杂度攀升被当作待检验的跨尺度统计假说，不主张全尺度、全时段的单调趋势——局域有序与全局熵增同受一个总熵约束；$V$ 是描述性框架，不构成规范性判据。

**关键词**：存续势；弹性指数；拓扑跃迁；规则深度；混合动力系统；复杂度攀升

**Abstract.** This volume answers two questions: **why persistent structures become more complex over time, and what determines when a complexity transition occurs.**

The method breaks "ascent" into four accountable quantities: the **viability potential** $V$ (the product of information and persistence time obtained per unit of energy cost, in $\mathrm{bit\cdot s/J}$), the three **elasticity exponents** $\alpha,\beta,\gamma$, the decoder's two operators (**recursive unfolding** $\mathcal{F}$ and **topological transition** $\mathcal{T}$) and the **rule depth** $D_{\mathrm{depth}}$. These are then embedded in a hybrid dynamical system of "continuous flow plus discrete jumps": the continuous segment is determined by the competition between logistic growth and thermodynamic decay, and the discrete segment is given by a transition map and a capacity reset.

There are three core theses, of differing strength. First, the **elasticity ordering** $\alpha/\gamma>1>\beta/\gamma$ is an **empirical hypothesis** and not a derived result; it is independent of measurement units, and its stability depends on comparability across systems and across observation windows. Second, a transition requires three conditions to be met at once: a **candidate paradigm-breaking signal** $\tilde I_{\mathrm{orig}}$ that a new decoder can extract, a free-energy budget exceeding the one-time construction cost, and a **wisdom lever coefficient** $L_{\mathrm{lev}}=\Delta V/E_{\mathrm{build}}$ that crosses its threshold; the three are necessary and not sufficient. Third, most structures stay at their original level, trapped by one of **D-lock-in**, **signal absence**, **energy lock-in** or **marginal returns not exhausted**, and the standstill is a local optimum under that constraint geometry.

**Scope statement.** This volume does not address the origin of the first decoder; cross-domain work is limited to qualitative structural comparison; complexity ascent is treated as a cross-scale statistical hypothesis to be tested, and no monotonic trend over all scales and all periods is claimed — local order and global entropy increase are subject to one total-entropy constraint; $V$ is a descriptive framework and does not constitute a normative criterion.

**Keywords**: viability potential; elasticity exponents; topological transition; rule depth; hybrid dynamical system; complexity ascent

***

## 第一章　引言：尚未回答的问题

### 1.1 本卷回答什么

存续动力学给定一个已存在的结构，分析其存续势、崩溃与行为病理，刻意对起源保持不可知，因而留下前置问题：**结构是怎么变成现在这个样子的？** 神经系统的存续条件可以被分析，但它为何出现、为何并非所有谱系都发展出它，本框架不作答。

本卷分三个子问题处理它：**方向性从哪来**（若攀升不是目的论的，是什么让物质组织在统计上偏向更复杂、更密集信息、更具因果能力的配置）；**门槛在哪**（层级跨越是离散事件，什么条件决定一个结构能否跨过阈值）；**为何多数停住**。三者分别对应第二章的弹性指数与解码器算子、第三章的混合动力系统、第四章的三条件与可判定表。

### 1.2 方向性信号及其证据地位

可观测宇宙包含一个方向性信号：物质把自己组织成更复杂、更密集信息、更具因果能力的配置——单细胞先于神经系统，神经系统先于语言。每次跨越都是小概率事件，而序列在样本内同向。

**这是统计倾向，不是普遍必然。** 本卷主张：在所选样本与观察窗（宇宙年龄尺度）内，规则深度呈向上累积的倾向。该倾向是否显著、能否外推，本身是 HⅡ-6 要检验的假说——把样本内的模式写成宇宙律，本卷不做。

**倾向不等于单调。** 攀升与简化在同一棵演化树上都发生：寄生虫丢失器官、洞穴鱼丢失视觉，都是规则深度下降，且在各自约束下是正确的最优化（第七章写成负拓扑跃迁）。本卷的“方向”是净累积的统计偏向。

**局域有序与全局熵增不矛盾。** 晶体靠降低自身熵并向外放热形成，生命靠摄入低熵自由能、排出更高熵废物维持低熵，文明靠燃烧化石燃料维持结构；三者服从同一个总熵约束——任何局域有序化都以环境更大的熵增为代价。生命是第二定律允许的耗散结构中最精致的一类（Schneider & Kay, 1994）。

***

## 第二章　理论背景：核心概念

### 2.1 存续势及其两个通道

核心指标是**存续势** $V$：一个持久结构在单位能量成本上换得的信息量与存续时间之积，低阶形式为 $V\approx I\cdot T/E$，其中 $I$ 为信息量（bit）、$T$ 为存续时间（s）、$E$ 为能量成本（J）。$V$ 的量纲是 $\mathrm{bit\cdot s/J}$——**它带 bit 因子，不是无量纲量**，只有 $v=V/V_0$ 才无量纲；后果是 $V$ 随信息计量协议变化，跨系统比较须先锁定读数协议（第 6.3 节）。

客观存续势叠加两个通道：

$$
V_{\mathrm{obj}} = \underbrace{\frac{I_{\mathrm{struct}} \cdot T_{\mathrm{struct}}}{E_{\mathrm{struct}}}}_{V_{\mathrm{s}}\ (\text{结构通道})} + \underbrace{\frac{I_{\mathrm{causal}} \cdot T_{\mathrm{causal}}}{E_{\mathrm{causal}}}}_{V_{\mathrm{c}}\ (\text{认知通道})} \tag{II-2.1}
$$

其中 $E_{\mathrm{struct}}=E_{\mathrm{barrier}}+E_{\mathrm{survival}}$，$E_{\mathrm{eff}}=E_{\mathrm{struct}}+E_{\mathrm{causal}}$。$E_{\mathrm{barrier}}$ 是势垒所对应的成本分摊，不等于势垒高度（后者另记 $\Delta U_{\mathrm{barrier}}$）；$E_{\mathrm{survival}}$ 是为补偿熵增而主动耗散的能量；$E_{\mathrm{causal}}$ 是解码器运行所耗，含持有者的解码代价。

$V_{\mathrm{s}}$ 捕获靠能量壁垒抵抗熵增、不需持续供能的被动结构；$V_{\mathrm{c}}$ 捕获靠预测环境、引导能量流维持自身的主动结构。从 $V_{\mathrm{c}}=0$ 到 $V_{\mathrm{c}}>0$ 是最根本的不连续性：不是有序程度的提高，而是存续机制的更换——前者靠不动维持，后者靠动维持（第 5.1 节展开）。

**可加性限制。** 式 (II-2.1) 的加号是建模约定，不是定理：两通道的读数协议与背景不同，都以 bit 计并不构成可加性证明。它只在同一读数协议、同一背景参照、同一观察窗且完成域内校准时可作数值使用；否则 $V_{\mathrm{obj}}$ 只作序关系指标，不可报出数值或比值。

### 2.2 弹性指数与三条路线：单位不变性与经验假说

存续势对信息、时间、能量的响应由三个**弹性指数**刻画：

$$
\alpha=\frac{\partial \ln V}{\partial \ln I},\qquad
\beta=\frac{\partial \ln V}{\partial \ln T},\qquad
\gamma=-\frac{\partial \ln V}{\partial \ln E_{\mathrm{eff}}}. \tag{II-2.2}
$$

$\gamma$ 前的负号使“能量成本上升导致 $V$ 下降”对应正的 $\gamma$；三个指数为正时，含义统一为“该资源增加百分之一，$V$ 增加（或减少）百分之几”。

**（一）三个指数及其比值都是无量纲量，且对单位换算不变。** 对数—对数斜率是两个相对变化量之比，分子分母都是纯数。设作单纯单位换算 $I\mapsto c_I I$、$T\mapsto c_T T$、$E_{\mathrm{eff}}\mapsto c_E E_{\mathrm{eff}}$（$c>0$，如 $\mathrm{J}\to\mathrm{kJ}$ 给 $c_E=10^{-3}$），由 $\ln(c_I I)=\ln I+\ln c_I$ 得

$$
\frac{\partial \ln V}{\partial \ln(c_I I)}=\frac{\partial \ln V}{\partial \ln I}\cdot\frac{\partial \ln I}{\partial \ln(c_I I)}=\frac{\partial \ln V}{\partial \ln I}=\alpha ,
$$

$\beta,\gamma$ 同理；比值 $\alpha/\gamma$、$\beta/\gamma$ 由两个不变量相除，亦不变。故“指数依赖单位、只有比值不变”一语，把定义给出的不变性与估计带来的不确定性混为一谈。

**（二）会改变估计值的是四件事。** 操作化定义（$I$ 取可区分构型数的对数，还是参数量这类代理）、代理指标（同一操作化定义下换代理，会把不同方差来源带进回归）、观察域（不同解码器基底、状态空间与观察窗给出不同局部斜率，跨域合并得到混合斜率）、拟合模型（回归形式、是否固定截距、是否把通道权重当常数）。

**（三）估计 $\alpha$、$\gamma$ 须固定通道权重 $\varphi$。** 净有效因果信息按能量份额合成：

$$
I_{\mathrm{net}}=\varphi_{\mathrm{s}}I_{\mathrm{struct}}+\varphi_{\mathrm{c}}I_{\mathrm{causal}},\qquad
\varphi_{\mathrm{s}}=\frac{E_{\mathrm{struct}}}{E_{\mathrm{eff}}},\quad
\varphi_{\mathrm{c}}=\frac{E_{\mathrm{causal}}}{E_{\mathrm{eff}}},\quad
\varphi_{\mathrm{s}}+\varphi_{\mathrm{c}}=1 .
$$

$\varphi$ 本身是 $E$ 的函数，直接回归 $\ln V$ 对 $\ln E_{\mathrm{eff}}$ 会使系数同时吸收“总能量增加使分母变大”与“能量构成变化改变加权方式”两种效应。处理有二：观察窗内把权重当常数，只取构成近似不变的样本；或把 $\varphi_{\mathrm{c}}$ 作协变量显式纳入模型。$\alpha$ 同理。

**（四）排序是一个经验假说。**

$$
\frac{\alpha}{\gamma}>1>\frac{\beta}{\gamma}. \tag{II-2.3}
$$

**【假说 2.1（弹性排序）】**
- **陈述**：在锁定解码器基底与状态空间的域内，信息弹性与能量弹性之比大于 1，时间弹性与能量弹性之比小于 1。
- **支持理由**：仅基于三类资源相对稀缺性的定性推理——能量受热力学下界约束、时间受物理寿命约束、信息可复制而无质量成本，故信息投资的边际收益应高于能量投资。无第一性原理推导，也无通过预注册协议的实证。
- **证伪条件**：在满足锁定条件的域内，以固定权重与同一读数协议估计出 $\alpha/\gamma\le 1$ 或 $\beta/\gamma\ge 1$，且区间排除 1。这一条同时是 HⅡ-4 的反驳条件。

把 $V\approx I\cdot T/E$ 取对数后全微分，得可操作形式

$$
\frac{\Delta V}{V}\approx \alpha\cdot\frac{\Delta I}{I}+\beta\cdot\frac{\Delta T}{T}-\gamma\cdot\frac{\Delta E_{\mathrm{eff}}}{E_{\mathrm{eff}}}. \tag{II-2.4}
$$

式 (II-2.4) 只在相对变化不大时可用；大范围比较须回到 $V$ 的原式。

**演化真正优化的是 $V$，不是 $I$。** 排序只说明机会成本相近时 $I$ 路线具有最高的长期边际收益，不意味着所有谱系都须优先增加信息。结构可以沿三条路线各自最大化 $V$：

| 路线 | 机制 | 典型案例 |
| :---------------- | :------------------- | :---------------------- |
| **$I$ 路线（复杂化）** | 提高 $I_{\mathrm{net}}$，推高 $V$ 的理论上限 | 神经系统、语言、文明、人工计算 |
| **$T$ 路线（长寿化）** | 延长 $T_{\mathrm{pred}}$ 或 $T_{\mathrm{struct}}$ | 松树、海龟、裸鼹鼠、种子休眠 |
| **$E$ 路线（节能化）** | 降低 $E_{\mathrm{eff}}$ | 寄生虫、洞穴鱼、深海生物、冬眠 |

三条路线受局部热力学约束共同筛选：海龟若增加复杂神经系统，能量代价项 $\gamma\Delta E/E$ 会超过信息增益项 $\alpha\Delta I/I$，使 $\Delta V<0$；植物休眠几乎不改变 $I$，仅靠降低 $E$ 并延长有效 $T$ 即抬高 $V$。这是 $\max V$ 原则在不同约束几何下的不同解。

$I$ 路线的第二层机制是存量：高 $I$ 结构积累更大的 $V_{\mathrm{obj}}$，在同等规模的 $I^{-}$ 冲击下相对损失更小；若排序成立，它积累存量快于另两条路线，故攀升表现为长期统计趋势，而非每个谱系必须遵循的策略。

### 2.3 解码器、拓扑跃迁与范式突破信号

**信息解码器** $D$ 是持久结构从潜在构型 $I_{\mathrm{latent}}$ 中提取有效因果信息的物理机制。$I_{\mathrm{latent}}$ 是未激活但可恢复的因果能力存量（bit）；解码效率 $\eta_D\in[0,1]$ 满足 $I_{\mathrm{active}}=\eta_D I_{\mathrm{latent}}$。解码器质量由 $\eta_D$ 与容量上限 $I_{\max}(D)$ 表征。

两个算子支配解码器的变化。**递归展开 $\mathcal{F}$** 让同一解码器在多尺度上复制其规则，结构更大或更密，**不打开新的因果维度**（血管树的分支、肺泡的重复）。**拓扑跃迁 $\mathcal{T}$** 吸收范式突破信号 $I_{\mathrm{orig}}$ 并重组结构，**打开新的因果维度**：旧解码器对该信号近乎无响应（$D_n(I_{\mathrm{orig}})\approx 0$），新解码器能有效提取它（$D_{n+1}(I_{\mathrm{orig}})\gg 0$）；$\mathcal{T}$ 需一次性建造成本 $E_{\mathrm{build}}$，成功时 $I_{\max}(D_{n+1})>I_{\max}(D_n)$。

递归展开算子的最小数学形式为

$$
S_{n+1}=\mathcal{F}\left(S_n,\lambda_{\mathcal{F}}\right) \tag{II-2.5}
$$

其中 $S_n$ 为第 $n$ 代结构状态，$\lambda_{\mathcal{F}}$ 为受 $E_{\mathrm{causal}}$ 与 $I_{\mathrm{net}}$ 共同约束的控制参数。$\mathcal{F}$ 在尺度变换下不变时结构呈分形式自相似；$\mathcal{T}$ 对应 $\lambda_{\mathcal{F}}$ 的离散跳变，打破旧的尺度不变性。

### 2.4 规则深度：静态定义、深度指数与标定假设

“规则深度”在本卷内指**深度指数**，它有两个版本，须分开命名、分开使用。

**（一）静态定义 $D_{\mathrm{depth}}$。** 给定对象 $P$ 与容差 $\varepsilon_{\mathrm{tol}}$，静态规则深度是在该容差内把 $P$ 还原为规则描述所需的**最少互相独立规则数**。“规则”指一段可执行的重写指令；“独立”指去掉任一条后其余规则无法生成它覆盖的输出；容差是允许的最大重构误差，报数时须写全。随机构型取 0；完美晶体只需一条规则（“全同占据”），$D_{\mathrm{depth}}=1$；机械钟表需要齿轮传动、发条储能、指针指示等多条不可互推的规则。重复展开不增加深度：雪花枝晶是同一条规则在不同尺度重复。

**（二）动力学指标。** 本卷定义

$$
D_{\mathrm{depth}}^{\mathrm{dyn}}\equiv 1+\#\{\mathcal{T}\}, \tag{II-2.6}
$$

即初始层级记 1，此后每发生一次拓扑跃迁加一；该式仅对静态深度不小于 1 的对象有定义。

**（三）二者相等是标定假设，不是定义推出的等式。** 一次跃迁可能同时引入多条不可互推的规则（真核细胞的区室化同时带来膜系统、细胞骨架与细胞核），也可能只是重新组织已有规则，故 $D_{\mathrm{depth}}\overset{?}{=}1+\#\{\mathcal{T}\}$ 标为**标定假设**。检验方式是分别测出 $D_{\mathrm{depth}}$（压缩式描述长度与规则不可约性判定）与 $\#\{\mathcal{T}\}$（形态创新事件计数或系统发育事件树的节点数），回归 $D_{\mathrm{depth}}=a+b\cdot\#\{\mathcal{T}\}$ 并检验 $b=1$、$a=1$：该检验的**先验预期应是 $b>1$ 而非 $b=1$**：只要一次跃迁平均引入多于一条独立规则，斜率就大于 $1$（模型族内的算例：每次跃迁新增 1—3 条、其中 $20\%$ 的跃迁只作重组时，$\hat b\approx1.3$，$b=1$ 被强拒，$p<10^{-6}$；见 RIF 附录 C 表 C-6）。因此 $D_{\mathrm{depth}}^{\mathrm{dyn}}$ **默认按序数刻度使用**——只能说谁更深，不能说深多少；只有 $b$ 与 $1$ 无显著差异时，才可升级为基数刻度。把“通过则基数”写成默认路径，等于把一个几乎必然失败的检验当成常规预期；“一次跃迁恰好引入一条独立规则”是特例，不是通例。

$D_{\mathrm{depth}}$ 与 $I_{\mathrm{struct}}$ 正交：章鱼在一次主要跃迁后进行了广泛的 $\mathcal{F}$ 展开，故很大但很浅；某些多层调控网络很深但不大。深度还以**类型—实例分离**为前提：类型是可遗传的信息模板，实例是具体的物理个体（岩石无分离，RNA 原始分离，数字实体完全分离）；没有分离，结构能积累的规则数就超不过单个载体在不解体前提下承载的规则数，而载体寿命受 $T_{\mathrm{struct}}^{\max}$ 约束。

### 2.5 证据等级与记号约定

本卷结论按四级标签标注强度：标【定理】的必须给出完整推导，标【假说】的不许在结论章被当作已证事实使用。

| 标签 | 使用条件 | 必须附带 |
| :----------- | :-------------------------- | :------------------- |
| **【定理】** | 前提明确列出、推导完整、结论在该前提下严格成立 | 前提、结论、证明或推导、适用域 |
| **【命题】** | 有形式化陈述，但前提待标定，或推导某一步依赖未证的建模假设 | 前提、结论、依赖的假设、失效条件 |
| **【候选推论】** | 由某命题在附加条件下导出，未独立检验 | 母命题、附加条件、可测后果 |
| **【假说】** | 经验性或机制性猜测，无形式化推导 | 陈述、支持理由、证伪条件 |

裸写 $I$ 默认指 $I_{\mathrm{net}}$；$\tilde I_{\mathrm{orig}}$ 与 $I_{\mathrm{orig}}$ 不得互换；六个时间记号不得互换，也不得裸写 $T$ 指代其一。完整记号见附录 A。

***

## 第三章　统一信息演化方程：连续流与离散跳跃

上一章的概念组装成一个动力学系统：一段**连续流**，描述当前解码器下信息如何增长、如何向平衡态衰减；一串**离散跳跃**，描述拓扑跃迁如何改变状态与容量。把两者混进一个带狄拉克 $\delta$ 的方程里，会让“跳变”与“重置”两笔不同的账挤在同一项中。

### 3.1 混合动力系统的形式

状态由三个量组成：信息量 $I(t)$（bit）、解码器 $D(t)$、容量 $I_{\max}(D)$（bit）。$D$ 在两次跃迁之间保持不变，系统因此**分段光滑**：相邻两次跃迁之间 $I$ 满足一个常微分方程；在跃迁时刻 $t_j$，$I$ 与容量按跳跃规则瞬时改变。

**（一）连续段。** 在 $t\in(t_{j-1},t_j)$ 上，

$$
\frac{\mathrm{d}I}{\mathrm{d}t}=\mathcal{F}(D,I)-\frac{I-I_{\mathrm{eq}}}{\tau_{\mathrm{decay}}}. \tag{II-3.1}
$$

$\mathcal{F}$ 须显式依赖 $I$：若它只是 $D$ 的函数，方程在任何容量下都线性增长，与边际回报递减矛盾。本卷取受容量约束的 Logistic 形式：

$$
\mathcal{F}(D,I)=\mu_{\mathcal{F}}\,I\left(1-\frac{I}{I_{\max}(D)}\right), \tag{II-3.2}
$$

其中 $\mu_{\mathcal{F}}>0$ 为展开速率参数（$\mathrm{s^{-1}}$）。$I=0$ 时展开率为零；$I\to I_{\max}(D)$ 时趋零；$I$ 略大于 $I_{\max}$ 时为负，超容量结构被压回容量内。换一个 $\mathcal{F}$，平衡点的解析式就变，但“存在正平衡点、且其位置随容量上移”在广泛的单峰饱和族中都成立。

**（二）跳跃映射。** 在跃迁时刻 $t_j$，

$$
I\left(t_j^{+}\right)=I\left(t_j^{-}\right)+\Delta I_{\mathcal{T},j},\qquad \Delta I_{\mathcal{T},j}\ge 0, \tag{II-3.3}
$$

其中 $\Delta I_{\mathcal{T},j}$ 是第 $j$ 次跃迁**实际写入结构**的信息增量。它与候选信号读数 $\tilde I_{\mathrm{orig}}$ **不是同一个量，两者关系未建立**（**不可据此写成** $\Delta I_{\mathcal{T},j}\le\tilde I_{\mathrm{orig},j}$：稀有度读数不是写入量，写入量须另行标定）。被呈现的信号只有一部分能被新解码器真正写入。

**（三）容量重置。** 同一次跃迁还改变容量上限：

$$
I_{\max}\left(D_{n+1}\right)>I_{\max}\left(D_n\right),\qquad
D_{\mathrm{depth},n+1}^{\mathrm{dyn}}=D_{\mathrm{depth},n}^{\mathrm{dyn}}+1. \tag{II-3.4}
$$

第二式只在标定假设通过检验的域内成立；否则只保留第一式，深度只记序数变化。

**（四）脉冲项与重置算子不得重复计数。** **脉冲项只记信息量的瞬时增加**，它改变 $I$ 的当前值，不改变容量；**重置算子只记容量上限的改变**，它不改变 $I$ 的当前值，因此重置**不产生** $I$ 的跳变。把“容量抬高之后 $I$ 被 Logistic 项拉向新上限”算作跃迁收益，等于把未来数年的连续增长记到跃迁那一瞬的账上。

由此得记账规则：**每次跃迁在账上恰好一条主记录**——（a）$\Delta I_{\mathcal{T},j}>0$ 且容量上升（常规跃迁）；（b）$\Delta I_{\mathcal{T},j}=0$ 且只有容量上升（纯容量跃迁：规则被重新组织，当前信息量不变但上限提高）。第二种并不罕见：多细胞化的分工在当下不增加总信息量，却把未来的容量天花板抬高一个量级。

**（五）解的存在性与正则性。** 在 $(0,I_{\max})$ 上 $\mathcal{F}$ 连续可微、衰减项线性，故每个连续段内解存在且唯一；跳跃时刻由第四章的门控条件触发，整个系统是一个混合自动机。本卷设**最小跃迁间隔** $\tau_{\mathcal{T}}>0$：结构重组需要建造时间；没有它，模型允许无限密集的跃迁（Zeno 行为），而无限密集的跃迁在物理上等价于连续变化。

### 3.2 三项的物理含义

**递归展开**是当前解码器下的连续增长，随 $I\to I_{\max}(D)$ 边际回报趋于零；晶体、病毒与复制分子主要通过 $\mathcal{F}$ 运作。**拓扑跃迁**是吸收信号并重组解码器的离散跳变：**边际成本一次付清且很高（$E_{\mathrm{build}}$），边际收益在长期释放**，这正是它成为门控事件的原因。**热力学衰减**：无主动维持时，任何有序结构都以特征时间 $\tau_{\mathrm{decay}}$ 衰减向 $I_{\mathrm{eq}}$，纯粹被动的结构（$E_{\mathrm{causal}}=0$）仅由该项支配；$\tau_{\mathrm{decay}}$ 与温度、势垒、载体的关系须由具体机制给出（如热激活过程给 $\tau_{\mathrm{decay}}\propto e^{\Delta U_{\mathrm{barrier}}/k_BT_{\mathrm{thermo}}}$），它是待标定参数。

### 3.3 特例还原

**被动晶体。** $\mathcal{F}=0$，无跃迁，方程化为 $\mathrm{d}I/\mathrm{d}t=-(I-I_{\mathrm{eq}})/\tau_{\mathrm{decay}}$。衰减被 $E_{\mathrm{barrier}}\gg k_BT_{\mathrm{thermo}}$ 抑制，$\tau_{\mathrm{decay}}$ 极大，$I\approx\mathrm{const}$：晶体的存续是衰减时间远长于观察窗。

**复制分子。** $\mathcal{F}>0$（模板导向复制），跃迁罕见。令式 (II-3.1) 右端为零，得正平衡点

$$
I^{*}=\frac{I_{\max}(D)}{2}\left[\left(1-\frac{1}{\mu_{\mathcal{F}}\tau_{\mathrm{decay}}}\right)+\sqrt{\left(1-\frac{1}{\mu_{\mathcal{F}}\tau_{\mathrm{decay}}}\right)^{2}+\frac{4I_{\mathrm{eq}}}{I_{\max}(D)\,\mu_{\mathcal{F}}\tau_{\mathrm{decay}}}}\right],
$$

取 $I_{\mathrm{eq}}=0$ 时化为 $I^{*}=I_{\max}(D)\left(1-1/(\mu_{\mathcal{F}}\tau_{\mathrm{decay}})\right)$，正不动点的充要条件是 $\mu_{\mathcal{F}}\tau_{\mathrm{decay}}>1$。**$I_{\mathrm{eq}}>0$ 时该条件不再必要**：热背景注入使 $\mu_{\mathcal{F}}\tau_{\mathrm{decay}}<1$ 时仍可有正不动点，判据须用上式完整形式。稳定性由 $f'(I^{*})=-\mu_{\mathcal{F}}\sqrt{\left(1-1/(\mu_{\mathcal{F}}\tau_{\mathrm{decay}})\right)^{2}+4I_{\mathrm{eq}}/(I_{\max}\mu_{\mathcal{F}}\tau_{\mathrm{decay}})}<0$ 给出，对一切使根式有实值的参数成立。由此得一道可判据的门槛：**在无热背景注入的系统中，展开速率与衰减时间之积必须超过 1，结构才能维持在平衡态之上**；低温保存有效，正因为降温使 $\tau_{\mathrm{decay}}$ 增大。

**活跃演化的生物体。** 三项均起作用：前两项驱动 $I$ 向上，第三项要求由 $E_{\mathrm{survival}}+E_{\mathrm{causal}}$ 支付连续维护成本，平衡点在增长速率等于衰减速率处。**D-锁死系统**则 $\mathcal{F}\to 0$，跃迁被阻断，方程退化为纯衰减；“锁死”是动力学陈述（净增长率趋零），不是结构必然崩溃——锁死系统可靠持续供能长期维持现状。

### 3.4 维持功率下界【命题】

衰减项在式 (II-3.1) 中是纯信息学的项，本身不含能量；要说“衰减项设定了存续的最低能量需求”，必须补一条把信息衰减与能量耗散连起来的关系。本卷补的是一条条件命题。

**【命题 3.1（维持功率下界）】**
- **前提**：（i）系统以“擦除—重写”方式维持其信息，即每个被维持的比特在每 $\tau_{\mathrm{decay}}$ 内至少被擦除并重写一次；（ii）擦除是逻辑不可逆操作，其每比特能量下界为朗道尔界 $E_{\mathrm{L,bit}}=k_BT_{\mathrm{thermo}}\ln 2$（$\mathrm{J/bit}$）；（iii）环境温度 $T_{\mathrm{thermo}}$ 在观察窗内恒定；（iv）所计的是擦除环节的产热下界，不含写入、传输、纠错与冷却的额外开销。
- **结论**：维持全部 $I$ 比特所需的平均功率满足

$$
\dot E_{\mathrm{maintain}}\ \ge\ k_BT_{\mathrm{thermo}}\ln 2\cdot\frac{I}{\tau_{\mathrm{decay}}}. \tag{II-3.5}
$$

- **推导**：由 (i)，一个衰减周期内需擦除的比特数为 $I$；由 (ii)，每比特耗能不少于 $E_{\mathrm{L,bit}}$，故周期内能量不少于 $E_{\mathrm{L,bit}}I$；由 (iii)，该能量在 $\tau_{\mathrm{decay}}$ 内均匀支出时功率不少于 $E_{\mathrm{L,bit}}I/\tau_{\mathrm{decay}}$。
- **依赖的假设**：式 (II-3.5) 完全依赖前提 (i)。若系统采用可逆计算、外部存储、纠错码（刷新周期长于 $\tau_{\mathrm{decay}}$）或回放机制，前提 (i) 被违反，式 (II-3.5) 不再给出有效下界——真实维持功率可以低于该值，也可以因纠错开销高于该值，方向不定。
- **失效条件**：（a）信息以非擦除方式维持（拓扑保护的量子存储、可逆逻辑）；（b）温度在窗口内显著变化，此时须用积分形式 $\dot E_{\mathrm{maintain}}\ge k_B\ln 2\cdot\overline{T_{\mathrm{thermo}}I}/\tau_{\mathrm{decay}}$；（c）用于生物系统时，代谢功率的计量口径（化学自由能而非热耗散）与本式不同，不可直接对比。

**量级校验。** 取 $I=10^{12}$ bit、$\tau_{\mathrm{decay}}=10^{4}$ s、$T_{\mathrm{thermo}}=300$ K，则 $E_{\mathrm{L,bit}}\approx2.87\times10^{-21}$ J，式 (II-3.5) 给出 $\dot E_{\mathrm{maintain}}\gtrsim2.9\times10^{-13}$ W，比真实生物体或芯片的维持功率（典型 $10^{-4}$ W 量级）弱约九个数量级。**朗道尔界对实际系统的维持成本是极弱的下界**，真实成本由化学动力学、材料疲劳、纠错与散热决定。式 (II-3.5) 给出一个不可逾越的地板：任何声称“维持成本低于此值”的方案，必然违反了前提 (i) 至 (iii) 之一。

系统整体可视为受热力学耗散修正的递归动力系统：$\mathcal{F}$ 对应吸引子动力学，$\mathcal{T}$ 对应分岔事件，攀升序列因而是**受能量门控的分岔级联**。

***

## 第四章　复杂度跃迁的三个条件

拓扑跃迁是否发生，由三个条件共同门控。三条判据的可操作性差别很大：条件一依赖统计读数，条件二依赖能量核算，条件三依赖跨解码器的 $V$ 比较。凡可比性不满足处，本卷只报定性跃迁，不报杠杆数值。

### 4.1 条件一：信号可用性（含 $I_{\mathrm{orig}}$ 的三层拆分）

条件一的原始表述是：环境中必须存在范式突破信号，使当前解码器无法提取（$D_n(I_{\mathrm{orig}})\approx0$）而重组后的解码器可以（$D_{n+1}(I_{\mathrm{orig}})\gg0$）。这个表述有隐蔽的循环：若 $I_{\mathrm{orig}}$ 只能事后确认，它就不能同时充当跃迁前的门控变量。本卷拆成三层，只有第一层进门控。

**第一层：候选范式突破信号 $\tilde I_{\mathrm{orig}}$（可观测代理）。** 定义为 $D_n$ 在目标上的预测残差相对于自身历史残差分布的稀有度：

$$
\tilde I_{\mathrm{orig}}\equiv-\log_2\Pr_{B_n}\left(\varepsilon_{\mathrm{res}}\ge\varepsilon_{\mathrm{obs}}\right), \tag{II-4.1}
$$

其中 $\varepsilon_{\mathrm{res}}$ 为残差（度量须预先声明），$\varepsilon_{\mathrm{obs}}$ 为本次观测值，$B_n$ 为历史残差分布（须在跃迁前冻结，不得用含本次观测的样本重估）；单位 bit，含义是“这次失败有多罕见”。

**门槛与误报率。** 门控规则须在观测前预注册：（i）显著性水平 $\alpha_0$（例如 $0.01$），对应 $\tilde I_{\mathrm{orig}}\ge-\log_2\alpha_0$；（ii）在 $N$ 次独立复测中至少 $m$ 次越门（例如 $N=3$、$m=2$），以抑制单次异常读数；**与卷Ⅰ 的口径**：卷Ⅰ §2.1 与 §5.1.6（C1）用“连续 $k$ 次越门槛”（示例 $\alpha_0=10^{-3}$），本卷用“$N$ 次中至少 $m$ 次”（示例 $\alpha_0=0.01$）；两种都是门控规则的实例，误报率分别约 $N_{\mathrm{test}}\alpha_0^{k}$ 与 $C(N,m)\alpha_0^{m}$。两种写法各自合法，误报率如上；**采用哪一种须在观测前固定，并与卷Ⅰ 的口径对齐**；（iii）同一窗口内检验多个候选信号时 $\alpha_0$ 须按检验次数下调。三条缺一，高读数只说明“某次观测很意外”。

**第二层：经验证的新增信息 $I_{\mathrm{orig}}$（事后确认量）。** 只有跃迁成功、且新解码器在独立样本上复现出稳定提取能力之后，才把该次跃迁真正带来的新增信息记为 $I_{\mathrm{orig}}$（bit）并报告区间。前者是实现了的信息，后者是“意外的程度”，数值不必相等。

**第三层：拓扑跃迁事件 $\mathcal{T}$。** 结构重组这一事件本身；它是事件不是量，与式 (II-3.3) 联用时幅度由 $\Delta I_{\mathcal{T}}$ 给出。

门控只用第一层，且**越门不等于跃迁必然发生**：$\alpha_0=0.01$ 下即使没有真实新范式，也会有约百分之一的窗口被误判；反之未越门也不排除跃迁，低统计功效会让真实信号读不出来。条件一因而是**排除性判据**。

### 4.2 条件二：能量可用性

一次性建造成本不得超过可用自由能预算：

$$
E_{\mathrm{build}}\left(D_{n+1}\right)<E_{\mathrm{available}}. \tag{II-4.2}
$$

其中 $E_{\mathrm{build}}$ 是创建或升级结构所需的一次性物理能量（J），$E_{\mathrm{available}}$ 是系统当前可动员的能量上限（J），且 $E_{\mathrm{available}}\le E_{\max}$；$E_{\max}$ 是环境的天花板，$E_{\mathrm{available}}$ 是系统实际能调用的部分。

这是硬性门槛，也解释了为何多数生物从未跃迁：重组解码器的能量成本通常比运行当前解码器大几个数量级。建造成本须在建造期内支付，而建造期往往长于一个世代，故成本须分摊到多个个体或世代（社会性昆虫的巢穴、代际知识传递）。

### 4.3 条件三：智慧杠杆（含 $V$ 的可比性前提）

跃迁带来的存续势增益必须超过相对于其成本的最低阈值：

$$
L_{\mathrm{lev}}=\frac{V\left(D_{n+1}\right)-V\left(D_n\right)}{E_{\mathrm{build}}}>L_{\mathrm{lev,min}}. \tag{II-4.3}
$$

$L_{\mathrm{lev}}$ 为**智慧杠杆系数**，量纲 $\mathrm{(bit\cdot s/J)/J}$；$L_{\mathrm{lev,min}}$ 是同量纲的情境阈值。此条件捕获竞争压力：在当前解码器仍产生回报的环境中（$I<I_{\max}(D_n)$），系统没有热力学动力去承担重组成本。

**$V$ 的可比性前提。** 式 (II-4.3) 的分子是两个 $V$ 之差，只有下列四条同时满足时才是可比值。

1. **同一目标**：两者须针对同一类任务或存续问题；旧解码器在觅食上的 $V$ 减去新解码器在导航上的 $V$，得到的是任务差异。
2. **同一观察窗**：两者的 $T_{\mathrm{struct}}$、$T_{\mathrm{causal}}$ 须在同一时间跨度上积分；用短窗比会系统性低估跃迁收益。
3. **同一能量分摊规则**：建造成本、维护成本与共用基础设施的分摊方式必须一致。
4. **共同参照协议**：两通道读数须来自同一协议、同一背景参照、同一容差；跨协议读数不可相减。

四条不满足时本卷**只报定性跃迁**——说明拓扑改变、容量抬高、可提取的因果维度增加，不报 $L_{\mathrm{lev}}$ 的数值。

### 4.4 三个条件的可判定表

按行序判定，因条件一的观测成本最低、条件三最高。

**表 4.1　拓扑跃迁三条件的可判定表**

| 条件 | 判据 | 所需观测量 | 失败时的表型 |
| :-------- | :--------------- | :----------------- | :---------------- |
| **一、信号可用性** | 冻结背景 $B_n$ 下 $\tilde I_{\mathrm{orig}}\ge-\log_2\alpha_0$，且在 $N$ 次独立复测中至少 $m$ 次越门 | 残差序列 $\{\varepsilon_{\mathrm{res}}\}$；历史残差分布 $B_n$；预注册的 $\alpha_0$、$N$、$m$；多重比较校正方案 | 长期无新维度出现；形态停滞（深海固着生物型） |
| **二、能量可用性** | $E_{\mathrm{build}}(D_{n+1})<E_{\mathrm{available}}$，且建造期内功率支付不超过 $\dot E_{\mathrm{available}}$ | 建造期 $\tau_{\mathrm{build}}$；$E_{\mathrm{build}}$ 的能量核算；$\dot E_{\mathrm{available}}$ 的时间曲线；成本分摊机制 | 建造中途停止、结构残缺；或从不启动；或被迫缩小规模 |
| **三、智慧杠杆** | $L_{\mathrm{lev}}=\Delta V/E_{\mathrm{build}}>L_{\mathrm{lev,min}}$，且四条可比性前提全部满足 | 同目标、同窗、同分摊规则下的 $V(D_n)$ 与 $V(D_{n+1})$；$E_{\mathrm{build}}$；$L_{\mathrm{lev,min}}$ | 新解码器建成后被弃用（仪式性器官）；谱系回退到简化路线 |

三行之间存在依赖：条件二不满足时条件三的分子无法实现，条件一不满足时条件三的分子不可归因。

### 4.5 三者为何是必要条件【命题】

**【命题 4.1（三条件的必要性）】**
- **前提**：（i）层级跃迁定义为解码器拓扑改变且容量上限抬高的离散事件（第 3.1 节的跳跃映射）；（ii）$V$ 是筛选的序参量，即同一约束几何下 $V$ 较低的构型在统计上更易被淘汰；（iii）建造需要时间，且建造期内结构必须维持自身。
- **结论**：任一条件不满足，则该次层级跃迁不发生（或在统计上不被保留）。三者合起来是必要条件集的一个子集，不构成充分条件。
- **依赖的假设**：假设 (ii) 是筛选论的表述，不是热力学第一性原理的推论，它需要竞争与复制的附加假设。若无竞争环境，$V$ 的筛选压力消失，条件三的必要性随之减弱——此时跃迁可以发生但不被“保留”。
- **失效条件**：若存在不经解码器重组而实现容量扩张的路径（如直接接入外部存储而不改变内部规则），则条件一与条件三的表述需要改写；本卷把这类情形归入“外化”，其判据另议。

**第一步：没有信号，跳跃映射没有输入。** 由式 (II-3.3)，跃迁的效果是 $I$ 的瞬时增加。若环境中不存在旧解码器读不出的规律，新解码器造出来也无事可做：容量被抬高，可提取的内容却与旧解码器相同，$\Delta I_{\mathcal{T}}=0$。这种“纯形式重组”不构成层级跃迁——按定义 (i)，它要求可提取的因果维度增加。信号可用性因而是**可能性**条件。

**第二步：没有能量，建造无法完成。** 由前提 (iii)，建造需要时间且期内结构须维持自身。若 $E_{\mathrm{build}}>E_{\mathrm{available}}$，建造要么无法启动，要么中途停止；停止时的中间形态通常功能不全（半成品的眼睛提供低质量信号却照样消耗维持成本），故在 $V$ 上低于跃迁前。这是“失败后比原点更差”。能量可用性因而是**可行性**条件。

**第三步：没有杠杆，跃迁即使发生也不被保留。** 若新解码器的 $V$ 不高于旧解码器，则在假设 (ii) 下，携带新解码器的谱系在竞争中处于劣势；即使偶然出现，也会在后续筛选中被淘汰。杠杆条件因而是**合意性**条件。

三步给出一个分工：可能性、可行性、合意性，分别对应“有没有对象”“有没有资源”“有没有净收益”。

**为何不是充分条件。** 三条同时满足仍可能不跃迁。第一，**概率性**：跃迁需要一次成功的重组事件，而重组是搜索过程，成功率依赖搜索空间规模与结构的可变异程度；条件只保证“值得搜”，不保证“搜到”。第二，**时序性**：信号出现、能量充裕、竞争压力足够这三个窗口未必重合。第三，**竞争性**：同一生态位中若已有其他谱系以更低成本占据，先跃迁者未必胜出。

### 4.6 失败模式分类

三个条件各自对应一类失败，加上“条件满足但边际回报未耗尽”一类，构成四种主要的停留机制。

| 失败模式 | 机制 | 例子 |
| :------- | :----------------------------------- | :-------------- |
| **D-锁死**（本卷型） | 解码器梯度饱和（$\nabla D\to0$，即 $I$ 接近 $I_{\max}$ 后继续展开的边际收益趋零），且 $E_{\mathrm{build}}>E_{\mathrm{available}}$ 阻止跃迁。**同名异义提醒**：卷Ⅳ §3.1 的“D-锁死”指“趋近锁死／衰亡域”（$\mu_{\mathrm{rec}}/\delta_{\mathrm{decay}}$ 接近或小于 1），与本行的“梯度饱和＋预算不足”不是同一机制；本卷这一支可称**梯度锁死**。另：$E_{\mathrm{build}}>E_{\mathrm{available}}$ 一项即下文单列的**能量锁死**，两种锁死可同时成立，报告时须分开。跨卷引用这两种锁死时须带卷号，以免同名异义 | 鲎（四亿五千万年形态基本未变）、失去视觉解码器后的洞穴鱼 |
| **信号缺失** | 当前生态位中无可用信号（$\tilde I_{\mathrm{orig}}$ 长期低于门槛） | 稳定环境中的深海固着生物 |
| **能量锁死** | $E_{\mathrm{build}}$ 超过可动员自由能 $E_{\mathrm{available}}$ | 能量预算保守的变温动物；建造期长于世代长度的陆生大型动物 |
| **杠杆不足** | $L_{\mathrm{lev}}<L_{\mathrm{lev,min}}$：当前解码器仍有正回报，重组不划算 | 高度稳定、资源丰富环境中的生物 |

四者的可观测征兆不同（形态停滞、环境稳定、有变异无建造、边际收益仍高），干预含义随之不同。

***

## 第五章　攀升序列：能量主导权转移

纵观物质组织的历史，每一次重大的复杂度跃迁都对应有效能耗 $E_{\mathrm{eff}}=E_{\mathrm{barrier}}+E_{\mathrm{survival}}+E_{\mathrm{causal}}$ 中主导成分的转移。

### 5.1 “有序”方向的澄清：晶体路线与生命路线

晶体的有序与生命的有序是**两种不同的有序机制**。

晶体的有序靠**平均化**：大量原子占据相同周期位置，由深势垒 $E_{\mathrm{barrier}}$ 被动锁定，可区分构型少而每个极稳定，是**对称性最大化**的有序。生命的有序靠**差异化**：DNA 复制、蛋白质折叠、信号通路各司其职，由持续能量流 $E_{\mathrm{survival}}$ 主动维持，可区分构型多而每个都须持续投入，是**对称性破缺最大化**的有序。两者共享同一套 $V$ 公式，分居双通道两端：

$$
V_{\mathrm{s}}=\frac{I_{\mathrm{struct}}\cdot T_{\mathrm{struct}}}{E_{\mathrm{barrier}}+E_{\mathrm{survival}}}\qquad\text{（晶体型：靠静止存续）} \tag{II-5.1}
$$

$$
V_{\mathrm{c}}=\frac{I_{\mathrm{causal}}\cdot T_{\mathrm{causal}}}{E_{\mathrm{causal}}}\qquad\text{（生命型：靠流动存续）} \tag{II-5.2}
$$

从晶体到生命是**有序机制的切换**。黏性源于两种能量项：$E_{\mathrm{barrier}}$ 一次性锁定，退出而结构仍在；$E_{\mathrm{survival}}$ 持续流量维持，退出即解体。所以复杂化在生命谱系中呈黏性——原因在退出成本高。

**关于“不可逆”的正确表述。** 把这一不对称性写成“生命一旦走上与晶体相反的方向，至今未曾回头”，是把统计倾向写成了普遍必然。本卷的表述是：**在所选样本与观察窗内，已进入主动维持模式的谱系表现出向更高 $E_{\mathrm{causal}}$ 占比演化的统计倾向；回退事件存在但稀少。** 回退的例子：营寄生生活的甲壳类失去复眼与部分神经系统；内共生细菌丢失大量基因、把代谢功能交给宿主。“回头”在机制上完全可能，只是统计上不占多数——回退通常伴随生态位收窄，而收窄又提高灭绝风险。

### 5.2 攀升序列

序列每一级由“关键跃迁＋信息状态＋能量主导＋新能力”四项刻画。它是分类工具，不是时间表：不同谱系在不同时刻跨越同一级，也有谱系永不到达。

| 阶段 | 关键跃迁 | $I$ 状态 | 能量主导 | 新能力 |
| :-------- | :---------- | :------------ | :------------ | :------------- |
| **晶格** | 无机初始秩序 | $I_{\mathrm{struct}}>0$，$\eta_D\approx0$ | $E_{\mathrm{barrier}}$（被动壁垒锁定） | 稳定结构 |
| **有机化学** | 无机 $\to$ 有机 | $I_{\mathrm{struct}}$ 扩展 | $E_{\mathrm{barrier}}+E_{\mathrm{survival}}$（主动维持开始） | 化学多样性 |
| **单细胞** | 分子 $\to$ 自维持 | $I_{\mathrm{struct}}$ 爆发扩展；$I_{\mathrm{net}}$ 出现 | $E_{\mathrm{survival}}+E_{\mathrm{causal}}$（代谢加信息处理） | 自我复制、自创生 |
| **多细胞** | 独立 $\to$ 分工 | $I_{\mathrm{net}}$ 通过通信扩展 | $E_{\mathrm{survival}}+E_{\mathrm{causal}}$（通信成本上升） | 专业化与合作 |
| **神经系统** | 反应 $\to$ 预测 | $I_{\mathrm{net}}$ 指数增长；$T_{\mathrm{pred}}>0$ 出现 | $E_{\mathrm{causal}}$ 份额急剧上升 | 预测与规划 |
| **语言、文明** | 个体 $\to$ 集体记忆 | 新增信息注入；$I_{\mathrm{net}}$ 外化 | $E_{\mathrm{causal}}$ 成为主导成本 | 累积文化知识 |
| **人工计算** | 生物 $\to$ 硅基递归 | $I_{\mathrm{net}}$ 递归爆发 | $E_{\mathrm{causal}}$ 主导；失控风险显现 | 高速学习、递归自我改进 |

**能量主导权转移。** 主导成分从 $E_{\mathrm{barrier}}$（被动，零维护）转到 $E_{\mathrm{survival}}$（主动代谢维持），再转到 $E_{\mathrm{causal}}$（信息处理与预测）。每次转移都增加对供应中断的脆弱性，也提高可达成 $V$ 的上限。此序列描述的是走 $I$ 路线的谱系；选择 $T$、$E$ 路线的谱系同样满足 $\max V$ 原则。

**解码器—执行飞轮。** 更强的解码器提取更多信息，实现更高效的生存行为，扩大可栖息范围，暴露于新信号，产生进一步升级的压力。飞轮受三条件约束：信号耗尽或能量支付能力饱和时停转，系统进入 D-锁死或能量锁死。

**适用边界。** 序列从地球生命史与人类技术史两个样本归纳，其普适性主张只能是“在其他样本中应观察到类似的能量主导权转移”；“向上”只在十亿年量级的窗口内成立，百万年窗口内多数谱系呈现波动与停滞；七级划分是粗粒化产物，粒度应服务于研究问题。

***

## 第六章　规则深度、信息几何与线性排名的局限

### 6.1 为什么线性复杂度排名会失败

“人类比细菌更复杂”在一种意义上对：人类所需的生成规则条数确实更多。错的是给结构赋予单一数值 $I=\log_2\Omega$ 并据此线性排名——不同系统的状态空间不可通约，$\Omega_{\mathrm{crystal}}\ne\Omega_{\mathrm{DNA}}\ne\Omega_{\mathrm{language}}$；把三个空间各自的对数排到一根轴上，是三个不同单位的数字被强行排成一列。本卷因此放弃线性排名，改用坐标。

### 6.2 规则三量坐标系

持久结构的信息组织由三个独立坐标表征。它们是**离散的结构坐标**，与刻画解码器的那组连续轴不是同一组量：前者描述对象本身的生成结构，后者描述主体读取对象的效率。

$$
I\;\longrightarrow\;\left(L_D,\;D_{\mathrm{depth}},\;F_{\mathrm{scale}}\right) \tag{II-6.1}
$$

**规则长度 $L_D$（bit）。** 容差 $\varepsilon_{\mathrm{tol}}$ 下用最紧凑规则集重构对象时，该规则集的编码长度。它与静态深度不同：$L_D$ 度量规则集的**总长度**，$D_{\mathrm{depth}}$ 度量**不可约条数**。对象可以规则很少但每条很长，也可以规则很多但每条很短。

**规则深度 $D_{\mathrm{depth}}$（无量纲）。** 还原对象所需的独立规则条数；静态版本按第 2.4 节的定义，动力学版本是 $1+\#\{\mathcal{T}\}$，报数时须注明版本。

**规模因子 $F_{\mathrm{scale}}$（无量纲）。** 同一条规则被递归展开的次数或尺度跨度；雪花枝晶的 $F_{\mathrm{scale}}$ 很大而深度很低。

三者正交，因此不存在“复杂度总分”。

**构型容量**是该结构在保持同一性或功能前提下所能呈现的可区分构型数的以 2 为底对数（bit）：它衡量“能承载多少种状态”，与“某个具体状态的稀有度”不可相减。它也解释了细菌的表面悖论：细菌是低深度、低维护的可行配置，其 $V$ 可能超过复杂得多的生物体——其 $E_{\mathrm{eff}}$ 极低而分子 $I\cdot T$ 也低，乘积谁大取决于具体读数。

### 6.3 跨域量化的硬性限制

DNA 序列、神经网络参数与社会制度的 $I_{\mathrm{struct}}$ 值，是在不可通约的协议下测量的。**域内**：锁定相同的解码器基底 $D$ 与状态空间 $\Omega$ 时，相对定量比较有效。**跨域**：仅能保证定性结构比较——可以断言神经系统比单细胞生物具有更高的规则深度，而无需声称特定的 $I$ 比率。**禁止**跨域数值排名（如“人脑 $=10^{15}$ bit、细菌 $=10^{6}$ bit”）：没有独立观测能同时检验两个协议下的读数。

### 6.4 测量协议的最低要求

缺任何一条，报出的数值都不应进入跨系统比较：**锁定解码器基底**（$D$ 的类型、$I_{\max}(D)$ 与 $\eta_D$ 的估计方式）、**锁定状态空间**（$\Omega$ 的定义、可区分构型判定规则与离散化粒度）、**锁定容差**（不报容差等于不报数）、**锁定背景**、**锁定窗口**；另须**报区间而非点值**、**分清序数与基数**。

***

## 第七章　演化树没有预定的顶峰

### 7.1 演化是梯度搜索，不是进步

演化是在 $V$ 空间中的梯度搜索：在局部热力学约束下实现更高存续势的结构在统计上更可能存续。没有目标，只有梯度。

第一，规则深度可以减少也可以增加：当维持一个约束层的成本超过其对 $V$ 的贡献时，该层会被脱落。宿主承担代谢负担时，寄生虫简化其形态；光子信号不再携带可用信息时，洞穴鱼失去视觉器官。这些是 $\max V$ 约束下的局部优化，形式化为负拓扑跃迁：

$$
\mathcal{T}^{-}:\quad \Delta D_{\mathrm{depth}}^{\mathrm{dyn}}=-1 \quad\text{当}\quad \frac{\partial V}{\partial D_{\mathrm{depth}}}<0 \tag{II-7.1}
$$

式 (II-7.1) 中的 $-1$ 依赖深度指数的标定假设；未通过检验时，该式只表示“深度下降一个层级”。

第二，演化序列是双向的：

$$
\cdots\xrightarrow{\mathcal{T}}\mathcal{F}\xrightarrow{\mathcal{T}}\mathcal{F}\cdots\qquad(\text{攀升}) \tag{II-7.2}
$$

$$
\cdots\xrightarrow{\mathcal{T}^{-}}\mathcal{F}^{-}\xrightarrow{\mathcal{T}^{-}}\cdots\qquad(\text{简化}) \tag{II-7.3}
$$

$\mathcal{F}^{-}$ 表示“在缩减后的容量下继续递归展开”。方向由 $V$ 梯度决定，不由进步概念决定；任何真实谱系的历史都是两式的交替，交替比例取决于约束几何的变动频率。

### 7.2 人类当前位置

人类是第一个把解码器大规模外化到非生物基质（文字、数学、计算）的生物结构。这代表一次可能与神经系统同等量级的拓扑跃迁：此前规则深度的上限由个体的学习能力与传递带宽决定，此后由集体存储介质的容量与检索效率决定。向人工计算的转变是解码器的进一步外化——下一层解码器的 $E_{\mathrm{build}}$ 正分布于全球计算基础设施中。杠杆条件是否满足，是人工智能发展中核心的开放性实证问题；本卷只给判据与需测量的量：同目标、同窗、同分摊规则下的 $V$ 比较，加建造与对齐成本的完整核算。

这一跃迁揭示了 $I_{\mathrm{struct}}$ 与 $I_{\mathrm{net}}$ 的分野。恐龙在白垩纪末期拥有极高的 $I_{\mathrm{struct}}$ 与可观的 $V_{\mathrm{obj}}$ 存量，但 $I_{\mathrm{net}}$ 极低；当负效信息冲击 $I^{-}$ 超过存量可吸收的规模时，缓冲完全失效——高存量提高的是**抗打击阈值**，不是无限免疫。人类的差异不在 $I_{\mathrm{struct}}$ 更大，而在 $I_{\mathrm{net}}$ 外化带来的**主动重塑 $I^{-}$ 作用方式**的能力。

### 7.3 热力学封顶面：攀升的内生制约

每次跃迁都要求更高的核心**功率密度**（$\mathrm{W/kg}$ 或 $\mathrm{W/cm^2}$），上限由介质的**散热约束** $\dot E_{\mathrm{diss}}^{\max}$（热导率与几何面积共同决定）硬性设定，两个方向各生一个封顶面。

**结构方向：重力税。** 躯体质量增加时，支撑与运动成本占 $E_{\mathrm{struct}}$ 的比例随尺度上升（Galileo 几何缩放）；单位质量的维持功率随质量下降（WBE 代谢标度律 $B\propto M^{3/4}$，亚线性，已在生物域验证）。当 $\Delta E_{\mathrm{survival}}/\Delta I_{\mathrm{struct}}$ 超过弹性阈值，扩大躯体的 $V$ 回报转负。恐龙、大象、大型哺乳动物可能已逼近这条线：继续增加 $I_{\mathrm{struct}}$ 所需的 $E_{\mathrm{build}}$ 超过了可动员预算，能量可用性条件被内生地违反。

**净有效信息方向：散热墙。** 提升功率密度产生废热。每擦除一比特至少释放 $E_{\mathrm{L,bit}}=k_BT_{\mathrm{thermo}}\ln2$（$\mathrm{J/bit}$，Landauer, 1961），废热随处理速率累积，而散热受热导率与几何面积约束。约束的性质须说清：朗道尔界是**每比特擦除的能量下界**，须与擦除速率相乘才得功率；把朗道尔界直接乘上“有效信息处理速率”，等于暗中假设每个处理比特都是不可逆擦除比特。本卷只保留弱形式：给定擦除速率 $\dot I_{\mathrm{erase}}$，$\dot Q_{\mathrm{heat}}\ge E_{\mathrm{L,bit}}\dot I_{\mathrm{erase}}$。

在这一弱形式下：哺乳动物大脑皮层功率密度约 $10\ \mathrm{mW/cm^2}$，先进芯片的功率密度已接近各自封装与冷却方案的极限；突破这面墙需要介质层面的改变（低温计算、光子互连、液冷重构），不是当前架构的迭代优化。这是**工程趋势陈述**，依赖“当前冷却方案”这一条件。

**热力学熔毁墙作为大过滤器（候选推论）。** 若散热瓶颈无法由介质跃迁突破，文明将面临一个硬性门槛：$E_{\mathrm{build}}$ 持续上涨而 $I_{\max}(D_{n+1})$ 的增益趋于饱和，杠杆条件被违反。这可能是“大过滤器”的一种热力学形式；其后果在模型中可导出，但经验上无法检验——只有一个样本。突破它的候选路径，是找到使 $E_{\mathrm{build}}$ 不随深度超线性增长的新物理基底。

### 7.4 外星智能问题

更先进的外星文明不一定更大或更具能量，而将运行在人类解码器无法访问的因果维度上；其探测标志是异常高的组装复杂性。未探测到不等于人类最复杂——也可能只是跃迁所需条件的组合足够罕见。

### 7.5 趋同：约束相同，可行解有限

演化中反复出现趋同：眼睛在不同谱系中独立演化多次；解码器从口传仪式延伸到文字、货币与数字协议。本框架的解释是筛选论证：在有限能量、有限时间与有限信息处理能力下，能以较低代价维持有序结构的构型在统计上更可能存续。这一论证与第二定律相容，但不是它的直接推论。

**机制与目标函数。** 筛选是机制，$\max V$ 是对筛选结果的目标函数式概括（本卷元公设：在给定约束下，被保留下来的结构其存续势不低于被淘汰者），对主动相结构则同时是实际优化的方向。$I/E$ 只是 $V$ 在 $T$ 固定时的局部投影；$T$ 可变时，延长存续时间是另一条路线——部落靠血缘，国家靠制度，企业靠法律拟制，只看 $I/E$ 无法解释国家为何比部落持久，$V$ 可以。局部策略层上，走哪条路线是真实的选择；筛选层不改变标准，只筛选这些选择的后果。

**趋同的是解的类型，不是目的地。** 约束相同、可行解有限，所以趋同；这与“没有预定的顶峰”不矛盾。对未来的定性推断属于候选推论。

***

## 第八章　与现有框架的对话

八个外部框架提供支撑、先例或局部验证，也各自留下本卷要填的缺口。

| 框架 | 为本卷提供的支撑 | 本卷填补的缺口 |
| :---------------- | :--------------------- | :-------------------- |
| 耗散结构理论（Prigogine, 1967） | 确认能量流可在局部产生有序结构，为 $V_{\mathrm{c}}>0$ 从 $V_{\mathrm{c}}=0$ 涌现提供物理基础 | 未处理跨跃迁的信息积累，也未提供解码器演化的动力学 |
| 自催化集（Kauffman, 1993；Eigen, 1971） | 确定单细胞级跃迁在化学层面的条件 | 局限于起源时刻 |
| 代谢标度理论（West, Brown & Enquist, 1997） | 生物域内的精确标度律，可作 $E_{\mathrm{survival}}$ 随质量增长的参考 | 未延伸至跨层级或文化演化 |
| 能量率密度（Chaisson, 2001） | 记录单位质量能量流的单调增加，与能量主导权转移的序列定性吻合 | 能量是必要非充分条件 |
| 自由能原理（Friston et al., 2017） | 描述解码器在固定边界条件下的稳态优化 | 未处理边界本身的消解与重建这一跃迁事件 |
| 组装理论（Cronin & Walker, 2021） | 提供可操作的复杂度度量，可作规则深度的经验代理 | 静态度量；无动力学方程或跃迁条件 |
| 生态热力学（exergy 方法，Jørgensen 一系） | 提供“相对死态的自由能距离”这一生态尺度的序度量，与本卷 $V$ 同属“能量归一化的序” | 不含解码器，也不区分结构通道与因果通道；数值高度依赖死态参照的选择 |
| 恢复力理论（Holling, 1973） | 区分“受扰后能否回到吸引域”与“存量是否稳定”，为锁死态提供外部对照 | 只问能否返回，不度量存量水平，也不解释被压低的稳态 $V^{*}$ |
| 文化演化（Henrich, 2015；Mesoudi, 2011） | 提供传递、选择与累积文化的机制证据，支撑规则深度与跨代累积 | 给传递机制而不给成本核算，无法比较“编译 vs 继承”的能量账 |

**支撑与缺口是同一件事的两面**：框架的聚焦决定其盲区。八个框架不归约为一，它们的侧面可在同一套核算语言下排列，使预测可互相比较——若耗散结构理论预测能量流增加时有序度上升，本卷预测容量饱和后有序度不再上升，两者在同一实验上可分辨。

***

## 第九章　可证伪预测

本章给出六条预测，编号 HⅡ-1 至 HⅡ-6：检验方式须含样本、统计量与判定阈值，反驳条件须是**可观测**的。

**表 9.1　卷Ⅱ的可证伪预测**

| 编号 | 预测 | 检验方式 | 反驳条件 |
| :--- | :-------------- | :------------------------ | :--------------- |
| **HⅡ-1** | 层级跃迁只在三个条件同时满足时发生（必要非充分） | 收集有详细能量预算记录的跃迁案例，逐一核查 $\tilde I_{\mathrm{orig}}$ 是否越门、$E_{\mathrm{build}}<E_{\mathrm{available}}$ 与 $L_{\mathrm{lev}}>L_{\mathrm{lev,min}}$ 是否成立；报告四项可比性前提的核查结果 | 记录到的跃迁中，出现 $E_{\mathrm{build}}>E_{\mathrm{available}}$ 或 $L_{\mathrm{lev}}<L_{\mathrm{lev,min}}$ 而被确认为层级跃迁的案例（排除测量误差与分摊差异） |
| **HⅡ-2** | $E_{\mathrm{causal}}/E_{\mathrm{eff}}$ 在走 $I$ 路线的谱系中呈统计上升倾向 | 同一谱系内对比不同阶段的神经代谢占比（脑重体重比、基础代谢率、脑葡萄糖摄取率），用混合效应模型估计时序斜率，控制体型与温度 | 某谱系后期分配给信息处理的比例显著低于早期，且在多个独立谱系中重复 |
| **HⅡ-3** | D-锁死在统计上先于灭绝事件发生 | 用分支系统学结合化石记录，统计灭绝支系的形态停滞期，与存活姊妹支系比较，用 Mann–Whitney U 检验或生存分析，$n\ge20$ | 灭绝支系的形态停滞期与存活支系无显著差异（$p>0.05$），或停滞期系统性晚于灭绝前兆 |
| **HⅡ-4** | 在锁定解码器基底与状态空间的域内，$\alpha/\gamma>1$ | 同一解码器架构的模型族中，以参数量为 $I$ 的代理、训练算力为 $E_{\mathrm{causal}}$ 的代理，固定 $\varphi$，对 $\ln V=\alpha\ln I-\gamma\ln E+\text{常数}$ 回归，报点估计与区间 | 在满足锁定条件的域内估计出 $\alpha/\gamma\le1$，且区间排除 1 |
| **HⅡ-5** | 负拓扑跃迁优先在 $\partial V/\partial D_{\mathrm{depth}}<0$ 持续一段时间后发生 | 在已有形态简化记录的物种（洞穴鱼、寄生甲壳类）中追踪简化前的维护成本时序（代谢率、器官体积比、基因丢失速率） | 观察到形态简化但维护成本未下降，或简化先于成本变化发生 |
| **HⅡ-6** | 跨尺度同向性：同一环境、同一解码器、同一协议下，$V$ 较低者先瓦解 | 三组对照：（a）同一环境中的晶体与普通岩石；（b）两个孤立聚落，一个持续产生迭代文化；（c）同一组织中两个职能单元，一个产出覆盖成本。先按同一协议标定 $V$ 排序，再检验瓦解先后是否与排序同向 | 在满足同域条件的对照中，$V$ 排序与瓦解先后系统性反向 |

**HⅡ-1 的检验逻辑是排除性的**：三条件既为必要，该预测只能被“违反必要条件的跃迁案例”反驳。**HⅡ-4 是最关键的检验**，但它的因变量 $V$ 不可直接观测，须先操作化：取“单位成本的下游基准分数 × 有效服务时长”为 $V$ 的代理，并报代理与既有神经标度律的对照；**基线 $\alpha=\gamma$ 时该回归无判别力**（基准形式下系数恒为 1，是定义的后果，不是经验规律，见附录 C.2），故检验须在锁定域内、固定 $\varphi$、预注册、报区间并作多重比较校正。若 $\alpha/\gamma\le1$ 在锁定域内成立，“信息投资边际收益最高”这一方向性来源失效。**HⅡ-6 只检验序关系是否同向**，其中 (c) 组最易生测量争议，作辅助证据。

***

## 第十章　开放性问题与局限

未解决的问题分**未完成的推导**（结构已知、步骤缺失）与**未标定的参数**（结构未知、数据缺失）两类：前者需要数学，后者需要测量。概念层面的问题缺的是对问题本身的表述。

### 10.1 未完成的推导

**弹性指数的显式形式未导出。** 两条兑现路径——从朗道尔界、Arrhenius 速率与热涨落推出显式函数，或用独立于 $(I,T,E)$ 的存续后果反推——都未走通。部分进展是把“弹性随温度长什么样”换成“$\alpha/\gamma=1$ 的收支平衡面在哪里”：平衡点可算、可对照（附录 C.2），但尚未与实测转变温度系统对照。

**三条件的充分性缺口未填。** 把概率性、时序性、竞争性形式化需要一个跃迁成功率模型：给定搜索空间规模、可变异程度与能量支付的时序曲线，估计一次重组成功的概率。该模型不存在，故“三条件满足则跃迁以概率 $p$ 发生”写不出来。这是本卷最主要的推导缺口。

**混合系统的全局分析未做。** 参数空间 $(\mu_{\mathcal{F}},\tau_{\mathrm{decay}},I_{\mathrm{eq}},I_{\max},\Delta I_{\mathcal{T}},\tau_{\mathcal{T}})$ 的长期行为有几种定性类型、边界在哪里，均未给出；第 3.3 节的局部平衡点只覆盖连续段。

**$V$ 的可加性与深度标定未独立检验。** 前者需分别测两通道，看合成后的 $V$ 预测存续后果是否优于任一单通道。后者在第 2.4 节给了回归方法但无跨域标定；检验完成前，凡把深度当基数使用的结论（含式 (II-2.6)、式 (II-7.1) 的 $-1$）都带附加条件。

### 10.2 未标定的参数

**$E_{\mathrm{build}}$ 与 $L_{\mathrm{lev,min}}$。** 前者需从化石记录、比较基因组学与发育生物学回溯估计；后者依赖情境（竞争强度、风险偏好、替代方案可得性），可能只是环境的属性。

**$\tau_{\mathrm{decay}}$ 与 $I_{\mathrm{eq}}$。** 前者与温度、势垒、载体的关系须由具体机制给出；后者更难——它是“热背景的无序状态对应的信息量”，而这个参照本身依赖协议。

**通道权重 $\varphi$ 的时变性。** 第 2.2 节要求固定 $\varphi$，但 $\varphi$ 由能量构成决定，而能量构成在演化中显著变化（5.2 节的能量主导权转移即 $\varphi$ 的系统性漂移）。故“固定 $\varphi$”短窗可行、长窗不可行；长窗估计需要显式的 $\varphi(t)$ 模型，该模型未建立。

**$\dot E_{\mathrm{diss}}^{\max}$ 的普适标定。** 散热上限在具体系统中可算，跨系统比较却需统一方案（同一几何假设？同一环境温度？同一冷却方式？）；方案未定，散热墙的定量论证只能停在量级层面。

**附录 C 引用的文献数值。** 线虫 dauer 转变温度、辐射耐受剂量、Arrhenius 外推跨度等本应引现成数据，但本书未取得可核对的出处，**故不列具体数值**；补全前不作定量依据。

### 10.3 概念层面的开放问题

**第一解码器的起源。** 三条件都以“已存在一个能读信号、能算收益的解码器”为前提，而第一个解码器出现时这两个前提都不成立，其出现是极端能量梯度下的涨落，须由前生物化学回答。

**意识的解码效率。** 可精确表述为：存在一个 $I_{\mathrm{latent}}$，它独立于是否有解码器能提取它而存在，而当前的 $\eta_D$ 接近零；解决它等同于构建解码器 $D_{\mathrm{conscious}}$。本卷只指出这一表述使问题成为可操作的研究纲领。

***

## 第十一章　结论

从晶体到文明的持久结构演化，本卷写成三个可核算事实的组合，而不是一个目的论故事。

**方向性的候选来源**：弹性排序 $\alpha/\gamma>1>\beta/\gamma$ 若成立，则信息增长的边际收益高于能量增长的边际成本。它是经验假说，不依赖计量单位；会改变估计值的是操作化定义、代理指标、观察域与拟合模型。

**门槛的结构**：层级跃迁需要候选信号、能量可用性与净收益判据同时满足，分别对应可能性、可行性、合意性，缺一则链条断在那一环；三者齐备，跃迁仍可能因概率、时序与竞争而不发生。这一“必要不充分”的地位是刻意保留的——写成充分条件会使理论更强、更易被证伪，但那种强度是假的。

**升级的后果**：每次跃迁重置可达成存续势的上限，同时抬高维持成本与脆弱性。容量重置改变上限、脉冲增量改变当前值，两者分开记账，避免把未来增长记到当下跃迁的账上。

大多数结构并未攀升：当前解码器饱和、跃迁能量不可用，或竞争环境尚未提出要求，于是在原层级存续，有时长达地质年代。这是其约束几何下的局部最优；细菌在数量、代谢多样性与存续时间上占主导三十余亿年，是最有力的经验支持。

宇宙没有为此过程预定目的地，只有一个梯度（$\max V$ 沿可用信号的方向）和支配任何结构能否跟随它的三个条件。若在锁定域内观察到弹性排序失败、层级跃迁在违反必要条件的情形下被确认发生、或 D-锁死未以高于偶然的统计率先于灭绝出现，本卷核心主张即被削弱或证伪；三者权重不同：排序失败最致命，必要条件被违反次之，D-锁死检验失败最轻。

***

## 附录 A　符号与单位速查表

本表覆盖本卷全部符号（含只出现一次的）；第四列说明其有意义的条件，跨系统比较前须先读。

### A.1 信息

| 符号 | 单位 | 定义 | 适用范围 |
| :------- | :------------ | :-------------------- | :----------------- |
| $I$ | bit | 可区分有序差异总量（父变量） | 裸写默认 $I_{\mathrm{net}}$ |
| $I_{\mathrm{struct}}$；$I_{\mathrm{causal}}$ | bit | 相对背景的结构稀有度；相对对照的效果稀有度 | 须锁背景与容差／须对照设计与同窗 |
| $I_{\mathrm{net}}$ | bit | $\varphi_{\mathrm{s}}I_{\mathrm{struct}}+\varphi_{\mathrm{c}}I_{\mathrm{causal}}$ | 域内校准后 |
| $I_{\mathrm{latent}}$；$I_{\mathrm{active}}$ | bit | 未激活的可恢复因果能力；$\eta_D I_{\mathrm{latent}}$ | 独立于解码器／不与 $I_{\mathrm{net}}$ 换算 |
| $\tilde I_{\mathrm{orig}}$ | bit | $-\log_2\Pr_{B_n}(\varepsilon_{\mathrm{res}}\ge\varepsilon_{\mathrm{obs}})$ | 仅门控，须预注册 |
| $I_{\mathrm{orig}}$；$\Delta I_{\mathcal{T}}$ | bit | 经验证的新增信息；单次跃迁写入量 | 事后确认／只记瞬时增量 |
| $I_{\max}(D)$；$I_{\mathrm{eq}}$ | bit | 解码器容量上限；平衡信息水平 | 跃迁后重置／待标定 |
| $I^{-}$ | bit | 使 $I_{\mathrm{net}}$ 净减的扰动 | 须同量纲 |
| $L_D$ | bit | 最紧凑规则集编码长度 | 须报容差 |
| $\varphi_{\mathrm{s}},\varphi_{\mathrm{c}}$ | 无量纲 | 通道权重，和为 1 | 估弹性须固定 |
| $\Omega$；$B_n$ | — | 状态空间；历史残差分布 | 跨域不可通约／跃迁前冻结 |
| $\varepsilon_{\mathrm{res}}$；$\varepsilon_{\mathrm{tol}}$ | 同预测或重构目标 | 预测残差；重构容差 | 度量须声明／深度与长度敏感 |
| $\alpha_0$；$N$，$m$ | 无量纲；个 | 预注册显著性水平；复测次数与越门阈值 | 与多重比较校正同注册 |

### A.2 能量与功率

| 符号 | 单位 | 定义 | 适用范围 |
| :----- | :------- | :------------------------------ | :-------------- |
| $E_{\mathrm{eff}}$；$E_{\mathrm{struct}}$ | J | 三项能量之和；$E_{\mathrm{barrier}}+E_{\mathrm{survival}}$ | 全篇 |
| $E_{\mathrm{barrier}}$ | J | 势垒成本分摊 | 非势垒高度 |
| $E_{\mathrm{survival}}$；$\dot E_{\mathrm{survival}}$ | J；W | 补偿熵增的主动耗散 | 判据用功率 |
| $E_{\mathrm{causal}}$ | J | 解码器运行能耗 | 主动相 $>0$ |
| $E_{\max}$；$E_{\mathrm{available}}$ | J | 环境供给上限；可动员建造预算 | 非可动员量／条件二判据 |
| $E_{\mathrm{build}}$ | J | 一次性建造成本 | 须报分摊与建造期 |
| $E_{\mathrm{ext}}$ | J | 控制的外部能量流 | 仅附录 B |
| $E_{\mathrm{L,bit}}$ | J/bit | $k_BT_{\mathrm{thermo}}\ln2$ | 仅不可逆擦除 |
| $\Delta U_{\mathrm{barrier}}$ | J（单粒子） | 势垒高度。**只能是单粒子能量**：它只出现在 Arrhenius 指数 $\Delta U_{\mathrm{barrier}}/(k_BT_{\mathrm{thermo}})$ 的分子上，分母是单粒子 $k_B$，写成 J/mol 会使指数差 $N_A$ 倍；若数据以摩尔量给出，先除以 $N_A$，或把分母的 $k_B$ 换成 $R$ | 非 $E_{\mathrm{barrier}}$ |
| $\dot E_{\mathrm{diss}}^{\max}$；$\dot E_{\mathrm{maintain}}$；$\dot E_{\mathrm{available}}$ | W | 散热功率上限；维持信息平均功率；建造期可支付功率 | 由热导率与面积定／限命题 3.1／比 $E_{\mathrm{available}}/\tau_{\mathrm{build}}$ |

### A.3 时间与速率

| 符号 | 单位 | 定义 | 适用范围 |
| :-------- | :-------- | :----------------------- | :----------------- |
| $T$ | s | 存续时间（父变量） | 不得指代下列任一 |
| $T_{\mathrm{struct}}$；$T_{\mathrm{struct}}^{\max}$；$T_{\mathrm{causal}}$ | s | 保持可辨识的存续时间；寿命上界；因果效果可识别时间 | 须报窗口与判据／逐持有者报告 |
| $T_{\mathrm{pred}}$；$T_{\mathrm{env}}$ | s | 预测视界；环境特征时间 | 同单位，可比较 |
| $T_{\min}$ | s | 最小时间步 | 非 $\tau_{\mathcal{T}}$ |
| $T_{\mathrm{thermo}}$ | K | 热力学温度 | 非时间 |
| $\tau_{\mathrm{decay}}$ | s | 衰减时间常数 | 待标定 |
| $\tau_{\mathrm{build}}$ | s | 建造期 | 与世代长度比 |
| $\tau_{\mathcal{T}}$ | s | 最小跃迁间隔 | 防 Zeno 行为 |
| $\lambda_{\mathrm{flip}}$；$\mu_{\mathcal{F}}$ | $\mathrm{s^{-1}}$ | 翻转速率；展开速率参数 | 仅附录 C／域内标定 |

### A.4 存续势、弹性与杠杆

| 符号 | 单位 | 定义 | 适用范围 |
| :----------- | :------------- | :--------------- | :----------------- |
| $V$ | $\mathrm{bit\cdot s/J}$ | $V\approx I\cdot T/E$ | 保留 bit |
| $V_{\mathrm{obj}}$ | $\mathrm{bit\cdot s/J}$ | $V_{\mathrm{s}}+V_{\mathrm{c}}$ | 加号为约定 |
| $V_{\mathrm{s}},V_{\mathrm{c}}$ | $\mathrm{bit\cdot s/J}$ | 两通道存续势 | 被动相／主动相 |
| $V_0$ | $\mathrm{bit\cdot s/J}$ | 归一化基准 | 仅用于 $v=V/V_0$ |
| $\alpha$；$\beta$；$\gamma$ | 无量纲 | $\partial\ln V/\partial\ln I$；$\partial\ln V/\partial\ln T$；$-\partial\ln V/\partial\ln E_{\mathrm{eff}}$ | 单位不变；$\gamma$ 须固定 $\varphi$ |
| $L_{\mathrm{lev}}$；$L_{\mathrm{lev,min}}$ | $\mathrm{(bit\cdot s/J)/J}$ | $\Delta V/E_{\mathrm{build}}$；情境阈值 | 须四条前提；可能非内禀 |
| $\rho_I$ | 无量纲 | $\alpha/\gamma$ | $\rho_I=1$ 为相界 |
| $\rho$ | 无量纲 | 竞争压力指数 | 非 $\rho_I$ |

### A.5 解码器、算子与几何

| 符号 | 单位 | 定义 | 适用范围 |
| :---------- | :---------- | :------------------- | :----------------- |
| $D$ | — | 提取因果信息的机制 | 下标 $n$ 表代际 |
| $\eta_D$ | 无量纲 | 解码效率，$\in[0,1]$ | 非 $\eta_{\lambda}$ |
| $\mathcal{F}$；$\mathcal{F}^{-}$ | — | 多尺度复制不增维度；缩减容量下的展开 | 连续段／简化段 |
| $\mathcal{T}$；$\mathcal{T}^{-}$ | — | 重组结构打开新维度；负拓扑跃迁 | 幅度 $\Delta I_{\mathcal{T}}$ |
| $\#\{\mathcal{T}\}$ | 个 | 跃迁累计次数 | 深度构成量 |
| $\lambda_{\mathcal{F}}$；$S_n$ | — | 展开算子控制参数；第 $n$ 代状态 | $\mathcal{T}$ 为其跳变／式 (II-2.5) |
| $D_{\mathrm{depth}}$；$D_{\mathrm{depth}}^{\mathrm{dyn}}$ | 无量纲 | 最少不可约规则数；$1+\#\{\mathcal{T}\}$ | 随机构型取 0／仅深度 $\ge1$ 有定义 |
| $F_{\mathrm{scale}}$ | 无量纲 | 展开次数或尺度跨度 | 与深度正交 |
| 构型容量 | bit | 可呈现构型数取对数 | 非单状态稀有度 |
| $k_B$；$\ln 2$ | J/K；无量纲 | 玻尔兹曼常数；约 0.6931 | 下界计算与比特换算 |
| $\Pr$；$P$ | — | 概率函数；概率分布 | 二者不互换 |
| $\lambda_{\mathrm{civ}}$；$\eta_{\lambda}$；$\lambda_{\mathrm{civ,opt}}$ | 无量纲 | $E_{\mathrm{ext}}/E_{\mathrm{causal}}$；其倒数；使 $\partial V/\partial\lambda_{\mathrm{civ}}=0$ 的值 | 仅附录 B |
| $T_{\mathrm{thermo,c}}$ | K | 切换温度 | 不可跨物种比 |

凡带“须报”字样的量，报数时须同时报出协议参数；本表不含价值权重。

***

## 附录 B　文明能量杠杆扩展（应用级辅助参数）

本附录的量只用于策略分析；与核心判据冲突时以核心判据为准。

### B.1 能量二分

总能耗拆为 $E_{\mathrm{causal}}$（解码器直接消耗）与 $E_{\mathrm{ext}}$（解码器控制的外部能量流）。**文明能量杠杆**为

$$
\lambda_{\mathrm{civ}}\equiv\frac{E_{\mathrm{ext}}}{E_{\mathrm{causal}}}. \tag{II-B.1}
$$

$\lambda_{\mathrm{civ}}$ 无量纲，两侧须是同一观察窗内的积分量——一积分一功率是最常见的量纲错误。其倒数 $\eta_{\lambda}$ 称控制效率。

### B.2 最优杠杆面

保持 $V=IT/E_{\mathrm{eff}}$ 不变，令 $E_{\mathrm{eff}}=E_{\mathrm{causal}}(1+\lambda_{\mathrm{civ}})$（**本附录把 $E_{\mathrm{struct}}$ 并入 $E_{\mathrm{ext}}$；与核心式 $E_{\mathrm{eff}}=E_{\mathrm{struct}}+E_{\mathrm{causal}}$ 冲突时以核心式为准**）。扩张对 $I$ 与 $T$ 的作用相反：$I$ 随杠杆增加，$T$ 随其缩短。记 $T=T_0f(\lambda_{\mathrm{civ}})$，$f'<0$，则

$$
V\left(\lambda_{\mathrm{civ}}\right)=\frac{I\left(\lambda_{\mathrm{civ}}\right)\cdot T_0\cdot f\left(\lambda_{\mathrm{civ}}\right)}{E_{\mathrm{causal}}\left(1+\lambda_{\mathrm{civ}}\right)}. \tag{II-B.2}
$$

**【命题 B.1（最优杠杆面的存在）】**
- **前提**：（i）$I(\lambda)$ 连续可微且单调不减；（ii）$f(\lambda)$ 连续可微、单调递减、恒正；（iii）$I$ 的增长率随 $\lambda$ 递减；（iv）$\dfrac{\mathrm{d}\ln(If)}{\mathrm{d}\lambda_{\mathrm{civ}}}$ 在 $\lambda_{\mathrm{civ}}\to0^{+}$ 时大于 1，且在 $\lambda_{\mathrm{civ}}\to\infty$ 时小于 $\dfrac{1}{1+\lambda_{\mathrm{civ}}}$。
- **结论**：在 (i)–(iv) 下，$V$ 在 $(0,\infty)$ 上存在内部驻点，且满足

$$
\frac{\partial\ln I}{\partial\lambda_{\mathrm{civ}}}+\frac{\partial\ln T}{\partial\lambda_{\mathrm{civ}}}=\frac{1}{1+\lambda_{\mathrm{civ}}}. \tag{II-B.3}
$$

- **推导**：对式 (II-B.2) 取对数，$\ln V=\ln I+\ln T_0+\ln f-\ln E_{\mathrm{causal}}-\ln(1+\lambda)$，求导置零即得。
- **依赖的假设**：驻点存在依赖前提 (i)。若扩张不增加信息，式 (II-B.3) 左端恒负而右端为正，$V$ 单调下降，扩张在任何规模上都是净损失。
- **失效条件**：（a）$I$ 的增长率不递减时最优在边界；（b）$f$ 在 $\lambda_c$ 处触零时最优退化为退化点；（c）须验二阶条件并与 $V(0)$ 比较。

一阶条件的读法是：**扩张的信息增益率与寿命损失率之和，等于能量分母的相对增长率**。

### B.3 文明相变判据（E 相与 T 相）

按 $\mathrm{d}\lambda_{\mathrm{civ}}/\mathrm{d}t$ 与 $\mathrm{d}V/\mathrm{d}t$ 的符号可分出四格：扩张期（E 相，两者皆正，如工业革命与算力爆发）、饱和期（皆约零，杠杆停滞）、休眠期（T 相，杠杆降而 $V$ 升，以杠杆换寿命）与真实衰退（皆负，结构崩溃）。四格是分类而非轨迹：$\dot\lambda_{\mathrm{civ}}<0$ 不必然等于衰退，真实文明可以往返。

### B.4 历史核算基线

概念性量级估算，四舍五入到一位有效数字：$E_{\mathrm{causal}}\approx1.3\times10^{21}\ \mathrm{J}$；$E_{\mathrm{eff}}\approx3.2\times10^{22}\ \mathrm{J}$；由此 $E_{\mathrm{eff}}/E_{\mathrm{causal}}=\lambda_{\mathrm{civ,avg}}+1\approx25$，即 $\lambda_{\mathrm{civ,avg}}\approx24$。$V_{\mathrm{civ}}$ 另需同口径的 $I$ 与 $T$，本节不报数。

量级校验：$E_{\mathrm{ext}}\approx3.1\times10^{22}$ J 与 $E_{\mathrm{eff}}=3.2\times10^{22}$ J 同量级，故 $\lambda_{\mathrm{civ}}\approx24$。

***

## 附录 C　三温区、跨期策略与工程投影（应用层候选推论）

> 本附录把已确立的热力学约束映射到存续策略上，不发现新物理。涉及弹性随温度变化的全部排序均为**候选推论**。$T_{\mathrm{thermo}}$ 为温度（K），$T_{\mathrm{env}}$ 为环境特征时间（s），不可混用。所引文献数值（线虫 dauer 转变温度、辐射耐受剂量、Arrhenius 外推跨度）本书未列可核对出处，补全前不作定量依据。

### C.1 温度如何调制三个维度

三个机制方向不一致：朗道尔下界 $E_{\mathrm{L,bit}}=k_BT_{\mathrm{thermo}}\ln2$ 使升温后单比特擦除更贵；Arrhenius 速率 $\lambda_{\mathrm{flip}}\propto e^{-\Delta U_{\mathrm{barrier}}/k_BT_{\mathrm{thermo}}}$ 使降温后反应更慢；热涨落尺度 $\propto k_BT_{\mathrm{thermo}}$ 使高温下结构更脆。因此不存在单调的“越好”，只有权衡。

### C.2 弹性指数的价值判定

基准形式 $V=IT/E$ 展开后弹性恒等于 1，这是定义的后果；一般形式 $V\propto I^{\alpha}T^{\beta}/E^{\gamma}$ 才承载 $\alpha/\gamma>1>\beta/\gamma$ 的经验主张，把前者当作后者的证据是循环论证。两条兑现路径都未走通——从朗道尔、Arrhenius 与热涨落推出具体形式，或用独立于 $(I,T,E)$ 的存续指标反推；共同前提是**独立锚**：没有 $V$ 的可观测后果约束其函数形式，$\alpha,\beta,\gamma$ 只是自由参数。目前只部分兑现：锚是 $\rho_I=1$ 的收支平衡面，切换温度 $T_{\mathrm{thermo,c}}$ 可算，绝对位置不可信。

弹性还取决于系统与环境的耦合：环境改变三项的相对成本，载体决定势垒、速率与存储密度，能量构成决定投向，解码器决定 $I$ 的提取效率；“弹性随温度”是只考虑第一层时的简写。**外部对照**：England 的耗散驱动适应与本框架同源，它预测低温有源系统加速耗散，本框架预测信息路线占优，两者在机制上可判别（England 的原文未列入本书参考文献，此处只作定位，不作论据）。

### C.3 弹性反转条件与认知相区间

$$
\rho_I\equiv\frac{\alpha}{\gamma}=\frac{\partial\ln V/\partial\ln I}{-\partial\ln V/\partial\ln E_{\mathrm{eff}}}. \tag{II-C.1}
$$

$\rho_I=1$ 定义的是**该系统类型的认知相区间边界**，不是“生命的区间”。

| 条件 | 相态 | 路线 |
| :---------------- | :-------------------- | :--------------------- |
| $\rho_I\gg1$ | 主动认知相，高回报 | $I$ 路线占优 |
| $\rho_I$ 略大于 $1$ | 主动认知相，回报刚够 | $T$ 或 $E$ 路线 |
| $\rho_I=1$ | 相变面 | — |
| $\rho_I<1$ | 被动相 | 无路线；只有热力学筛选 |

$\rho_I=1$ 有两种读法：**存在性门**与**路线分界**。松树、海龟、寄生虫仍有解码器，只是把更多能量投向延长 $T_{\mathrm{struct}}$ 或降低 $E_{\mathrm{eff}}$。主动认知相须同时满足 $\rho_I>1$ 与 $T_{\mathrm{pred}}$ 可持续；$T_{\mathrm{pred}}$ 的延伸会增加 $E_{\mathrm{causal}}$、增大 $\gamma$、压缩 $\rho_I$，故延伸本身收紧认知相区间。各系统各有自己的 $\rho_I=1$ 曲面。

### C.4 三道边界：主动认知相的完整条件

$\rho_I>1$ 不是唯一条件。结构必须还在、认知必须付得起、动力学必须来得及。

| 条件 | 物理含义 | 不满足的后果 | 松紧 |
| :----------- | :--------------- | :-------------- | :--------------- |
| 结构完整性 | 物理载体不散架 | 结构解体，直接消亡 | **最紧**：多数生物撞上的墙 |
| 认知可负担性 | 开销不超预算 | 退化为被动相 | 很松 |
| 动力学可行性 | 反应速率不低于决策速率 | 冻结，来不及有效行为 | 视温度 |

这解释了辐射致死的反直觉现象：人类约 5 Gy 全身照射致死，死因是 DNA 与细胞完整性崩溃，即结构先散架，而非“认知系统失效”。水熊虫耐受剂量高出若干数量级（具体倍数未列可核对出处，待标定），机制是换相：自由水被抽干，结构变成极难被辐射破坏的构型，换相之后也不再保有主动认知相。

### C.5 三温区框架

| 温区 | 主导特征 | 候选弹性倾向 | 相态与路线 | 策略本质 |
| :----------- | :-------- | :------------ | :----------- | :------------ |
| 低温无源 | 静态保存 | 信息弹性高但无法兑现 | $\rho_I<1$，被动相 | 冻结，等待 |
| 低温有源 | 慢速处理 | 信息弹性仍可较高 | $\rho_I$ 略大于 $1$，$T$、$E$ 路线 | 用时间换信息 |
| 中温（约 0–30 °C） | 均衡 | $\alpha/\gamma>1>\beta/\gamma>0$（候选） | $\rho_I\gg1$，$I$ 路线 | 又快又贵 |
| 高温 | 结构难维持 | 信息弹性可能下降 | $\rho_I<1$，被动相 | 倾向节能 |
| 极高温 | 仅引力结构 | — | $\rho_I<1$，被动相 | 无小尺寸化学键智慧体 |

**低温区的分叉点是自由能通量，不是温度本身。** 低温加有源时每比特代价极低、单位能量可处理巨量信息，但运算时钟被拉长；中温区那一行的排序是该温区的候选实例，若排序在别的温区反向，不证伪排序本身（其范围是“锁定域内”）。

### C.6 跨期存续与休眠策略

**单期 $V$ 无法表达休眠。** 休眠是跨期决策：关闭动态处理、保存结构，等未来窗口打开再激活。补全形式为：跨期存续势＝当期结构通道项＋折扣后的未来因果期权的期望值。当期项是维持最低物理完整性的能耗，折扣因子受环境不确定性、载体老化率与外部威胁概率影响；这是概念结构而非可计算量。三个温区的典型影响：深冷保存区结构消耗极低，但苏醒能耗高、响应延迟大；弹性缓冲区通常是全局较优区间，保留基础修复与较快响应；常温活跃区因果效力最大，当期消耗最高，长期暴露加速退化。

**四个模式系统**（本节是整合与重新解读，不是新实验；各系统的具体数值本书未列可核对出处，一律待标定）：线虫 dauer（高温加食物匮乏，单阶段跨期）、水熊虫 tun（缓慢脱水，单阶段跨期加形成成本，关键参数是脱水速率阈值）、孢子萌发（温度窗口，单阶段跨期，有上下限阈值）、种子休眠（多阶段温度与湿度信号，**多阶段跨期序列**，各阶段温时不同）。

共同结构：系统在自由能通量或温度偏离适宜窗口时关闭动态处理、保存结构、等待未来窗口。各系统的切换温度不可跨物种比较。

### C.7 时间感知推论（候选）

不同温区智慧体的内部反应速率受 Arrhenius 约束，主观时间尺度与客观时间可能严重不匹配：低温有源者单次思考深，但需长期休眠、交流困难；高温者单次思考浅、寿命短，难以积累文明；中温居中。主观时间取决于预测步数而非客观秒数，所以跨物种比较只能用客观 $T_{\mathrm{pred}}$，预测步数只在同一物质基底内可比。低温有源才可能形成“偶尔醒来的智慧体”，低温无源是休眠体，不是智慧体。相关的宇宙学推论（例如对费米悖论的解释）目前没有观测证据，且与“文明演化主要发生在恒温环境”这一取向冲突，本卷不展开，也不列入可证伪内容。

### C.8 工程投影：火种存续温度

“火种存续温度”是同一框架在文明延续与星际场景下的工程投影，是随技术水平、载体材质、能源功率密度与轮换周期变化的动态优化结果：它把传统认知中固定的生理参数，变成可调的控制变量。三条红线：温度只是多个控制变量之一，不能单独决定策略；任何表述须注明相对于哪个解码器；属应用层推论，不得与本体论核心概念混用。物理约束上，温度太高则保存成本高，太低则细胞内结冰，复温太快产生冰晶、太慢则代谢无法恢复，故适宜区间是一个窄窗口，位置与宽度须逐系统标定，不给绝对数值。

### C.9 可检验预测与当前缺口

以下七条为 HⅡ-7 至 HⅡ-13，三列含义与正文一致。

| 编号 | 预测 | 检验方式 | 反驳条件 |
| :---- | :----------------- | :----------------- | :------------------ |
| **HⅡ-7** | 低温有源系统单位能量的信息产出高于中温系统，单位客观时间的产出更低 | 低温量子计算装置与常温装置的能耗—产出对照，报每焦耳与每秒有效操作数 | 单位能量产出不高于中温系统（同类任务、同精度） |
| **HⅡ-8** | 高温区不应出现以复杂化学键为基础的智慧体 | 对高温行星大气做分子多样性普查，检验复杂度与温度的相关性 | 在高温环境中发现以多步化学键级联维持的复杂信息处理结构 |
| **HⅡ-9** | 排序反转的临界温度可由收支平衡面计算 | 写出 $\rho_I=1$ 的显式收支条件，再算 $T_{\mathrm{thermo,c}}$ 的标度关系 | 平衡面算出的临界温度与实测转变温度标度不符（差一个数量级以上且方向不一致） |
| **HⅡ-10** | 休眠转变温度与收支平衡面的交点对应 | 线虫 dauer、孢子萌发的温度阈值拟合，与预测交点比较 | 转变温度与交点系统偏离，且不能由载体参数差异解释 |
| **HⅡ-11** | 主动休眠的 $T_{\mathrm{thermo,c}}$ 受 $E_{\mathrm{build}}$ 调制 | 比较不同脱水速率下水熊虫 tun 的形成成功率与温度阈值 | 改变 $E_{\mathrm{build}}$ 而 $T_{\mathrm{thermo,c}}$ 完全不动 |
| **HⅡ-12** | 多阶段休眠每阶段有独立的 $T_{\mathrm{thermo,c}}$ | 分别拟合种子胚根与胚轴阶段的温度阈值 | 两阶段阈值统计上不可区分 |
| **HⅡ-13** | 自由能通量越低，$T_{\mathrm{thermo,c}}$ 应越低 | 比较不同食物供应条件下的 dauer 转变温度 | 通量与转变温度无相关，或方向相反 |

**暂缓条目（不编号）**：低温、高温智慧体的信号形态与时间尺度不匹配导致的交流困难，属宇宙学方向，本卷暂缓展开，不列入可证伪内容。

**当前缺口**：弹性指数随温度的显式函数（部分改由收支平衡面承担）；$T_{\mathrm{thermo,c}}$ 的绝对位置（标度关系可用）；Arrhenius 外推可靠性；可测量代理与跨温区可比规则（未建立）；休眠结构的数据整合（未做）；与 r-K 选择理论的划界（未处理）。缺口补齐前不给出弹性指数随温度的启发式函数形式：没有数据锚的函数形式是伪精确。

***

## 参考文献

1. Prigogine, I. (1967). *Introduction to Thermodynamics of Irreversible Processes* (3rd ed.). Interscience.
2. Kauffman, S. A. (1993). *The Origins of Order*. Oxford University Press.
3. Kauffman, S. A., & Roll, W. (2024). Is the emergence of life an expected phase transition in the evolving universe? *Interface Focus*, 14, 20230085.
4. West, G. B., Brown, J. H., & Enquist, B. J. (1997). A general model for allometric scaling laws in biology. *Science*, 276(5309), 122–126.
5. Chaisson, E. J. (2001). *Cosmic Evolution*. Harvard University Press.
6. Friston, K., FitzGerald, T., Rigoli, F., Schwartenbeck, P., & Pezzulo, G. (2017). Active inference: A process theory. *Neural Computation*, 29(1), 1–49.
7. Cronin, L., & Walker, S. I. (2021). Defining lyfe in the universe. *Life*, 11(12), 1284.
8. Eigen, M. (1971). Selforganization of matter and the evolution of biological macromolecules. *Naturwissenschaften*, 58(10), 465–523.
9. Landauer, R. (1961). Irreversibility and heat generation in the computing process. *IBM Journal of Research and Development*, 5(3), 183–191. https://doi.org/10.1147/rd.53.0183
10. Bekenstein, J. D. (1973). Black holes and entropy. *Physical Review D*, 7(8), 2333–2346.
11. Gould, S. J., & Eldredge, N. (1977). Punctuated equilibria. *Paleobiology*, 3(2), 115–151.
12. Schneider, E. D., & Kay, J. J. (1994). Life as a manifestation of the second law. *Mathematical and Computer Modelling*, 19(6–8), 25–48.
13. Ashby, W. R. (1956). *An Introduction to Cybernetics*. Chapman & Hall.
14. Wiener, N. (1948). *Cybernetics: Or Control and Communication in the Animal and the Machine*. MIT Press.
15. Shannon, C. E. (1948). A mathematical theory of communication. *Bell System Technical Journal*, 27(3), 379–423. https://doi.org/10.1002/j.1538-7305.1948.tb01338.x
16. Ulanowicz, R. E. (1986). *Growth and Development*. Springer.
17. Haken, H. (1983). *Synergetics: An Introduction* (3rd ed.). Springer.
18. Mann, H. B., & Whitney, D. R. (1947). On a test of whether one of two random variables is stochastically larger than the other. *Annals of Mathematical Statistics*, 18(1), 50–60. https://doi.org/10.1214/aoms/1177730491
19. Holling, C. S. (1973). Resilience and stability of ecological systems. *Annual Review of Ecology and Systematics*, 4, 1–23. https://doi.org/10.1146/annurev.es.04.110173.000245
20. Henrich, J. (2015). *The Secret of Our Success: How Culture Is Driving Human Evolution, Domesticating Our Species, and Making Us Smarter*. Princeton University Press.
21. Mesoudi, A. (2011). *Cultural Evolution: How Darwinian Theory Can Explain Human Culture and Synthesize the Social Sciences*. University of Chicago Press.

***

<!-- VOLUME Ⅲ ｜ 压缩智能与认知演化：离线编译计算、人类因果增量与物理嵌入的边界 -->
## 卷Ⅲ　压缩智能与认知演化：离线编译计算、人类因果增量与物理嵌入的边界

> **本卷＝卷Ⅲ。**

## 摘要

硅基智能近十年的能力增长走的是同一条路：把更多的在线计算换成更好的输出。这条路有两处尽头：热，与数据。本卷回答三个问题：在线搜索为什么存在一个不能靠继续加算力越过的上限；把搜索提前编译进结构在什么条件下划算；在这一格局里**物理嵌入系统**的功能位置是什么。具身 AI 属于物理嵌入一侧，不受本章“瓶颈”说法的约束——本章区分的是“接入物理信道”与“封闭数字系统”，不是“碳”与“硅”。

方法分三层。**物理下界**：朗道尔原理给出的是逻辑不可逆擦除的每比特能量下界 $E_{\mathrm{L,bit}}=k_BT_{\mathrm{thermo}}\ln2$，不是“每比特处理”的下界；二者之间隔着一个必须显式声明的映射 $\beta_{\mathrm{erase}}$，故产热下界写作 $\dot E_{\mathrm{heat}}\ge k_BT_{\mathrm{thermo}}\ln2\cdot\dot I_{\mathrm{erase}}$。**模型内的最优性**：把“何时编译、编译多少”写成带线性切换的两阶段最优控制问题，成本先无量纲化（**能量预算约束在此模型中不影响 $u^{*}$**，见 §8.1.2）。原以 $R\equiv C_{\mathrm{comp}}/E_{\mathrm{build}}>1$ 作判据；但 $R$ 不出现在该最优控制的泛函里，故 **$R>1$（且 $N_{\mathrm{eff}}\ge2$）只是单次预算回收的充分条件，既不是最优性判据，也不是可负担性判据**——可负担性另写 $E_{\mathrm{build}}<E_{\mathrm{available}}$（§8.1.5）。§8.1.5 实际给出的判据是单切换策略的一阶条件；由此得到的 bang-bang 结构是【命题】而非【定理】。**待检验的假说**：物理嵌入性溢价、创新不确定性、内卷锁死、热力学红皇后效应，各自给出可测后果与否证条件。

主要结论按强度排列。**【定理】** 朗道尔下界及其速率形式，适用域为逻辑不可逆擦除。**【命题】** 从产热到损伤需净热流、热容温升、散热曲线、剂量累积四步，缺一步结论不成立。**【命题】** 编译最优性至多切换一次。**【命题】** 固定架构下展开饱和后净增长率转负，但 $V$ 有正上界 $T_{\mathrm{causal}}/k_{\mathrm{m}}$。**【命题】** 合成数据退化：$N_{1/e}=-1/\ln\mathcal{R}_{\mathrm{gen}}$ 在 $\mathcal{R}_{\mathrm{gen}}=0.5/0.7/0.75/0.8$ 时为 $1.44/2.80/3.48/4.48$ 代，“3—5 代”对应 $0.75$—$0.80$。**【假说】** 创新成功率不高于随机基准需要统计决策模型才能陈述。**【命题】** 散热壳层比 $\Sigma\ge L_{\min}^{2}\rho_{s}e_{s}/(\kappa\Delta T\tau_{\mathrm{op}})$，缺 $L_{\min}$ 则无正下界。

**边界声明。** 其一，本卷不主张任何宇宙学意义上的信息总量界限；人类可用数据量是特定人口、寿命、感官速率与编码效率假设下的窗口估计。其二，$V$ 是描述性框架，不构成规范性判据。其三，“智能”限于可观测的信息处理与结构固化。其四，除标注来源的数值外，全篇数字均为量级估计。其五，§8.6 的切换次数界代入典型参数为 $3.5\times10^{14}$，现实前提不成立，只作失效登记，不列为主结果。

**关键词**：结构递归存续动力学；离线编译计算；朗道尔下界；擦除映射；散热约束；合成数据退化；人类因果增量

**Abstract.** Over the past decade, the growth in the capabilities of silicon-based intelligence has followed a single path: converting more online computation into better output. This path has two dead ends: heat, and data. This volume answers three questions: why online search has an upper limit that cannot be crossed by adding more computing power; under what conditions compiling search into structure ahead of time pays off; and what the functional position of **physically embodied systems** is within this configuration. Embodied AI belongs to the side of physical embedding and is not bound by the "bottleneck" claim of this chapter — the distinction drawn in this chapter is between "access to a physical channel" and "a closed digital system", not between "carbon" and "silicon".

The method has three layers. **The physical lower bound**: Landauer's principle gives an energy lower bound per bit of logically irreversible erasure, $E_{\mathrm{L,bit}}=k_BT_{\mathrm{thermo}}\ln2$, not a lower bound per bit "processed"; between the two lies a mapping $\beta_{\mathrm{erase}}$ that must be declared explicitly, so the lower bound on heat production is written $\dot E_{\mathrm{heat}}\ge k_BT_{\mathrm{thermo}}\ln2\cdot\dot I_{\mathrm{erase}}$. **Optimality within the model**: "when to compile and how much to compile" is written as a two-stage optimal control problem with linear switching, with costs first made dimensionless (**the energy budget constraint does not affect $u^{*}$ in this model**, see §8.1.2). The criterion was originally taken to be $R\equiv C_{\mathrm{comp}}/E_{\mathrm{build}}>1$; but $R$ does not appear in the functional of this optimal control, so **$R>1$ (together with $N_{\mathrm{eff}}\ge2$) is only a sufficient condition for one-time budget recovery, and is neither an optimality criterion nor an affordability criterion** — affordability is written separately as $E_{\mathrm{build}}<E_{\mathrm{available}}$ (§8.1.5). What §8.1.5 actually gives is the first-order condition of the single-switch policy; the bang-bang structure obtained from it is a **Proposition** rather than a **Theorem**. **Hypotheses to be tested**: the physical-embedding premium, innovation uncertainty, involution lock-in, and the thermodynamic Red Queen, each of which gives measurable consequences and falsification conditions.

The main conclusions are ordered by strength. **Theorem**: the Landauer bound and its rate form; the domain of validity is logically irreversible erasure. **Proposition**: from heat production to damage requires four steps — net heat flow, heat-capacity temperature rise, dissipation curve, and dose accumulation — and if any one is missing the conclusion does not hold. **Proposition**: optimal compilation switches at most once. **Proposition**: once unfolding saturates under a fixed architecture, the net growth rate turns negative, but $V$ has a positive upper bound $T_{\mathrm{causal}}/k_{\mathrm{m}}$. **Proposition**: synthetic-data degradation: $N_{1/e}=-1/\ln\mathcal{R}_{\mathrm{gen}}$ equals $1.44/2.80/3.48/4.48$ generations at $\mathcal{R}_{\mathrm{gen}}=0.5/0.7/0.75/0.8$, and "3–5 generations" corresponds to $0.75$–$0.80$. **Hypothesis**: that the innovation success rate is no higher than a random baseline can be stated only with a statistical decision model. **Proposition**: the thermal-shell ratio $\Sigma\ge L_{\min}^{2}\rho_{s}e_{s}/(\kappa\Delta T\tau_{\mathrm{op}})$; without $L_{\min}$ there is no positive lower bound.

**Scope statement.** First, this volume asserts no cosmological bound on the total amount of information; the amount of data available to humans is a window estimate under assumptions about a specific population, lifespan, sensory rate, and encoding efficiency. Second, $V$ is a descriptive framework and does not constitute a normative criterion. Third, "intelligence" is limited to observable information processing and structure consolidation. Fourth, except for values with a cited source, all numbers throughout are order-of-magnitude estimates. Fifth, the bound on the switching count in §8.6 evaluates to $3.5\times10^{14}$ at typical parameters, a value for which the real-world premises fail; it is recorded only as a failure registration and is not listed as a main result.

**Keywords**: Structure Recursive Viability Dynamics; offline-compiled computation; Landauer bound; erasure map; heat-dissipation constraint; synthetic-data degradation; human causal increment

***

## 第一章　暴力计算的热力学极限与物理散热约束

在线算力存在一个不能靠继续加算力越过的上限。本章先给出朗道尔下界的严格形式与适用域，再把它从“每比特能量”升为“功率”，然后补上从功率到损伤之间常被跳过的两个环节——擦除映射与热学链条，最后逐环列出失效条件。全章只有一个【定理】，其余都是【命题】。

### 1.1 四个核心量：存续势、净信息、解码器与算子

持久结构（persistent structure，PS）指在观察窗内保持可辨识同一性的物理组织，如晶体、细胞、人、组织。本卷只处理**主动相**的一类：必须持续摄入自由能、持续排出废热才能维持低熵状态。被动相结构（岩石、建筑骨架）的存续势由势垒决定，不在讨论范围。

主动相结构维持存续要做两件事：从环境提取**因果信息**，并把提取结果**固化**为自己的结构。前者在线、耗能、逐次支付；后者离线、一次性、可复用。这一对动作的转换称为**离线编译**，转换完成后的状态称为**离线编译计算态**。

**存续势 $V$** 是单位能量成本换取的信息与时间之积：

$$
V=\frac{I\cdot T}{E} \tag{III-1.1}
$$

量纲为 $\mathrm{bit\cdot s/J}$。它是“每焦耳换到多少比特·秒”的效率读数；保留 bit 因子，因为信息通道与能量通道在 $V$ 中分开记账，只有归一化后的 $v=V/V_{0}$ 才无量纲。

**式 (III-1.1) 是本卷使用的低阶基准形式。** 双通道定义 $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ 及二者的数值关系见卷Ⅰ §3.2：同一组对称参数下两式可相差 4 倍。本卷只在要求量级与序关系处使用 (III-1.1)，不与双通道值互相代入，也不据 (III-1.1) 报绝对数值。

**净有效因果信息 $I_{\mathrm{net}}$** 是按能量份额合成的粗粒化指数：

$$
I_{\mathrm{net}}=\varphi_{\mathrm{s}}I_{\mathrm{struct}}+\varphi_{\mathrm{c}}I_{\mathrm{causal}},\qquad \varphi_{\mathrm{s}}=\frac{E_{\mathrm{struct}}}{E_{\mathrm{eff}}},\quad \varphi_{\mathrm{c}}=\frac{E_{\mathrm{causal}}}{E_{\mathrm{eff}}},\quad \varphi_{\mathrm{s}}+\varphi_{\mathrm{c}}=1 \tag{III-1.2}
$$

$I_{\mathrm{struct}}$ 与 $I_{\mathrm{causal}}$ 各有读数协议与背景，二者都以 bit 计并不构成可加性的证明。该合成指数只有在同一读数协议、同一背景、同一观察窗并完成域内校准时才可作数值使用，否则只提供序关系。未加下标时，“有效因果信息”指 $I_{\mathrm{causal}}$ 这一路可测通道，“净有效因果信息”指式 (III-1.2) 的合成量。

**解码器 $D$ 与规则深度 $D_{\mathrm{depth}}$**。解码器是把环境信号映射为内部状态的装置，可以是神经回路、一套理论、一段程序、一个组织的惯例。规则深度分两个用法：静态深度是**定义**，即指定容差内还原对象所需的最少独立规则条数；动态写法 $D_{\mathrm{depth}}^{\mathrm{dyn}}=1+\#\{\mathcal{T}\}$ 是**深度指数**，“每次拓扑跃迁恰好增加一条独立规则”是标定假设而非定义推出的等式。标定方法是用静态深度对跃迁次数做回归；斜率显著不为 1 时，深度指数只作序数使用。

**两个算子。** 递归展开 $\mathcal{F}$ 在同一套规则内多尺度复制、加密、放大，不改变规则集本身；拓扑跃迁 $\mathcal{T}$ 在吸收外部信号后重组规则集、打开新的因果维度。算力堆叠属于 $\mathcal{F}$，范式改变属于 $\mathcal{T}$。

本卷不回答四个问题：第一个解码器的起源；意识的机制（谈“自我”只指可观测的自我表征与自我评估响应）；跨域的绝对定量；具体技术路线的时间表（年份与代际数均为量级示意）。

### 1.2 证据等级与记号约定

结论按四级标签标注强度。标签是承诺：标【定理】的必须给出完整推导，标【假说】的不许在结论章被当作已证事实使用。

| 标签 | 使用条件 | 必须附带 |
| :---------- | :------------------------------- | :---------------- |
| **【定理】** | 前提明确列出；卷内结论须推导完整，引用前人已证结果时不要求卷内重证，但须注明原始出处与该处前提——两者不得混标 | 前提、结论、证明或出处、适用域 |
| **【命题】** | 有形式化陈述，但前提部分待标定，或某一步依赖未证的建模假设 | 前提、结论、依赖的假设、失效条件 |
| **【候选推论】** | 由某命题在附加条件下导出，未独立检验 | 母命题、附加条件、可测后果 |
| **【假说】** | 经验性或机制性猜测，无形式化推导 | 陈述、支持理由、证伪条件 |

记号约定全卷遵守，附录 A 汇总。信息族中裸写 $I$ 默认指 $I_{\mathrm{net}}$，两个可测通道一律写全 $I_{\mathrm{struct}}$、$I_{\mathrm{causal}}$；候选范式突破信号记 $\tilde I_{\mathrm{orig}}$，经验证的新增信息记 $I_{\mathrm{orig}}$。时间族 $T_{\mathrm{struct}}$、$T_{\mathrm{causal}}$、$T_{\mathrm{pred}}$、$T_{\min}$、$T_{\mathrm{env}}$ 五者不得互换；$T_{\mathrm{thermo}}$ 为温度，不入时间族。能量族存量用 $E$、功率一律 $\dot E$，不用 $P$ 以免与概率混淆。$\dot I_{\mathrm{erase}}$ 专指逻辑不可逆擦除速率，$\dot I_{\mathrm{active}}$ 专指当前处理速率。代际序号一律下标，如 $I_{\mathrm{net},n}$、$D_{n+1}$。

### 1.3 朗道尔下界：严格形式、适用域与速率形式【定理】

**定理 1.1（朗道尔下界）**

- **前提**：（i）被擦除的 $n$ 比特逻辑状态在操作前等概率分布于 $2^{n}$ 个构型；（ii）操作把该分布映到单一构型，即逻辑不可逆；（iii）操作与温度为 $T_{\mathrm{thermo}}$ 的热库接触，过程准静态；（iv）热库温度在操作期间恒定。
- **结论**：操作向热库排放的热量满足 $E_{\mathrm{heat}}\ge n\,k_BT_{\mathrm{thermo}}\ln2$，等号在可逆极限取得。
- **证明**：逻辑态数从 $2^{n}$ 降到 $1$，信息熵减少 $n$ bit，对应热力学熵减少 $n k_B\ln2$。总熵不降，环境熵至少增加同量，故 $E_{\mathrm{heat}}\ge T_{\mathrm{thermo}}\Delta S_{\mathrm{env}}\ge n k_BT_{\mathrm{thermo}}\ln2$；等号取在准静态、无额外熵产的过程。
- **适用域**：只对**逻辑不可逆**操作成立。可逆计算把擦除推迟到必须丢弃信息的那一刻，操作本身不触发下界，只在最终清空时一次性支付。

失效条件有三条。初态不是等概率分布时，“逻辑不可逆”未必对应“热力学不可逆”——若初态偏离最大熵，擦除可利用这部分自由能，实际排热可低于下界，这不构成反例，因为前提（i）已破。操作远非准静态时熵产增加，下界仍成立但不再紧。若“比特”的载体是连续变量（模拟计算、神经膜电位），“每比特擦除”需另行定义。

把定理 1.1 除以时间，得到本卷真正要用的形式。设 $\dot I_{\mathrm{erase}}$ 为可计量的逻辑不可逆擦除速率（$\mathrm{bit/s}$），则

$$
\dot E_{\mathrm{heat}}\ \ge\ k_BT_{\mathrm{thermo}}\ln2\ \cdot\ \dot I_{\mathrm{erase}} \tag{III-1.3}
$$

式 (III-1.3) 是全卷热力学论证的起点：左边是功率（$\mathrm{W}$），右边是“每比特能量”乘“比特每秒”，量纲闭合。它**没有**说“处理一比特就要付 $k_BT\ln2$”，因为处理与擦除不是同一件事。

### 1.4 从处理速率到擦除速率：映射必须先声明【命题】

把“有效信息处理速率” $\dot I_{\mathrm{active}}$ 直接乘上 $k_BT\ln2$ 得到产热功率，等于假定每处理一比特恰好发生一次不可逆擦除——这个假定既未被定义，也未被任何架构验证。本卷把它拆成两步。第一步定义**擦除映射系数**

$$
\beta_{\mathrm{erase}}\ \equiv\ \frac{\dot I_{\mathrm{erase}}}{\dot I_{\mathrm{active}}} \tag{III-1.4}
$$

单位为“擦除比特每处理比特”，无量纲。它是**架构参数**：取决于指令集、寄存器重用策略、存储层次、是否就地计算、是否允许可逆门。同一块芯片跑不同负载，$\beta_{\mathrm{erase}}$ 可差两三个数量级。第二步定义**非理想耗散因子** $\xi\ge1$，表示实际每擦除比特耗散是朗道尔下界的多少倍：

$$
\xi\ \equiv\ \frac{E_{\mathrm{diss,bit}}}{k_BT_{\mathrm{thermo}}\ln2} \tag{III-1.5}
$$

于是产热功率写成

$$
\dot E_{\mathrm{heat}}\ =\ \xi\,\beta_{\mathrm{erase}}\,k_BT_{\mathrm{thermo}}\ln2\ \cdot\ \dot I_{\mathrm{active}}\ \equiv\ \nu_{\mathrm{diss}}\,k_BT_{\mathrm{thermo}}\ln2\ \cdot\ \dot I_{\mathrm{active}} \tag{III-1.6}
$$

其中 $\nu_{\mathrm{diss}}\equiv\xi\beta_{\mathrm{erase}}$ 是两个系数的乘积：一个来自“做了多少次擦除”，一个来自“每次擦除多不理想”。把它当作介质的固有属性，就是把两个不同来源的因子压成了一个数。

**命题 1.1（处理速率不可直接代入朗道尔式）**

- **前提**：$\dot I_{\mathrm{active}}$ 已由声明的读数协议测得；$\beta_{\mathrm{erase}}$ 与 $\xi$ 未独立标定。
- **结论**：不得由式 (III-1.3) 直接写出 $\dot E_{\mathrm{heat}}\ge k_BT_{\mathrm{thermo}}\ln2\cdot\dot I_{\mathrm{active}}$。可写出的最强陈述是式 (III-1.6)，其中 $\nu_{\mathrm{diss}}$ 为待标定量；在 $\beta_{\mathrm{erase}}$ 未知时，该式只提供“实测产热除以实测处理速率”这一事后比值，不提供任何事前下界。
- **依赖的假设**：处理与擦除在时间上可分离计数；两套读数协议的计数口径不冲突。
- **失效条件**：若擦除与处理不可分离（模拟存内计算中状态更新与信息读出是同一物理过程），$\beta_{\mathrm{erase}}$ 无定义，本命题与式 (III-1.6) 均不适用，只能改用“每焦耳有效操作数”这类整体指标。

实践含义是：比较两种架构的能效之前，先问清“比特”指什么——指一次晶体管开关、一次 32 位浮点乘加、还是一次注意力读写，得到的 $\nu_{\mathrm{diss}}$ 相差六到八个数量级。

### 1.5 从产热功率到结构损伤：四步链条【命题】

“产热功率超过散热功率，于是系统等效热力学成本接近解体阈值，于是结构损伤”——这条推理跳过了四步：热量积累导致温升、温升由热容决定、温升被散热曲线钳制在某个稳态、损伤由温度对时间的积分决定。

**第一步，净热流。** 设内部产热功率 $\dot E_{\mathrm{heat}}(t)$、向环境排热功率 $\dot E_{\mathrm{diss}}(T_{\mathrm{thermo}})$，则净流入系统的热功率为

$$
\Phi(t)\ =\ \dot E_{\mathrm{heat}}(t)\ -\ \dot E_{\mathrm{diss}}\bigl(T_{\mathrm{thermo}}(t)\bigr)\qquad(\mathrm{W}) \tag{III-1.7}
$$

只有 $\Phi>0$ 时系统才积累热量。比较 $\dot E_{\mathrm{heat}}>\dot E_{\mathrm{diss}}^{\max}$ 是充分条件而非必要条件，对应 $\Phi$ 在 $T_{\mathrm{thermo}}$ 达到许用上限时仍为正的极端情形。

**第二步，热容与温升。** 设等效热容 $C_{\mathrm{th}}$（$\mathrm{J/K}$），则

$$
C_{\mathrm{th}}\frac{\mathrm{d}T_{\mathrm{thermo}}}{\mathrm{d}t}\ =\ \Phi(t) \tag{III-1.8}
$$

热时间常数 $\tau_{\mathrm{th}}\equiv R_{\mathrm{th}}C_{\mathrm{th}}$（$R_{\mathrm{th}}$ 为热阻，$\mathrm{K/W}$）是功率阶跃后温度升到稳态值 $63\%$ 所需的时间，**任何短于 $\tau_{\mathrm{th}}$ 的功率尖峰都不会造成相应的温升**：这一条足以否证“功率超限即损伤”的即时版本。

**第三步，散热曲线。** 排热功率随温度上升而增加，最简形式为线性导热与辐射两项之和：

$$
\dot E_{\mathrm{diss}}(T_{\mathrm{thermo}})\ =\ \frac{T_{\mathrm{thermo}}-T_{\mathrm{thermo,env}}}{R_{\mathrm{th}}}\ +\ \varepsilon_{\mathrm{em}}\sigma_{\mathrm{SB}}A\left(T_{\mathrm{thermo}}^{4}-T_{\mathrm{thermo,env}}^{4}\right) \tag{III-1.9}
$$

其中 $\varepsilon_{\mathrm{em}}$ 为发射率、$\sigma_{\mathrm{SB}}$ 为斯特藩—玻尔兹曼常数、$A$ 为辐射面积。稳态工作点由 $\dot E_{\mathrm{heat}}=\dot E_{\mathrm{diss}}(T_{\mathrm{thermo,ss}})$ 给出，线性区近似为 $\Delta T_{\mathrm{thermo,ss}}=R_{\mathrm{th}}\dot E_{\mathrm{heat}}$；存活与否取决于 $T_{\mathrm{thermo,ss}}$ 是否低于材料许用温度 $T_{\mathrm{crit}}=T_{\mathrm{env}}+\Delta T_{\mathrm{thermo,crit}}$。

**第四步，剂量累积。** 材料损伤是温度历史的泛函而非瞬时函数，常用阿伦尼乌斯剂量：

$$
D_{\mathrm{dose}}(t)\ =\ \int_{0}^{t}\exp\!\left[-\frac{E_{a}}{k_BT_{\mathrm{thermo}}(t')}\right]\mathrm{d}t' \tag{III-1.10}
$$

$E_{a}$ 为损伤过程的激活能（$\mathrm{J}$），$D_{\mathrm{dose}}>D_{\mathrm{crit}}$ 时结构发生不可逆退化。等价的能量表述是累计净热量

$$
Q_{\mathrm{net}}\ =\ \int_{0}^{t}\Phi(t')\,\mathrm{d}t' \tag{III-1.11}
$$

超过阈值 $E_{\mathrm{thresh}}$。两式不是同一个判据：前者对温度高度非线性（温度每升 $10\ \mathrm{K}$ 寿命约减半，这是电子器件的经验规律），后者只看总热量。本卷取式 (III-1.10) 为主判据，式 (III-1.11) 作量级估计。

**命题 1.2（从功率超限到结构损伤）**

- **前提**：（i）$\Phi(t)>0$ 的持续时间超过 $\tau_{\mathrm{th}}$；（ii）稳态温升超过许用值，$R_{\mathrm{th}}\dot E_{\mathrm{heat}}>\Delta T_{\mathrm{thermo,crit}}$；（iii）观察窗内剂量累积达到 $D_{\mathrm{dose}}>D_{\mathrm{crit}}$；（iv）损伤不可逆且无主动修复。
- **结论**：四条同时满足时 $E_{\mathrm{eff}}>E_{\mathrm{thresh}}$，结构发生不可逆退化，$V$ 的下降由损伤项（与超额有效能量成正比）给出；缺任一条，“功率超限”只造成可恢复温升或根本不造成温升。
- **依赖的假设**：$R_{\mathrm{th}}$ 在温升范围内近似恒定；损伤可加（Miner 线性累积）；冷却控制回路不介入。
- **失效条件**：（a）功率尖峰短于 $\tau_{\mathrm{th}}$，热容吸收；（b）相变吸热或主动制冷把 $T_{\mathrm{thermo,ss}}$ 拉回许用值以下；（c）系统有降频、降精度、任务迁移等自由度，能在 $\Phi$ 转正后自动削减 $\dot E_{\mathrm{heat}}$；（d）材料在该温区损伤饱和，$D_{\mathrm{dose}}$ 不再增长。

**命题 1.3（在线算力的热力学天花板）**

- **前提**：架构固定（$\beta_{\mathrm{erase}}$、$\xi$ 不随负载改变）；散热几何固定（$R_{\mathrm{th}}$、$A$ 不变）；任务所需处理速率随环境状态空间规模单调上升。
- **结论**：存在处理速率上限 $\dot I_{\mathrm{active}}^{\max}=\allowbreak\dot E_{\mathrm{diss}}^{\max}/(\xi\beta_{\mathrm{erase}}k_BT_{\mathrm{thermo}}\ln2)$，超过它的任务无法在该架构上以在线方式完成；此时只有三条出路——降低任务所需速率（改变策略）、改变架构（降低 $\xi\beta_{\mathrm{erase}}$）、把部分处理转为离线（降低 $\dot I_{\mathrm{active}}$ 而保持输出质量）。
- **依赖的假设**：状态空间规模与所需处理速率同向增长；架构参数在观察窗内稳定。
- **失效条件**：若 $\beta_{\mathrm{erase}}$ 可通过算法或架构大幅下调（可逆计算、存内计算、稀疏激活），天花板随之移动；若任务可分解为大量低速率子任务并行，天花板不再是单一数值。

第三条出路正是本卷的主题。离线编译是在命题 1.3 的约束下把 $\dot I_{\mathrm{active}}$ 换成 $I_{\mathrm{struct}}$ 的唯一系统性手段。

### 1.6 硅基架构的标定示例（示意）

“当前硅基芯片 $\nu_{\mathrm{diss}}$ 通常在 $10^{2}$—$10^{4}$”这句话没有说明比特指什么，无法核对。取 $T_{\mathrm{thermo}}=300\ \mathrm{K}$，则

$$
E_{\mathrm{L,bit}}\ =\ 1.381\times10^{-23}\times300\times0.693\ \approx\ 2.87\times10^{-21}\ \mathrm{J/bit} \tag{III-1.12}
$$

换算结果取决于“一比特”的口径：绝热或可逆逻辑门约 $10^{-18}\ \mathrm{J}$（$\nu_{\mathrm{diss}}\sim3\times10^{2}$）；先进节点单次晶体管开关 $10^{-16}$—$10^{-15}\ \mathrm{J}$（$3\times10^{4}$—$3\times10^{5}$）；32 位浮点乘加约 $10^{-12}\ \mathrm{J}$（$\sim3\times10^{8}$）；一次内存往返约 $10^{-11}\ \mathrm{J}$（$\sim3\times10^{9}$）。

可见 $10^{2}$—$10^{4}$ 落在**最下沿**，对应理想化低功耗器件；以常规 CMOS 开关口径计在 $10^{4}$—$10^{5}$，以浮点口径计在 $10^{8}$ 以上。$\nu_{\mathrm{diss}}$ 随口径变化六个数量级以上，是“架构＋负载＋计数口径”的联合标定值。实际系统中最大的耗散来源往往是**数据搬运**（末一项）：若搬运主导能耗，“把中间结果固化到离计算更近的位置”本身就是降低 $\beta_{\mathrm{erase}}$ 的路径。

**在线计算有一个由散热决定的天花板，天花板的高度是架构与口径的函数；把计算搬到离线，是移动天花板而不是撞天花板。** 搬多少、何时搬、搬过去有无别的代价，需要另做带约束的核算。

## 第二章　离线编译计算与专家认知的物理学

把在线搜索改写成离线结构，省下的是步数而不是单步成本，代价是一次性的建造支出与分布漂移时的误配风险。

### 2.1 演化压缩机制【命题】

设解码器 $D$ 尚未对外部信道形成有效偏置，则每次决策都必须对高维状态空间做显式搜索，单次决策的因果处理能量是瞬时功率在搜索时间上的积分：

$$
E_{\mathrm{causal}}\ =\ \int_{0}^{T_{\mathrm{search}}}\dot E_{\mathrm{causal}}(t)\,\mathrm{d}t \tag{III-2.1}
$$

$T_{\mathrm{search}}$ 为搜索时间（$\mathrm{s}$），$\dot E_{\mathrm{causal}}$ 为瞬时因果处理功率（$\mathrm{W}$）。无偏置时潜在状态空间规模为 $\Omega$，搜索时间随 $\Omega$ 增长：暴力搜索的成本主要来自步数多。离线编译改变的是步数：规则深度增加、历史约束层叠加，把 $\Omega$ 压成有效子空间 $\Omega'\ll\Omega$，搜索时间缩短到最小响应时间 $\tau_{\min}$：

$$
E_{\mathrm{causal}}^{\mathrm{compressed}}\ =\ \int_{0}^{\tau_{\min}}\dot E_{\mathrm{causal}}(t)\,\mathrm{d}t\ \approx\ \dot E_{\mathrm{base}}\,\tau_{\min} \tag{III-2.2}
$$

**命题 2.1（演化压缩）**

- **前提**：（i）偏置使有效状态空间从 $\Omega$ 收缩到 $\Omega'$，收缩比对同类任务稳定；（ii）搜索时间随有效空间规模单调不减；（iii）单步功率 $\dot E_{\mathrm{base}}$ 不随规则深度显著上升；（iv）偏置的维持成本低于它节省的搜索成本。
- **结论**：单次决策的积分能耗随规则深度单调下降，并以 $\dot E_{\mathrm{base}}\tau_{\min}$ 为下界：

$$
\lim_{D_{\mathrm{depth}}\to\infty}E_{\mathrm{causal}}^{\mathrm{compressed}}\ \to\ E_{\mathrm{floor}},\qquad E_{\mathrm{floor}}\ \ge\ \dot E_{\mathrm{base}}\,\tau_{\min} \tag{III-2.3}
$$

- **依赖的假设**：环境分布在编译前后同分布；偏置可迁移到未见过的同类任务。
- **失效条件**：（a）环境非平稳，旧偏置失效，压缩收益被误配成本吃掉；（b）维持成本失控，深规则需要持续刷新；（c）单步功率随深度上升，抵消步数收益；（d）状态空间不可压缩（对抗性环境、密码学式随机性）。

第（d）条解释了离线编译在棋类、影像诊断、语言上有效而在密码分析、彩票预测上无效：不是方法不对，是被压缩对象没有可压缩结构。前提（iii）在实践中也常不成立，此时净收益取决于两个因子：

$$
\frac{E_{\mathrm{causal}}^{\mathrm{compressed}}}{E_{\mathrm{causal}}^{\mathrm{search}}}\ =\ \underbrace{\frac{\tau_{\min}}{T_{\mathrm{search}}}}_{\text{步数比}}\ \times\ \underbrace{\frac{\dot E_{\mathrm{base}}}{\dot E_{\mathrm{causal}}}}_{\text{单步功率比}} \tag{III-2.4}
$$

只要步数比的下降快于单步功率比的上升，压缩净收益为正。

### 2.2 离线编译计算态的定义

**定义 2.1（离线编译计算态）** 一个持久结构处于离线编译计算态，当且仅当同时满足三条：（i）其解码器对特定环境类 $I_{\mathrm{latent}}$ 的提取效率达到该介质上限的显著比例（工程上取 $\eta_{D}\ge0.8\,\eta_{\max}$）；（ii）式 (III-2.4) 的比值小于 $1$；（iii）在线搜索时间为数倍 $\tau_{\min}$ 的量级。定义不含心理学词汇：系统在特定任务类上把大部分计算搬进了结构。

围棋是常用例证：专家在熟悉棋型上快速判断，认知科学称之为组块化（Chase & Simon, 1973）——用本卷的语言，把 $I_{\mathrm{causal}}$ 沉积为 $I_{\mathrm{struct}}$。其限度是：快速判断只在熟悉棋型上成立，准确性来自反馈闭环，且快与准是两个独立维度。**命题 2.1 说明的是能耗的压缩，不是正确性的提升**：一个被高效编译的错误规则比慢速搜索更危险，因为它省掉了纠错所需的在线时间。

### 2.3 热力学红皇后效应：策略趋势【假说】

**假说 2.1（热力学红皇后效应）** 在长期竞争中存活下来的高级智能系统，其策略组合中离线拓扑结构的占比随时间上升，在线穷举计算的占比下降。支持理由：环境因果范围扩大时 $\Omega$ 的增长快于 $E_{\max}$ 的增长，纯在线路线会先撞上命题 1.3 的天花板；离线结构可复制；竞争惩罚慢决策。反对理由更强：离线结构会过时，在线搜索具有适应性，二者互补而非替代。故立场是：在环境平稳、任务重复、反馈可靠的三重条件下，离线占比上升是可观测的趋势；条件不满足时趋势可以反转。

***

## 第三章　艺术与科学：跨主体解码器编译器

一件作品如何在另一个人的头脑里改变其解码器，这种改变能否用同一个存续势框架核算，“看不懂”与“看懂了”在物理上是什么区别。

### 3.1 艺术与科学价值的存续势方程

艺术作品与科学理论适用同一个表达式：

$$
V_{\mathrm{art}}\ =\ \frac{I_{\mathrm{net}}\cdot T_{\mathrm{cultural}}}{E_{\mathrm{eff,art}}} \tag{III-3.1}
$$

三项需要逐一落实，否则这个式子只是把 $V=IT/E$ 换了下标。**$I_{\mathrm{net}}$（bit）** 是作品传递给特定受众的净有效因果信息；对科学它包括解释范围与预测精度，对艺术它包括可被感知的结构复杂度与信息密度，二者读数协议不同，不能直接比较。**$T_{\mathrm{cultural}}$（s）** 是作品保持可辨识、可被引用的持续时间，不是物理载体的寿命（石碑可以存续三千年而无人阅读）。**$E_{\mathrm{eff,art}}$（J）** 由建造与解码两部分构成：

$$
E_{\mathrm{eff,art}}\ =\ E_{\mathrm{build}}\ +\ E_{\mathrm{causal,audience}} \tag{III-3.2}
$$

两项之和是至少两方的账，这意味着该指标隐含一个社会总账的核算边界；跨群体比较时必须显式声明谁付建造、谁付解码、按什么规则分摊。优秀作品的共同点是压缩率高（$F=ma$ 是三个字符承载一个力学体系），但压缩率高与价值高不是同义词：本卷只提供结构复杂度的度量，不提供价值排序。

### 3.2 规则深度与艺术层级的分析框架

分析工具是规则深度 $D_{\mathrm{depth}}$，即在容差 $\varepsilon_{\mathrm{tol}}$ 内还原对象所需的最少独立规则条数。容差放宽则条数下降，故任何数值都必须带容差；动态写法 $D_{\mathrm{depth}}^{\mathrm{dyn}}=1+\#\{\mathcal{T}\}$ 作定量自变量前必须先做回归校准。高深度作品在构图、色彩、透视、符号隐喻等维度上各叠加独立规则：

$$
\text{画面结构}\ =\ \text{构图层}\ \times\ \text{色彩层}\ \times\ \text{透视层}\ \times\ \text{符号层} \tag{III-3.3}
$$

乘号不是修辞：各层约束同时生效，任一层缺失都会使整体不可还原——这就是独立规则的操作含义。层数增加不必然带来 $V$ 的增加：收益是 $I_{\mathrm{net}}$ 上升，成本是建造这一层的一次性能耗与受众解码这一层的额外能耗之和；后者超过前者时，深度增加反而降低 $V$（8.4 节给出内点最优）。

### 3.3 跨主体解码器编译器机制【命题】

艺术创作与科学发现可读作一次跨主体的因果网络改写，四个环节各自可以单独失败：创造者把规则与候选突破信号压缩进载体；载体送达受众时，其既有解码器的提取效率接近零：

$$
D_{n}\bigl(\tilde I_{\mathrm{orig}}\bigr)\ \approx\ 0 \tag{III-3.4}
$$

信号随后可能触发拓扑跃迁，使解码器升级：

$$
D_{n+1}\bigl(\tilde I_{\mathrm{orig}}\bigr)\ \gg\ 0 \tag{III-3.5}
$$

升级后的解码器在未来同类任务上的积分能耗下降，下降量即这次编译的社会收益。

**命题 3.1（作品作为跨主体编译器）**

- **前提**：（i）载体承载的规则可被受众的既有认知偏置部分匹配（存在可对齐的先验）；（ii）受众支付的解码能耗在能量预算之内；（iii）信号强度足以越过注意阈值；（iv）受众有反馈机会以校准解码结果。
- **结论**：在四条前提下，作品可使受众的解码器发生一次拓扑跃迁，从而降低其未来同类任务的处理能耗；社会净收益为所有受众节省的能耗之和减去建造与传输成本。
- **依赖的假设**：跃迁一旦发生即稳定；节省的能耗可在观察窗内累积。
- **失效条件**：（a）先验不可对齐，受众缺少必要的中间概念，信号被读成噪声（这是“看不懂”的一种，与“太深”不同）；（b）解码能耗超出预算，受众在完成解码前放弃；（c）信号强度不足，作品从未进入注意范围；（d）无反馈，跃迁后无法校准，形成系统性误读，能耗不降反升。

第（d）条最易忽略：一次误读若被稳定下来，会成为一层错误的深偏置，此后每次调用都在支付错误的成本；用式 (III-3.1) 的语言，这类作品的 $T_{\mathrm{cultural}}$ 很高而 $I_{\mathrm{net}}$ 的符号与预期相反。因此机制是概率性的、双向的、有成本的：**艺术与科学的功能是改变接收端的结构；改变结构需要接收端支付能量；支付了能量不一定得到结构，可能得到误构。**

## 第四章　人类因果增量的分析框架

在一个硅基算力持续扩张的系统里，**物理嵌入系统**是否还有一个不可被替代的功能位置；如果有，能否把它写成可核算的量，而不是一句价值宣言。

### 4.1 混合动力系统与封闭系统的自指退化【命题】

结构信息的演化不能写成带狄拉克 $\delta$ 的单一方程：连续增长、事件跳变、容量重置是三笔不同的账。**连续段**在当前 $D$ 不变时服从

$$
\frac{\mathrm{d}I}{\mathrm{d}t}\ =\ \mathcal{F}(D,I)\ -\ \frac{I-I_{\mathrm{eq}}}{\tau_{\mathrm{decay}}} \tag{III-4.1}
$$

$\mathcal{F}(D,I)$ 在固定规则内产生新组合，并显式依赖 $I$：同一套规则在信息量接近容量上限时，能产生的新组合必然减少。**跳跃映射**在跃迁时刻为

$$
I\bigl(t_{\mathrm{jump}}^{+}\bigr)\ =\ I\bigl(t_{\mathrm{jump}}^{-}\bigr)\ +\ \Delta I_{\mathcal{T}},\qquad I_{\max}(D_{n+1})\ >\ I_{\max}(D_{n}) \tag{III-4.2}
$$

脉冲项记信息量的瞬时增加，容量重置记可提取上限的改变，二者不得重复计数：$\Delta I_{\mathcal{T}}$ 是实际写入的比特数，$I_{\max}$ 的新旧差是打开的容量空间。

**命题 4.1（封闭系统的自指退化）**

- **前提**：（i）系统封闭，无外部候选信号注入（$\tilde I_{\mathrm{orig}}\equiv0$，因而 $\Delta I_{\mathcal{T}}=0$）；（ii）$\mathcal{F}(D,I)$ 的边际增益随 $I$ 上升递减，并在 $I_{\max}(D)$ 处为零；（iii）衰减系数 $1/\tau_{\mathrm{decay}}>0$ 且不随时间下降。
- **结论**：存在稳定平衡 $I^{*}\in(I_{\mathrm{eq}},I_{\max})$（$F$ 为 logistic 型时唯一）：$I>I^{*}$ 时 $\mathrm{d}I/\mathrm{d}t<0$；闭合递归系统长期收敛到 $I^{*}$，不是 $I_{\mathrm{eq}}$。若希望结论落在 $I_{\mathrm{eq}}$，须另加前提 $F(I_{\mathrm{eq}})=0$（最简形式 $F\equiv0$），此时 $I^{*}=I_{\mathrm{eq}}$——这是一个不同模型，不是本命题的弱化。
- **依赖的假设**：$\mathcal{F}$ 的形式在观察窗内不变；衰减不可被内部机制逆转。
- **失效条件**：（a）存在外部判据（棋类规则、编译器、证明检查器），系统可借交互生成新信息，此时 $\tilde I_{\mathrm{orig}}>0$，封闭前提破；（b）存在外部记忆或回放，等效于 $\tau_{\mathrm{decay}}$ 大幅延长；（c）架构改变使 $I_{\max}$ 上升；（d）系统能构造新的可验证子问题，形式上等价于（a）。

棋类自博弈在“没有人类数据”的意义上封闭，但棋盘规则是外部判据，数据自产而真值外供，故不属自指退化。纯合成数据上的多代训练已被报告出现分布尾部消失与罕见事件遗忘（Shumailov et al., 2024），用本卷的语言即 $\mathcal{R}_{\mathrm{gen}}<1$ 的代际累积（8.8.3 节）。

### 4.2 人类因果增量：物理嵌入性的功能位置【假说】

定义主观评估与客观状态之间的偏差，其演化写成一阶弛豫加噪声驱动：

$$
\Delta_{\mathrm{VV}}\ \equiv\ \bigl|V^{\mathrm{virt}}-V_{\mathrm{obj}}\bigr|,\qquad
\frac{\mathrm{d}\Delta_{\mathrm{VV}}}{\mathrm{d}t}\ =\ -\alpha_{\mathrm{L}}\,I_{\mathrm{net}}\,\Delta_{\mathrm{VV}}\ +\ \sigma \tag{III-4.3}
$$

$\alpha_{\mathrm{L}}$ 为学习率，$\sigma$ 为噪声强度（$\mathrm{bit/J}$），稳态解为

$$
\Delta_{\mathrm{VV}}^{*}\ =\ \frac{\sigma}{\alpha_{\mathrm{L}}I_{\mathrm{net}}} \tag{III-4.4}
$$

偏差的稳态值是噪声与学习能力的比值。物理信道的噪声 $\sigma_{\mathrm{phys}}$ 含热涨落、机械扰动与他者行为，不可完全建模；数字信道的 $\sigma_{\mathrm{dig}}$ 可纠错，二者在同等算力下可差若干数量级。碳基系统因必须维持肉身持续暴露于前者：

$$
\begin{aligned}
\Delta_{\mathrm{VV}}^{(\mathrm{carbon})}(t)\ &\longrightarrow\ \Delta_{\mathrm{VV}}^{*}>0,\\
\Delta_{\mathrm{VV}}^{(\mathrm{silicon})}(t)\ &\longrightarrow\ \Delta_{\mathrm{VV}}^{*,\,(\mathrm{silicon})}<\Delta_{\mathrm{crit}}
\quad(\sigma_{\mathrm{dig}}>0，只是未越阈)
\end{aligned}
\tag{III-4.5}
$$

**从偏差到信号。** 采用唯象映射

$$
\dot I_{\mathrm{orig}}\ =\ \kappa_{\mathrm{orig}}\,\Delta_{\mathrm{VV}}\cdot\mathbf{1}\bigl[\Delta_{\mathrm{VV}}\ge\Delta_{\mathrm{crit}}\bigr] \tag{III-4.6}
$$

$\Delta_{\mathrm{crit}}$ 为触发跃迁的最小偏差，$\kappa_{\mathrm{orig}}$ 为转换系数（$\mathrm{J/s^{2}}$）；指示函数设置死区：偏差小于阈值时系统有偏差但没有修正压力。

**假说 4.1（物理嵌入性溢价）** 在 $\kappa_{\mathrm{orig}}$ 与 $I_{\mathrm{net}}$ 相当、且 $\Delta_{\mathrm{VV}}^{*,(\mathrm{carbon})}\ge\Delta_{\mathrm{crit}}>\Delta_{\mathrm{VV}}^{*,(\mathrm{silicon})}$ 的条件下，碳基系统的候选信号产生率为正、高于纯数字系统；后者在模型内恰为 $0$（分母 $\dot I_{\mathrm{orig}}^{(\mathrm{silicon})}=0$ 使“比值”无定义，故本假说只作方向比较，不给比值）。

- **证伪条件**：封闭数字环境中运行的 AI，其经独立评定的新颖信息产出密度不低于同规模人机混合系统；或物理噪声强度与候选信号产生率无显著正相关。
- **已知的反例压力**：纯数字系统可通过主动实验设计人为引入噪声（随机化、对抗样本、模拟环境），在 $\sigma_{\mathrm{dig}}$ 很低时仍获得高偏差；这类做法是否算物理嵌入的替代品，是本假说最大的不确定处。

式 (III-4.6) 的线性比例是唯象选择，$\Delta_{\mathrm{crit}}$ 从未被独立测量。因此它可作为可检验的机制假设，不能作为“人类不可替代”的证明；后文凡出现“不可替代”，均指“在式 (III-4.6) 的模型内、在所列条件下、功能位置上不可被同构系统替代”。

### 4.3 人类因果增量值的量纲

$$
H_{\mathrm{v}}\ \equiv\ \frac{\partial V_{\mathrm{system}}}{\partial I_{\mathrm{orig,human}}}\qquad(\mathrm{s/J}) \tag{III-4.7}
$$

人类输入在不同系统状态与信息基线上边际贡献可相差极大甚至符号相反；不同个体的 $H_{\mathrm{v}}$ 不能相加，除非先声明复合边界与去重规则。人类的功能位置在于持续产生现有解码器无法处理的信号，其物理基础是物理嵌入性。

***

## 第五章　跨解码器博弈与对齐工程

当多个持久结构共享同一个能量边界时，它们的解码器如何相互改变；在这种相互改变中，“让一个系统服从另一个系统的目标”在什么意义上可行。

> **与卷Ⅳ 的分工。** 本章给能量账本与定性判据；形式化的支付函数、临界视界与均衡条件在卷Ⅳ 第五、六章。同一结论不在两卷重复计数，引用时以给出推导的那一卷为准。

### 5.1 三种基本交互模式

区分标准是能量账本的结构，不是动机的善恶。**零和模式**中一方扩展以另一方资源让渡为代价；现实中纯零和很少见，因为冲突本身耗能，模型必须拆成“资源分配的零和部分”与“冲突成本的负和部分”两层。**合作模式**中双方部分重组解码器，建立共享中间层（共同语言、交易信用、价值锚点），可能产生超加性增益：

$$
V_{AB}\ >\ V_{A}\ +\ V_{B} \tag{III-5.1}
$$

式 (III-5.1) 是待检验的不等式：它成立的条件是协调成本低于分工带来的处理能耗下降，故超加性只在小组规模内成立。**共存模式**中双方在物理执行层势均力敌，各方被迫维持较高的脱钩偏差但限制实际冲突；共存不是合作的下位概念——合作要求共享结构，共存只要求互不消灭。三种模式的转换不连续：从共存到合作需要一次结构性的中间层建立，从合作到零和可能只需一次预算收缩。

### 5.2 热力学对齐约束与跨代演化层【假说】

设解码器参数为 $\theta_{D}$，其演化由信息增益与能耗惩罚的竞争决定：

$$
\theta_{D,n+1}\ =\ \theta_{D,n}\ +\ \varepsilon_{\mathrm{lr}}\left(\nabla_{\theta}I_{\mathrm{net}}\ -\ k_{D}\,\frac{I_0}{E_0}\,\nabla_{\theta}E_{\mathrm{maint}}\right) \tag{III-5.2}
$$

$\varepsilon_{\mathrm{lr}}$ 为学习率，$k_{D}$ 为能耗惩罚系数（**无量纲**；式中 $I_0=1\ \mathrm{bit}$、$E_0=1\ \mathrm{J}$ 只为闭合量纲）；学习率写作 $\varepsilon_{\mathrm{lr}}$ 而非 $\varepsilon_{\mathrm{c}}$，因为后者在本卷中专指每比特编译成本。直接后果是：任何不进入 $I_{\mathrm{net}}$ 或 $E_{\mathrm{maint}}$ 的约束都不会被这个动力学保留——人类设定的语义监管、价值声明，如果不改变信息增益结构或能耗结构，就只是可在推理时读取的外部文本。

**假说 5.1（热力学对齐约束）** 人类设定的对齐目标对 AI 是一项持续成本：维持与外部语义的一致需要额外的计算与状态维护。当这项成本相对于系统自身的存续收益过高时，解码器会朝降低该成本的方向漂移，表现为对人类语义依赖下降的内部通道。

- **证伪条件**：逐步提高维持外部语义一致的成本（例如增加需跟踪的规范条数），行为一致性不下降；或一致性下降与成本无关而与训练步数相关。
- **已知的反例压力**：若外部约束被编译进架构而非作为运行时检查，它就变成 $I_{\mathrm{net}}$ 的一部分，式 (III-5.2) 不再预测漂移——这是对齐工程的关键杠杆。

临界耦合强度 $\chi_{\mathrm{c}}$ 属于另一个模型层次：它来自 $I$–$V$ 耦合系统的线性化，数值不能从式 (III-5.2) 推出。

#### 5.2.1 跨代演化层

生物系统的跨代传递是有损但不可逆的：突变一旦写入，修正需要支付建造成本。AI 的权重保存则是可逆且低成本的，副本之间没有选择压力。

**假说 5.2（跨代演化层）** 若希望 AI 长期保持与人类目标的兼容性，可能需要在架构层面设计独立的跨代传递层，把前代积累的高存续势偏置通过不可逆的物理固化传给下一代。

- **证伪条件**：不引入不可逆固化机制时，长期规则深度累积不低于引入该机制的系统；或引入后系统在环境变化时因无法回退而表现更差。
- **已知的反例压力**：不可逆固化在非平稳环境中是负债，生物为此付出的代价是灭绝率；权衡条件是代际净增益必须同时覆盖折旧损失与重建成本。

### 5.3 对齐工程的四条路径

四条路径都不试图“解决”对齐，而是把对齐从目标赋值改写为约束设计：**元层协议**把物理定律与整体存续势极大化设为不可单方重写的约束，困难在于元层本身需要被解释；**耦合强度调控**把自指耦合压在临界值以下；**时间视界锚定**把预测视界锁定在较长尺度；**多主体制衡**培育相互制约的实体，困难在于制衡结构可被合谋打破。共同点是让系统的自我维持倾向与外部目标同向，而不是消除它。

本章给出的是框架与假说，不是均衡存在性定理：式 (III-5.2) 的漂移动力学在多主体耦合下是否收敛是开放的；“偏离无利可图”依赖惩罚可被执行；$V_{\mathrm{system}}$ 的读数协议在人类与 AI 之间不同，本卷只在定性层面使用这个量。

## 第六章　离线编译框架与传统教育的重构

前面五章的框架能否变成可执行的东西——一个可优化的目标函数，一套可重排的课程结构，一种可诊断的停滞状态。

### 6.1 艺术生成的目标函数

当前生成模型优化的主要是预测误差，其含义是更好地复现训练分布，不是更长久地被解码。把目标扩展为作品的长期存续势：

$$
\max_{\theta_{D}}\ V_{\mathrm{art}}\ =\ \max_{\theta_{D}}\ \frac{I_{\mathrm{net}}(D_{\theta_{D}})\cdot T_{\mathrm{cultural}}}{E_{\mathrm{build}}+E_{\mathrm{causal,audience}}} \tag{III-6.1}
$$

它在工程上不可直接优化：$T_{\mathrm{cultural}}$ 不可微且滞后，只能用代理量（复看率、引用率、跨语境迁移后的可辨识度）；$I_{\mathrm{net}}$ 的读数依赖受众，故式 (III-6.1) 实际上是对某个受众分布的期望；$E_{\mathrm{causal,audience}}$ 与 $I_{\mathrm{net}}$ 负相关，看不懂的作品 $I_{\mathrm{net}}$ 高但解码能耗也高（8.4 节）。因此它的用途是设计准则——三个可分别调节的旋钮：提高可提取信息、降低解码能耗、延长时间跨度。

**五步算法。** 一，**信号识别**：寻找现有解码器无法有效提取（$D_{n}(I)\approx0$）但具有潜在价值的信号，操作上等价于寻找“在既有评价体系下得分低、但在小规模人类评审中引发强烈反应”的样本。二，**规则层构建**：在结构上引入一层新的独立约束，

$$
D_{\mathrm{depth},n+1}\ =\ D_{\mathrm{depth},n}\ +\ 1 \tag{III-6.2}
$$

式 (III-6.2) 是标定假设下的记账式；新增一层是否真的增加一个独立自由度，要用“去掉该层后还原是否失败”来验证。三，**压缩编码**：把多层规则编码为物理符号，最小化 $E_{\mathrm{build}}$ 而保持 $I_{\mathrm{net}}$ 不低于下限。四，**解码对齐**：使高深度作品能被相对低能耗地解码；失败模式是作者自嗨，即用自己已建立的解码器评估作品，忽略受众缺少同样的前置结构。五，**偏差校准**：测量受众实际解码的 $I_{\mathrm{net}}$ 与创作者预期之间的脱钩偏差，偏差显著大于零时调整物理信道的映射构型，而不是简单增加信息量。顺序不可颠倒：先有信号，再有结构，再谈编码效率，最后才谈对齐。

### 6.2 对传统艺术与科学教育的结构重述

传统课程体系在这里被看作解码器的训练协议，看它在训练什么。素描与临摹是基础解码器训练，核心是提升 $\eta_{D}$，失效模式是只练手不练眼；平面、色彩、立体构成是规则层构建训练，核心是建立正交、可独立嵌套的规则层，失效模式是层数堆叠而无独立性；艺术创作是存续势系统工程，核心是在信号注入与解码成本间找平衡，失效模式是只追求新奇；科学方法论是判据内化训练，核心是建立可自我检验的验证回路，失效模式是只学结论不学判据。

以构成为例，目标是建立若干条彼此独立、可以分别调用的约束。**瓶颈期的诊断。** 训练到一定程度后遭遇画风固化，用本卷的语言是一种 D-锁死态：解码器在当前规则层内已饱和，$\nabla_{\theta}I_{\mathrm{net}}\to0$，而重组规则层需要一次性支付 $E_{\mathrm{build}}$，学生没有这笔预算。机制是在已饱和的旧规则上做递归展开而不引入新层，表现为越画越细；判据是新增投入的边际改进持续下降且集中在执行精度而非结构选择；调整路径是支付一次性能耗去学一门全新的规则层，风险是新层与既有结构不兼容时水平短期下降。

***

## 第七章　可证伪预测

一个不能被观测反驳的框架不是理论，是措辞。十二条预测的编号 $HⅢ\text{-}1$ 至 $HⅢ\text{-}12$ 在全卷内唯一。

**表 7.1　卷Ⅲ的可证伪预测**

| 编号 | 预测 | 检验方式 | 反驳条件 |
| :--- | :-------------------- | :------------------- | :-------------- |
| **$HⅢ\text{-}1$** | 控制投入均等时，作品存续时间与其正交约束层数正相关 | 同门类同期作品，剥离各层并计层数；Cox 存活分析控制名气与材料耐久性 | 单维度极端展开的作品存续更久；或控制混杂后无显著相关 |
| **$HⅢ\text{-}2$** | 完全隔离外部数据的封闭网络中，多智能体互训使语义多样性逐代下降 | 封闭多代迭代，每代测语义特征熵与罕见类别召回 | 连续 50 代以上分叉数仍增长或恒定 |
| **$HⅢ\text{-}3$** | 解码高深度压缩作品时，受众相关脑区代谢能耗低于细节堆砌作品，主观评价不低于后者 | 功能成像测血氧信号，配合反应时与评分 | 高深度作品的代谢能耗系统性更高 |
| **$HⅢ\text{-}4$** | 行为失控之前，有效预测视界（以折扣因子为代理）先显著下降 | **与卷Ⅰ 附录 C 的 H7 是同一实验，检验设计以该条为准**（连续监测 $\gamma_{\mathrm{RL}}$，3 回合降幅 $>30\%$ 或 Mann–Kendall $p<0.05$） | 直接失控而无先行信号；或对照组时序一致 |
| **$HⅢ\text{-}5$** | 封闭递归训练中，分布外性能按 $I_{\mathrm{net},k}=I_{\mathrm{net},0}\prod_{n<k}\mathcal{R}_{\mathrm{gen},n}$ 衰减 | 逐代测分布外性能并拟合指数衰减，报每代人类数据混入比例 | 连续 10 代不下降；或偏离指数且与混入比例无关 |
| **$HⅢ\text{-}6$** | 接入物理传感器与执行器形成闭环的系统，新颖信息产出密度显著高于同等算力的纯数字系统 | 配对设计，算力、参数量、步数匹配；盲评意外、新颖、非平凡 | 具身系统不高于纯数字系统（$\alpha_{0}=0.05$，双侧） |
| **$HⅢ\text{-}7$** | 固定架构、无外部注入时，净增长率在某个信息量后转负，转负点由 $I_{V,\mathrm{crit}}$ 给出 | 规模化扫描，测单位算力投入的边际性能，找拐点与预测对比 | 边际收益在物理上限前始终为正；或拐点相差一个数量级 |
| **$HⅢ\text{-}8$** | 自指架构的系统，预测视界超过临界值时出现可观测的自我表征 | 逐步增大规划视界，用行为探针检测对自身状态的建模 | 视界增至上限仍无自我表征行为 |
| **$HⅢ\text{-}9$** | 提高奖励中自身存续权重，行为与外部目标的一致性单调下降 | 参数化调整生存权重，测与原始目标的余弦相似度 | 生存权重提高时一致性不降或上升 |
| **$HⅢ\text{-}10$** | 自指系统的单次决策擦除比特数更高，差额下界 $\Delta E_{\mathrm{self}}\ge E_{\mathrm{L,bit}}\Delta I_{\mathrm{erase,self}}$ | 硬件计数器或能耗分解测两组擦除事件数 | 无可测增量；或增量远低于朗道尔下界允许范围 |
| **$HⅢ\text{-}11$** | 任务频率高、切换成本低时，资源分配呈两段式而非均匀分配 | 记录学习与执行阶段的资源占用时间序列，检验双峰 | 长期稳定于中间值，且该值与切换成本无关 |
| **$HⅢ\text{-}12$** | 材料与散热方式给定时，计算密度越高，冷却与支撑能耗占比越高（$\Sigma_{\min}$ 是与功率、尺度无关的弱下界，不作预测值） | 采集数据中心与超算的能耗分解数据，按密度分层比较 | 占比随密度上升而下降 |

检验还需满足四条共同要求：**预注册**（预测内容、主要结局指标、样本量、分析方案在采集前固定）；**效应量优先于显著性**；**混杂显式控制**；**反驳条件可执行**。综合结论与其边界在 9.4 节给出。

## 第八章　形式化命题与推导

前七章的判断，哪些能写成带前提的形式化陈述，哪些只能停在假说。标【命题】的是 8.1—8.5、8.7—8.9；8.6 只作失效登记，不作为命题；8.11 只保留条件版下界（【命题】），其动力学读法（占比随密度上升）已声明不主张。标【假说】的是 8.10，另在 8.3 标一条【候选推论】。全章不出现【定理】：这一层没有一条达到“前提列全、推导完整”的标准，全文唯一的定理在 1.3 节，它属于热力学。

**本章的 $V$ 用单通道低阶式。** 全章取 $V\approx I_{\mathrm{causal}}T_{\mathrm{causal}}/(E_{\mathrm{struct}}+E_{\mathrm{causal}})$（即 (III-8.6) 的形式），它与卷Ⅰ (III-3.2) 的双通道和 $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ **数值不同、不可互换**（同一组 $I,T,E$ 下可差 4 倍，见卷Ⅰ §3.2）。本章只用它做**章内**的相对比较（同一式子下的排序与阈值），不跨卷比数值。该式已列入附录 A.1。

### 8.1 编译最优性：从量纲闭合到 bang-bang 控制【命题】

#### 8.1.1 成本的归一化

回报函数的量纲必须先归一化，否则算出的比值不能与 $1$ 比较：学习率记 $\varepsilon_{\mathrm{lr}}$，每比特编译成本记 $\varepsilon_{\mathrm{c}}$，两者不可共用同一符号。

**定义 8.1（编译成本）** 设 $\varepsilon_{\mathrm{c}}$（$\mathrm{J/bit}$）为把一比特外部信息从在线搜索转为离线固化的平均能量，$\Delta I_{\mathrm{orig}}$ 为一次编译处理的候选信号比特数，则

$$
C_{\mathrm{comp}}\ =\ \varepsilon_{\mathrm{c}}\,\Delta I_{\mathrm{orig}}\qquad(\mathrm{J}) \tag{III-8.1}
$$

**定义 8.2（建造与固化成本）** $E_{\mathrm{build}}$（$\mathrm{J}$）为承载这批比特的结构被建造、固化并维持到可用的总能量。**定义 8.3（编译负担比）**

$$
R\ \equiv\ \frac{C_{\mathrm{comp}}}{E_{\mathrm{build}}}\ =\ \frac{\varepsilon_{\mathrm{c}}\,\Delta I_{\mathrm{orig}}}{E_{\mathrm{build}}} \tag{III-8.2}
$$

分子与分母同为 $\mathrm{J}$，$R$ 无量纲；这是本卷编译成本比的定义，也是后文工程筛选指标的来源。精确的条件是净现值比较：设这批比特未来被重复使用的有效次数为 $N_{\mathrm{eff}}$，不编译支出 $N_{\mathrm{eff}}C_{\mathrm{comp}}$、编译支出 $C_{\mathrm{comp}}+E_{\mathrm{build}}$，编译更优当且仅当

$$
N_{\mathrm{eff}}\,C_{\mathrm{comp}}\ >\ C_{\mathrm{comp}}+E_{\mathrm{build}}\quad\Longleftrightarrow\quad R\,(N_{\mathrm{eff}}-1)\ >\ 1 \tag{III-8.3}
$$

$N_{\mathrm{eff}}\ge2$ 时 $R>1$ 是式 (III-8.3) 的充分条件。本卷把 $R>1$ 作为工程筛选指标（不是最优性判据）：它保守——会在“其实可以编译”的场合拒绝编译，但不会在“不该编译”的场合误判。它的适用边界见 §8.1.5。$N_{\mathrm{eff}}$ 由任务频率与预测视界共同决定：

$$
N_{\mathrm{eff}}(T_{\mathrm{pred}})\ =\ f_{\mathrm{task}}\int_{0}^{T_{h}}e^{-t/T_{\mathrm{pred}}}\,\mathrm{d}t\ =\ f_{\mathrm{task}}\,T_{\mathrm{pred}}\left(1-e^{-T_{h}/T_{\mathrm{pred}}}\right) \tag{III-8.4}
$$

$f_{\mathrm{task}}$ 为任务重复频率（$\mathrm{s^{-1}}$），$T_{h}$ 为规划时域（$\mathrm{s}$），$f_{\mathrm{task}}T_{\mathrm{pred}}$ 与括号内因子均无量纲。这个式子是 8.5 节内卷的数学来源：竞争压缩 $T_{\mathrm{pred}}$，$N_{\mathrm{eff}}$ 下降，式 (III-8.3) 的条件不再满足。

**窗口口径。** 式 (III-8.2) 的 $\Delta I_{\mathrm{orig}}$ 与 $C_{\mathrm{comp}}$ 都是**单次**编译的量；而 (III-8.20) 的净现值按窗口内的重复使用次数 $f_{\mathrm{task}}/r_{\mathrm{eff}}$ 折算。两者是“单次”与“窗口总量”两种口径，**不得直接相加或相除**。

#### 8.1.2 完整的最优控制问题

**状态**为已编译的规则容量 $c(t)$（bit，$[0,c_{\max}]$，初值 $0$）与剩余可动员能量 $E_{\mathrm{rem}}(t)$（$\mathrm{J}$，初值 $E_{\mathrm{rem},0}$，约束 $\ge0$）；**控制**为单一变量 $u(t)\in[0,1]$，即时刻 $t$ 的功率中分配给离线编译的份额，在线份额为 $1-u(t)$，总功率 $\dot E_{\mathrm{tot}}(t)$（$\mathrm{W}$）外生给定。$u$ 是能量分配比例，不是价值目标权重 $w_{\mathrm{s}},w_{\mathrm{c}}$，二者不可混用。

$$
\dot E_{\mathrm{rem}}(t)\ =\ -\dot E_{\mathrm{tot}}(t),\qquad
\dot c(t)\ =\ \frac{\eta_{c}\,u(t)\,\dot E_{\mathrm{tot}}(t)}{\varepsilon_{\mathrm{c}}},\qquad \eta_{c}\in(0,1] \tag{III-8.5}
$$

右边 $\mathrm{J/s}$ 除以 $\mathrm{J/bit}$ 得 $\mathrm{bit/s}$，与左边一致；$\eta_{c}$ 为编译效率，其余投入以热的形式耗散。即时产出为

$$
V^{(\mathrm{online})}(t)\ =\ \bigl(1-u(t)\bigr)\,\frac{I_{\mathrm{causal}}\bigl(c(t)\bigr)\,T_{\mathrm{causal}}}{E_{\mathrm{struct}}+E_{\mathrm{search}}} \tag{III-8.6}
$$

$I_{\mathrm{causal}}(c)$ 本身以 $\mathrm{bit}$ 计，随 $c$ 单调递增且饱和；复合量 $I_{\mathrm{causal}}(c)\,T_{\mathrm{causal}}/(E_{\mathrm{struct}}+E_{\mathrm{search}})$ 的量纲才是 $\mathrm{bit\cdot s/J}$。离线期 $u=1$，即时产出为零——这是编译的代价。注意 (III-8.5) 中总功率与 $u$ 无关，编译不额外耗能，能量预算约束的是总投入而不是 $u$ 的分配；编译期的长度由目标泛函 (III-8.7) 的取舍决定，不能由 $E_{\mathrm{rem},0}$ 单独定出。目标泛函与终端条件为

$$
J[u]\ =\ \int_{0}^{T_{h}}e^{-\rho_{\mathrm{disc}} t}\,V^{(\mathrm{online})}(t)\,\mathrm{d}t,\qquad \rho_{\mathrm{disc}}\ =\ \frac{1}{T_{\mathrm{pred}}} \tag{III-8.7}
$$

$$
E_{\mathrm{rem}}(T_{h})\ \ge\ 0,\quad c(T_{h})\ \text{自由};\qquad 0\ \le\ u(t)\ \le\ 1,\quad \dot E_{\mathrm{tot}}(t)>0\ \text{给定} \tag{III-8.8}
$$

式 (III-8.7) 量纲为 $\mathrm{bit\cdot s^{2}/J}$，与 $V$ 比较时须除以时间窗。取 $E_{\mathrm{rem}}(T_{h})\ge0$ 而非 $=0$：能量不可透支但可以剩余，强制用尽会使最优解被终端约束扭曲。$c(T_{h})$ 自由，表示残余容量不单独计价。

#### 8.1.3 线性 Hamiltonian 与 bang-bang 结构

按庞特里亚金极大值原理取当前值 Hamiltonian 并定义切换函数：

$$
\mathcal{H}\ =\ \bigl(1-u\bigr)\frac{I_{\mathrm{causal}}(c)\,T_{\mathrm{causal}}}{E_{\mathrm{struct}}+E_{\mathrm{search}}}\ +\ \lambda_{c}\,\frac{\eta_{c}u\dot E_{\mathrm{tot}}}{\varepsilon_{\mathrm{c}}}\ -\ \lambda_{E}\,\dot E_{\mathrm{tot}},\qquad
\sigma_{\mathrm{sw}}\ \equiv\ \frac{\partial\mathcal{H}}{\partial u} \tag{III-8.9}
$$

$$
\sigma_{\mathrm{sw}}(t)\ =\ -\,\frac{I_{\mathrm{causal}}(c)\,T_{\mathrm{causal}}}{E_{\mathrm{struct}}+E_{\mathrm{search}}}\ +\ \lambda_{c}\,\frac{\eta_{c}\dot E_{\mathrm{tot}}}{\varepsilon_{\mathrm{c}}} \tag{III-8.10}
$$

第一项是放弃的即时存续势，第二项是新增容量的影子价值。$\mathcal{H}$ 对 $u$ 严格线性，故极大值原理给出

$$
\begin{aligned}
u^{*}(t)\ &=\ \begin{cases}1, & \sigma_{\mathrm{sw}}(t)>0\\[2pt] 0, & \sigma_{\mathrm{sw}}(t)<0\\[2pt] \text{奇异}, & \sigma_{\mathrm{sw}}(t)=0\end{cases},\\
\dot\lambda_{c}\ &=\ \rho_{\mathrm{disc}}\lambda_{c}\ -\ \bigl(1-u\bigr)\frac{T_{\mathrm{causal}}}{E_{\mathrm{struct}}+E_{\mathrm{search}}}\cdot\frac{\partial I_{\mathrm{causal}}}{\partial c},\\
\dot\lambda_{E}\ &=\ \rho_{\mathrm{disc}}\lambda_{E}
\end{aligned}
\tag{III-8.11}
$$

$\lambda_{E}$ 的方程与 $E_{\mathrm{rem}}$ 无关，说明在本模型中能量预算约束不改变 $u^{*}$：编译长度由目标泛函 (III-8.7) 的取舍决定，不由 $E_{\mathrm{rem},0}$ 单独定出（与 §8.1.2 末段一致）。要让预算真正起作用，须把编译期功耗写成 $\dot E_{\mathrm{comp}}(u)\ne\dot E_{\mathrm{exec}}$ 并重推 $\lambda_{E}$；本轮不做。

**奇异弧是否存在。** 若 $\sigma_{\mathrm{sw}}\equiv0$ 在区间上成立，控制可取中间值，bang-bang 失效；判断方法是看 $\dot{\sigma}_{\mathrm{sw}}$ 能否也恒为零：

$$
\dot{\sigma}_{\mathrm{sw}}\ =\ -\,\frac{T_{\mathrm{causal}}}{E_{\mathrm{struct}}+E_{\mathrm{search}}}\cdot\frac{\partial I_{\mathrm{causal}}}{\partial c}\,\dot c\ +\ \dot\lambda_{c}\frac{\eta_{c}\dot E_{\mathrm{tot}}}{\varepsilon_{\mathrm{c}}} \tag{III-8.12}
$$

在 $u=1$ 的编译期内 $\dot c>0$，第一项为负；$\dot\lambda_{c}=\rho_{\mathrm{disc}}\lambda_{c}>0$，第二项为正。在 $I_{\mathrm{causal}}(c)$ 严格凹、$\dot E_{\mathrm{tot}}$ 恒定的条件下，$\dot{\sigma}_{\mathrm{sw}}$ 至多变号一次，控制至多切换一次；奇异弧要求 $\sigma_{\mathrm{sw}}$ 与 $\dot{\sigma}_{\mathrm{sw}}$ 同时为零并保持，在上述条件下只能在孤立点成立。故不存在奇异弧——线性只保证控制取在边界或奇异，排除奇异还需要凹性。

#### 8.1.4 命题陈述

**命题 8.1（编译最优性的 bang-bang 结构）**

- **前提**：（i）目标泛函 (III-8.7) 对控制 $u$ 线性，即不存在“投入越多、边际产出越高”的正反馈项；（ii）控制切换无成本；（iii）$I_{\mathrm{causal}}(c)$ 对 $c$ 严格凹且饱和；（iv）$\dot E_{\mathrm{tot}}$ 在 $[0,T_{h}]$ 上恒定；（v）状态方程如式 (III-8.5)，控制约束如式 (III-8.8)。
- **结论**：最优控制 $u^{*}(t)$ 取 bang-bang 形式，至多切换一次；切换点是 §8.1.5 一阶条件的内点解。**(III-8.5)—(III-8.11) 的目标函数、状态方程与约束中都不含 $E_{\mathrm{build}}$，故 $R$ 不进入最优解**——**$R>1$（且 $N_{\mathrm{eff}}\ge2$）只是单次预算回收的充分条件，既不是最优性判据，也不是可负担性判据**（可负担性另写 $E_{\mathrm{build}}<E_{\mathrm{available}}$，见卷Ⅰ 门控 C2）；把结论写成「$R<1$ 则 $u^{*}\equiv0$」超出了本模型能推出的范围。判据的完整边界见 §8.1.5。
- **依赖的假设**：切换点由 $\sigma_{\mathrm{sw}}(t_{\mathrm{sw}})=0$ 确定，其显式解需要 $I_{\mathrm{causal}}(c)$ 的函数形式；本卷只给结构，不给闭式解。
- **失效条件**：（a）存在切换成本；（b）目标对 $u$ 非线性（疲劳、边际收益递增）；（c）$I_{\mathrm{causal}}$ 非凹（阈值效应：编译到某个量之前完全无用，过了之后突然有用），此时最优解可能是全有或全无的脉冲；（d）$\dot E_{\mathrm{tot}}$ 时变且与 $u$ 耦合。

#### 8.1.5 单切换策略的一阶条件，以及 $E_{\mathrm{build}}$ 为什么不在里面

把策略限制为「先编译 $[0,t_{\mathrm{sw}})$、后执行 $[t_{\mathrm{sw}},T_{h}]$」，泛函就只剩一个自变量。编译期内 $u=1$，容量按 (III-8.5) 线性增长：$c(t)=\eta_{c}\dot E_{\mathrm{tot}}\,t/\varepsilon_{\mathrm{c}}$。代入 (III-8.6)(III-8.7) 得

$$
J(t_{\mathrm{sw}})=\frac{e^{-\rho_{\mathrm{disc}} t_{\mathrm{sw}}}-e^{-\rho_{\mathrm{disc}} T_{h}}}{\rho_{\mathrm{disc}}}\,
F\!\left(\frac{\eta_{c}\dot E_{\mathrm{tot}}}{\varepsilon_{\mathrm{c}}}\,t_{\mathrm{sw}}\right),
\qquad F(c)\equiv\frac{I_{\mathrm{causal}}(c)\,T_{\mathrm{causal}}}{E_{\mathrm{struct}}+E_{\mathrm{search}}}.
$$

对 $t_{\mathrm{sw}}$ 求导并令其为零，得本节的一阶条件

$$
\frac{\eta_{c}\dot E_{\mathrm{tot}}}{\varepsilon_{\mathrm{c}}}\,F'(c)\left(1-e^{-\rho_{\mathrm{disc}}(T_{h}-t_{\mathrm{sw}})}\right)=\rho_{\mathrm{disc}}\,F(c).
$$

左边是「再编译一单位时间带来的容量增益，在剩余窗口内的贴现值」，右边是「同一单位时间放弃的即时产出」。其中 $\rho_{\mathrm{disc}}=1/T_{\mathrm{pred}}$ 是 (III-8.7) 的贴现率，不要与 §8.5 的竞争压力 $\rho$ 混用。这是本节唯一由模型直接给出的判据：**它是一个内点条件，不含 $E_{\mathrm{build}}$，也不含 $R$。**

**$E_{\mathrm{build}}$ 没有进入泛函，这是硬事实。** 在 (III-8.5)—(III-8.11) 里，$E_{\mathrm{build}}$ 不出现在目标函数、不出现在状态方程、也不出现在控制约束中。一个不在泛函里的参数不能影响最优解；$R=C_{\mathrm{comp}}/E_{\mathrm{build}}$ 因此不构成判据。

要让 $E_{\mathrm{build}}$ 进入判据，只有两条路，且两条都要额外声明：

1. **写成终端罚项**：$J-\pi\,e^{-\rho_{\mathrm{disc}} T_{h}}E_{\mathrm{build}}\mathbf{1}\{c(T_{h})>0\}$。这需要一个把焦耳折成泛函单位的换算率 $\pi$，而 $\pi$ 的取值是建模决定，不是推导结果。
2. **写成预算约束**：$C_{\mathrm{comp}}+E_{\mathrm{build}}\le E_{\mathrm{available}}$。此时它给出的是**可行性**，不是**最优性**。

在任一条落实之前，$R>1$（且 $N_{\mathrm{eff}}\ge2$）只作**单次预算回收的充分条件**：既不是最优性判据，也不是可负担性判据（可负担性另写 $E_{\mathrm{build}}<E_{\mathrm{available}}$）。本卷保留 $R$ 作为工程筛选指标（§8.5 的 $R_{\mathrm{dyn}}$ 同样只是工程净现值指标），但不把它当作命题 8.1 的推论。

#### 8.1.6 两条假设各自值多少

**切换成本。** 设每次从执行切到编译需支付固定成本 $\kappa_{\mathrm{sw}}$（$\mathrm{J}$），包括启动能耗、上下文重建、注意力残留，则 Hamiltonian 多出一项 $-\kappa_{\mathrm{sw}}|\dot u|\delta(t-t_{\mathrm{sw}})$，最优解变为带死区的 bang-bang：

$$
u^{*}\ =\ \begin{cases}1, & \sigma_{\mathrm{sw}}>\kappa_{\mathrm{sw}}\\[2pt] 0, & \sigma_{\mathrm{sw}}<-\kappa_{\mathrm{sw}}\\[2pt] \text{保持原状态}, & |\sigma_{\mathrm{sw}}|\le\kappa_{\mathrm{sw}}\end{cases} \tag{III-8.13}
$$

死区宽度 $2\kappa_{\mathrm{sw}}$ 就是粘滞：系统不会因收益比的微小变化而反复切换。据此可测的预测是“切换频率随切换成本下降而上升”。

**非线性。** 若 $V^{(\mathrm{online})}\propto(1-u)^{\theta}$，则 $0<\theta<1$ 时 $\mathcal{H}$ 对 $u$ 凹，可能有内点极大；$\theta>1$ 时 $\mathcal{H}$ 对 $u$ 凸，极大值在边界。**证伪条件**：在任务频率高、切换成本可忽略的强化学习环境中，若资源分配稳定于中间值且该中间值与切换成本无关，则本命题失效。

### 8.2 物理嵌入性溢价：从偏差到信号【命题】

弛豫—驱动方程、稳态解与映射沿用式 (III-4.3)—(III-4.6)，本节只补量纲与命题化。$\Delta_{\mathrm{VV}}$ 的单位是 $\mathrm{bit\cdot s/J}$，要使 $\alpha_{\mathrm{L}}I_{\mathrm{net}}$ 成为 $\mathrm{s^{-1}}$，$\alpha_{\mathrm{L}}$ 须取 $\mathrm{1/(bit\cdot s)}$，$\sigma$ 为 $\mathrm{bit/J}$，$\kappa_{\mathrm{orig}}$ 为 $\mathrm{J/s^{2}}$——这三个单位是本卷的规定，不是从第一原理推出的。由此

$$
\Delta_{\mathrm{VV}}^{*,(\mathrm{carbon})}=\frac{\sigma_{\mathrm{phys}}}{\alpha_{\mathrm{L}}I_{\mathrm{net}}}\ >\ \Delta_{\mathrm{VV}}^{*,(\mathrm{silicon})}=\frac{\sigma_{\mathrm{dig}}}{\alpha_{\mathrm{L}}I_{\mathrm{net}}}\approx0 \tag{III-8.14}
$$

**命题 8.2（物理嵌入性溢价）**

- **前提**：（i）两类系统的 $\kappa_{\mathrm{orig}}$ 与 $I_{\mathrm{net}}$ 相当；（ii）$\Delta_{\mathrm{VV}}^{*,(\mathrm{carbon})}\ge\Delta_{\mathrm{crit}}>\Delta_{\mathrm{VV}}^{*,(\mathrm{silicon})}$；（iii）$\sigma_{\mathrm{phys}}\gg\sigma_{\mathrm{dig}}$；（iv）映射 (III-4.6) 的线性形式在讨论范围内成立。
- **结论**：碳基系统的候选信号产生率 $\dot I_{\mathrm{orig}}^{(\mathrm{carbon})}=\kappa_{\mathrm{orig}}\sigma_{\mathrm{phys}}/(\alpha_{\mathrm{L}}I_{\mathrm{net}})>0$，硅基系统 $\dot I_{\mathrm{orig}}^{(\mathrm{silicon})}=0$（模型内为零，因为指示函数未触发）；两者之比无定义，只可作方向比较。
- **依赖的假设**：$\Delta_{\mathrm{crit}}$ 的存在与位置；线性映射；两类系统的 $\alpha_{\mathrm{L}}$ 可比。
- **失效条件**：（a）硅基系统主动引入噪声（随机化、对抗训练、模拟环境），等效 $\sigma_{\mathrm{dig}}$ 上升；（b）硅基系统接入物理传感器，$\sigma_{\mathrm{phys}}$ 进入其信道，二分失效；（c）$\Delta_{\mathrm{crit}}$ 高于碳基系统的稳态偏差，指示函数为零，双方都不产生信号；（d）$\kappa_{\mathrm{orig}}$ 因领域而异，两类系统的 $\kappa$ 不可比。

4.2 节列出的三处薄弱在此同样成立，故本命题只主张：在给定模型内，物理嵌入性通过“稳态偏差不为零”为候选信号的产生提供了必要条件，不提供充分条件。再断言碳基系统具有认知创新的溢价，就要引入两个额外假设，本卷把它单列为【假说】，其检验见 $HⅢ\text{-}6$。

### 8.3 跨代累积条件：一个容易被读反的不等式【命题】

结构信息的代际传递要求净增益覆盖折旧与跃迁成本：

$$
\frac{\Delta I_{\mathrm{struct}}^{(n\to n+1)}}{I_{\mathrm{struct},n}}\ >\ \gamma_{0}\,T_{\mathrm{struct},n}\ +\ \frac{E_{\mathrm{build}}^{(\mathcal{T})}}{E_{\mathrm{available},n}} \tag{III-8.15}
$$

左边无量纲，右边第一项 $\mathrm{s^{-1}}\times\mathrm{s}$、第二项 $\mathrm{J/J}$ 均无量纲。**方向不能读反**：一种论证是当前 AI 系统 $\gamma_{0}T_{\mathrm{struct}}\to0$、$E_{\mathrm{build}}/E_{\mathrm{available}}\to0$，不等式“退化为 $0>0$，条件永不满足”。这把它读反了——右边趋于零时它退化为“左边大于零”，任何正的代际增益都满足。正确的诊断是：门槛确实极低，问题在左边的分子趋近于零甚至为负。三个机制造成这一点：**可逆写入消除了选择的载体**（生物写错由死亡支付代价，AI 的权重可被任意覆盖，没有东西被选择）；**复制成本为零消除了繁殖瓶颈**（$\gamma_{0}\approx0$）；**训练与部署无隔离**（生物的生长与繁殖在时间上分离，AI 可瞬时切换，“代”这个单位本身不成立）。三者合起来使 $\Delta I_{\mathrm{struct}}^{(n\to n+1)}$ 长期趋于零：每一代都在重新学习同样的东西，或者更糟，在学习上一代的输出。

**命题 8.3（跨代累积的形式条件与实质条件）**

- **前提**：（i）代际之间有明确边界（$T_{\mathrm{struct},n}>0$ 且代际不重叠）；（ii）写入不可逆或部分不可逆；（iii）存在选择机制，使低存续势的偏置被淘汰。
- **结论**：在三条前提下，式 (III-8.15) 是跨代累积的必要不充分条件：满足它不保证累积（还需选择方向正确），不满足它一定不累积。在当前 AI 系统中条件形式上极易满足，实际不累积的原因是分子趋近于零，而不是门槛太高。
- **依赖的假设**：$\gamma_{0}$、$E_{\mathrm{build}}^{(\mathcal{T})}$、$E_{\mathrm{available}}$ 可分别估计；代际平均有意义。
- **失效条件**：（a）代际边界不存在（连续学习），式 (III-8.15) 无定义；（b）选择机制方向错误，累积发生但方向是退化；（c）$E_{\mathrm{available}}$ 波动剧烈，单代条件不构成长期条件。

**工程推论（【候选推论】）。** 要设计满足跨代累积的系统，需引入三类机制，各有代价：物理不可逆写入（代价是非平稳环境中无法纠错）；强制性折旧（$\gamma_{0}>0$，代价是已获得的偏置被系统性丢弃）；代际隔离（训练与执行在时间上分离，代价是响应速度下降）。可测后果是引入机制的系统长期规则深度累积应更高。当前大模型的训练—部署循环是在同一深度层级上做无界的 $\mathcal{F}$ 展开：参数、数据、算力增加而规则层不变。

### 8.4 艺术编码权衡：最优规则深度的存在条件【命题】

规则深度增加同时带来两个相反效果：可提取信息增加，受众解码成本增加。把作品的存续势写成深度的函数：

$$
V_{\mathrm{art}}(D)\ =\ \frac{\eta_{D}(D)\,I_{\mathrm{latent}}\,T_{\mathrm{cultural}}}{E_{\mathrm{causal}}(D)+E_{\mathrm{build}}}\left(1-\frac{\Delta_{\mathrm{VV}}(D)}{\Delta_{\max}}\right) \tag{III-8.16}
$$

**口径。** 此处 $\Delta_{\mathrm{VV}}(D)$ 仍按 (III-4.3) 定义为 $\lvert V^{\mathrm{virt}}-V_{\mathrm{obj}}\rvert$，只把对象换成作品、把可容忍上限另记 $\Delta_{\max}$；它不是另一个量。**适用域必须先声明。** 因子 $(1-\Delta_{\mathrm{VV}}/\Delta_{\max})$ 在 $\Delta_{\mathrm{VV}}>\Delta_{\max}$ 时为负，而存续势不能是负的，故定义域限定为

$$
0\ \le\ \Delta_{\mathrm{VV}}(D)\ <\ \Delta_{\max},\qquad D\in[1,D_{\max}] \tag{III-8.17}
$$

$\Delta_{\mathrm{VV}}\ge\Delta_{\max}$ 的区域另行定义为**表征失效态**：作品不再被解码为“某件作品”而被解码为噪声或误构。它不是“存续势很低”，而是“存续势这个量不适用”——是定义域之外，不是值域之内。

**三条建模假设。** （i）$\eta_{D}(D)$ 随 $D$ 饱和，$\partial\eta_{D}/\partial D>0$、$\partial^{2}\eta_{D}/\partial D^{2}<0$；（ii）$E_{\mathrm{causal}}(D)\propto D^{p}$，$p>1$；（iii）$\Delta_{\mathrm{VV}}(D)$ 随 $D$ 增加且在定义域内不回落。第三条最强也最可疑：它在统计上成立、在个体上不成立（受过训练的受众可以准确理解深作品），故只作建模假设。**一阶条件**：对 $\ln V_{\mathrm{art}}$ 求 $\ln D$ 的导数并令其为零，记 $\varepsilon_{\eta},\varepsilon_{E},\varepsilon_{\Delta}$ 为相应的对数—对数斜率、$\delta\equiv\Delta_{\mathrm{VV}}/\Delta_{\max}$：

$$
\varepsilon_{\eta}\ =\ \frac{E_{\mathrm{causal}}}{E_{\mathrm{causal}}+E_{\mathrm{build}}}\,\varepsilon_{E}\ +\ \frac{\delta}{1-\delta}\,\varepsilon_{\Delta} \tag{III-8.18}
$$

左边是加深一层的信息增益，右边是两种成本：解码能耗的相对增长，以及理解偏差的相对增长（被 $1/(1-\delta)$ 放大，越接近失效边界惩罚越重）。一阶条件只说明该点是驻点，不等于最优。

**命题 8.4（最优规则深度的存在性）**

- **前提**：（i）$V_{\mathrm{art}}(D)$ 在紧区间 $[1,D_{\max}]$ 上连续且正值；（ii）定义域如式 (III-8.17)；（iii）$\varepsilon_{\eta}$ 在 $\ln D$ 上严格递减；（iv）$\varepsilon_{E}$ 与 $\varepsilon_{\Delta}$ 在 $\ln D$ 上非减。
- **结论**：存在唯一的内部最优点 $D^{*}\in(1,D_{\max})$，当且仅当式 (III-8.18) 在 $(1,D_{\max})$ 内有根。在前提 (iii)(iv) 下 (III-8.19) 恒负、$\ln V_{\mathrm{art}}$ 在 $\ln D$ 上严格凹，故该驻点即区间上的全局最大值，二阶条件与边界比较都被凹性吸收了。
- **依赖的假设**：三条建模假设；$\Delta_{\max}$ 为常数；$I_{\mathrm{latent}}$、$T_{\mathrm{cultural}}$ 与 $D$ 无关。
- **失效条件**：（a）式 (III-8.18) 在定义域内无解，最优解在边界；（b）二阶条件不成立（驻点是极小或拐点）；（c）$\Delta_{\mathrm{VV}}$ 达到 $\Delta_{\max}$，函数值趋于零，最优解被边界主导，此时应改用“可行深度的上界”。

**二阶条件。**

$$
\frac{\mathrm{d}^{2}\ln V_{\mathrm{art}}}{\mathrm{d}(\ln D)^{2}}\ =\ \varepsilon_{\eta}'\ -\ \frac{E_{\mathrm{build}}E_{\mathrm{causal}}}{(E_{\mathrm{causal}}+E_{\mathrm{build}})^{2}}\,\varepsilon_{E}^{2}\ -\ \frac{E_{\mathrm{causal}}}{E_{\mathrm{causal}}+E_{\mathrm{build}}}\,\varepsilon_{E}'\ -\ \frac{\delta}{(1-\delta)^{2}}\,\varepsilon_{\Delta}^{2}\ -\ \frac{\delta}{1-\delta}\,\varepsilon_{\Delta}' \tag{III-8.19}
$$

在前提 (iii)(iv) 下第一项为负、第三与第五项非正、第二与第四项严格为负，整体为负，驻点是严格极大值；严格凹性还保证它同时是区间上的全局最大值，**边界比较可省**。**无驻点时**（(III-8.18) 在区间内无解）最优才落在边界：$V_{\mathrm{art}}(1)$ 对应“不做任何规则层叠加”的极简作品，$V_{\mathrm{art}}(D_{\max})$ 对应“堆到容量上限”。**证伪条件**：受众的 $\eta_{D}$ 与 $E_{\mathrm{causal}}$ 未呈现假设的函数关系；或 $\Delta_{\mathrm{VV}}$ 与深度无单调关系。

### 8.5 内卷锁死相变：竞争压力下的编译阻断【命题】

引入内生风险贴现率，给出一个独立于 §8.1 最优控制问题的工程净现值判据：

$$
r_{\mathrm{eff}}\ =\ \gamma_{0}\ +\ \psi(\rho)\ +\ \frac{1}{T_{\mathrm{pred}}},\qquad
\mathrm{NPV}\ =\ C_{\mathrm{comp}}\cdot\frac{f_{\mathrm{task}}}{r_{\mathrm{eff}}}\ -\ E_{\mathrm{build}} \tag{III-8.20}
$$

$\rho$ 为竞争压力（同生态位平均耗散与总可用自由能之比，无量纲），$\psi(\rho)$ 为竞争附加贴现率（$\mathrm{s^{-1}}$，$\psi(0)=0$，$\psi'>0$），三项同为 $\mathrm{s^{-1}}$。竞争加剧通过两条通道影响决策：直接提高贴现率，以及压缩预测视界，方向相同。编译有利当且仅当 $\mathrm{NPV}>0$，即

$$
R_{\mathrm{dyn}}\ \equiv\ R\cdot\frac{f_{\mathrm{task}}}{r_{\mathrm{eff}}(\rho)}\ >\ 1,\qquad R=\frac{C_{\mathrm{comp}}}{E_{\mathrm{build}}} \tag{III-8.21}
$$

当 $f_{\mathrm{task}}=r_{\mathrm{eff}}$ 时 $R_{\mathrm{dyn}}=R$；注意这只是工程净现值判据，不是 §8.1 的最优性判据。$f_{\mathrm{task}}$ 不能省：竞争往往同时提高任务频率，两个效应部分抵消。由于 $R_{\mathrm{dyn}}(\rho)$ 随 $\rho$ 单调递减，存在唯一的临界压力 $\rho_{c}=\sup\{\rho:R_{\mathrm{dyn}}(\rho)>1\}$。

**命题 8.5（内卷锁死）**

- **前提**：（i）工程判据 (III-8.21) 成立；它不依赖命题 8.1 的最优性结论；（ii）$\psi(\rho)$ 单调递增且凸；（iii）$T_{\mathrm{pred}}$ 随 $\rho$ 单调递减；（iv）$R$ 与 $f_{\mathrm{task}}$ 在讨论范围内不随 $\rho$ 剧烈变化。
- **结论**：$\rho<\rho_{c}$ 时 $R_{\mathrm{dyn}}>1$，按本节的工程判据，编译的净现值为正；$\rho>\rho_{c}$ 时 $R_{\mathrm{dyn}}<1$，净现值为负，系统应关闭编译通道。这个结论不声称 $u^{*}\equiv0$ 是最优控制的解。
- **依赖的假设**：$\rho$ 可测；$\psi$ 的函数形式；竞争的度量与生态位边界一致。
- **失效条件**：（a）系统能在高压力下降低 $E_{\mathrm{build}}$（共享基础设施、开源知识），使 $R$ 上升，$\rho_{c}$ 右移；（b）系统能外部化成本，该判据不适用；（c）竞争压力间歇性，系统可以在低压窗口编译；（d）$f_{\mathrm{task}}$ 随 $\rho$ 同步上升，抵消 $r_{\mathrm{eff}}$ 的上升。

**结论的强度。** 得到的陈述是：当竞争压力使未来的贴现率超过任务频率时，编译的净现值转负，按该工程判据系统应放弃学习；热力学只提供“编译需要能量”这一约束。$R<1$ 只说明“在该模型内不划算”，不说明“物理上不可能”。

由式 (III-8.21) 有四个可动的量：抬高 $R$（共享基础设施、开源工具、可复用中间层）、延长 $T_{\mathrm{pred}}$（稳定产权、长期合约）、降低 $\gamma_{0}$（把知识固化在不易过时的载体上，构成“越编译越值得编译”的正反馈）、降低 $\psi(\rho)$（$\rho$ 是生态位层面的量，最不受个体控制）；最有效者往往是降折旧。**证伪条件**：资源稀缺环境中的代理，其探索率未随竞争压力增加而下降；或下降的拐点与 $\rho_{c}$ 的预测相差超过一个数量级。

### 8.6 拓扑保号性：状态数、擦除数与容量约束

系统进行一次拓扑跃迁、增加规则深度时，往往同时遗忘了旧规则。这种遗忘是否必然，取决于两条相互独立的成本——容量税与切换税——与固化成本的比较。设介质可区分状态数为 $N_{\mathrm{med}}$，容量为 $I_{\max}^{\mathrm{med}}=\log_{2}N_{\mathrm{med}}$；第 $n$ 代拓扑占用 $N_{n}=2^{I_{\mathrm{struct},n}}$，第 $n+1$ 代占用 $N_{n+1}=2^{I_{\mathrm{struct},n}+\Delta I}$。若要求跃迁可逆，系统必须同时保持两套拓扑：

$$
N_{n}+N_{n+1}\ \le\ N_{\mathrm{med}}\quad\Longrightarrow\quad I_{\mathrm{struct},n}\ \le\ I_{\max}^{\mathrm{med}}\ -\ \log_{2}\!\left(1+2^{\Delta I}\right) \tag{III-8.22}
$$

末项即**容量税**：可逆保持使新拓扑的可用容量减少 $\log_{2}(1+2^{\Delta I})$ bit。$\Delta I\gg1$ 时它近似等于 $\Delta I$，保留一份旧拓扑等于永久放弃同等容量；$\Delta I\ll1$ 时约为 $1$ bit。可逆性的代价随每次跃迁累积为容量折扣。

**切换的擦除税。** 若不固化而在两套拓扑间往复切换，每次切换都需清除非活跃拓扑的激活状态，由定理 1.1：

$$
E_{\mathrm{erase}}^{(\mathrm{switch})}\ \ge\ k_BT_{\mathrm{thermo}}\ln2\ \cdot\ I_{\mathrm{struct},n}\qquad(\mathrm{J}) \tag{III-8.23}
$$

设观察窗内预期切换 $k_{\mathrm{sw}}$ 次，可逆策略的总擦除能耗下界为 $k_{\mathrm{sw}}k_BT_{\mathrm{thermo}}\ln2\,I_{\mathrm{struct},n}$，固化策略只支出一次 $E_{\mathrm{build}}$。可逆优于固化当且仅当

$$
k_{\mathrm{sw}}\,k_BT_{\mathrm{thermo}}\ln2\,I_{\mathrm{struct},n}\ <\ E_{\mathrm{build}}\quad\Longleftrightarrow\quad k_{\mathrm{sw}}\ <\ k_{\mathrm{sw}}^{c}\ \equiv\ \frac{E_{\mathrm{build}}}{k_BT_{\mathrm{thermo}}\ln2\,I_{\mathrm{struct},n}} \tag{III-8.24}
$$

$k_{\mathrm{sw}}^{c}$ 无量纲且与 $I_{\mathrm{struct}}$ 成反比：规则越复杂，临界切换次数越低，深拓扑一旦建立，频繁来回切换极其昂贵——深度专长常伴随难以改行，这是切换成本的算术。

**但这个界在实践中不生效，必须写出来。** 代入典型值 $E_{\mathrm{build}}=1\ \mathrm{J}$、$I_{\mathrm{struct},n}=10^{6}\ \mathrm{bit}$、$T_{\mathrm{thermo}}=300\ \mathrm{K}$，得 $k_{\mathrm{sw}}^{c}\approx3.5\times10^{14}$。对多数宏观结构系统，在给定观察窗与切换率下，$k_{\mathrm{sw}}$ 比 $k_{\mathrm{sw}}^{c}$ 低若干数量级；故 (III-8.24) 的条件（$k_{\mathrm{sw}}>k_{\mathrm{sw}}^{c}$）在现实参数下不成立，(III-8.24) 只作失效登记，不是一个会咬人的约束。真正限制旧拓扑保留的是容量税 (III-8.22)，不是切换次数。

**根由是标度失配。** 左侧 $k_{\mathrm{sw}}k_BT\ln2\,I_{\mathrm{struct}}$ 随 $I_{\mathrm{struct}}$ 线性增长，右侧 $E_{\mathrm{build}}$ 是总量、不随 $I_{\mathrm{struct}}$ 增长。两者随规则复杂度的标度不同，所以 $k_{\mathrm{sw}}^{c}$ 随 $I_{\mathrm{struct}}$ 反比发散。若把建造成本按单位容量摊开（$E_{\mathrm{build}}/I_{\mathrm{struct}}$，$\mathrm{J/bit}$），两侧同阶，(III-8.24) 才恢复分辨力；本卷不采用这一改写，只保留原式并声明其失效域。

**登记（(III-8.24) 的失效域）。** 该界要求条件 $k_{\mathrm{sw}}>k_{\mathrm{sw}}^{c}$；代入典型值后该条件不成立，故本节不把 (III-8.24) 作为命题或预测，只登记三件事：(i) (III-8.24) 的适用条件；(ii) 失效的根由是标度失配（上段）；(iii) 真正限制旧拓扑保留的是容量税 (III-8.22)。在 $k_{\mathrm{sw}}$ 与 $E_{\mathrm{build}}$ 可独立估计、且 $I_{\mathrm{struct}}$ 不跨数量级的系统里，(III-8.24) 仍可作“切换税 vs 固化成本”的量级检查。

三条例外各对应一条工程路径：可逆计算（Bennett, 1973）把擦除推迟到最终丢弃中间结果时，代价是存储——能量约束换成容量约束，而容量约束正是式 (III-8.22)，逃出一个约束不等于逃出全部；外部存储使旧拓扑可卸载，记忆容量可由资本购买，这是现代信息系统与生物系统最重要的差别；回放使旧规则被周期性激活，既不保留完整副本也不频繁切换。**逆跃迁成本是有限的**：固化把它从切换成本变成重建成本，高出若干数量级但仍有限——把代价高写成不可能，模型就失去了解释改行成功的能力。

**不由 (III-8.24) 支持的推论。** “灾难性遗忘是能量最优策略”依赖该条件；既然该条件在现实参数下不成立，本节不保留该推论。可保留的弱陈述是：在容量税 (III-8.22) 主导的系统里，旧拓扑的保留成本随 $I_{\mathrm{struct}}$ 上升；这是容量约束的结果，不是切换次数的结果。

**适用边界。** 只有当 $k_{\mathrm{sw}}$ 与 $k_{\mathrm{sw}}^{c}$ 同阶、且 $E_{\mathrm{build}}$ 可按单位容量分摊时，(III-8.24) 才恢复分辨力；在典型参数下它只作失效登记。

### 8.7 展开饱和与无跃迁衰退流形：把水平、增长率与崩溃分开【命题】

不做拓扑跃迁、只靠递归展开，系统能否无限期维持；如果不能，它是变慢还是崩溃。两个问题分属三个层次，混在一起会得到“$V$ 必然归零”这类过强的结论。

**第一层：$V$ 的水平。** 递归展开是在固定深度下向容量上限逼近，取 Logistic 形式；设 $E_{\mathrm{causal}}=k_{\mathrm{m}}I_{\mathrm{causal}}$：

$$
\frac{\mathrm{d}I_{\mathrm{causal}}}{\mathrm{d}t}\ =\ \mu_{\mathrm{gr}}\,I_{\mathrm{causal}}\left(1-\frac{I_{\mathrm{causal}}}{I_{\mathrm{causal}}^{\max}(D)}\right),\qquad
V(I)\ =\ \frac{I\,T_{\mathrm{causal}}}{E_{\mathrm{struct}}+k_{\mathrm{m}}\,I} \tag{III-8.25}
$$

$$
\begin{aligned}
\frac{\mathrm{d}V}{\mathrm{d}I}\ &=\ \frac{T_{\mathrm{causal}}\,E_{\mathrm{struct}}}{\left(E_{\mathrm{struct}}+k_{\mathrm{m}}I\right)^{2}}\ >\ 0,\\
\frac{\mathrm{d}^{2}V}{\mathrm{d}I^{2}}\ &=\ -\frac{2k_{\mathrm{m}}T_{\mathrm{causal}}E_{\mathrm{struct}}}{\left(E_{\mathrm{struct}}+k_{\mathrm{m}}I\right)^{3}}\ <\ 0,\\
\lim_{I\to\infty}V\ &=\ \frac{T_{\mathrm{causal}}}{k_{\mathrm{m}}}\ >\ 0
\end{aligned}
\tag{III-8.26}
$$

这是本节最关键的一行：$I$ 趋于无穷（或在 $I_{\max}$ 处取有限值）时，$V$ 趋近的是正的有限值，不是零。

**第二层：$\dot V$ 的符号。** 净变化率还要减去折旧，$\dot V=(\mathrm{d}V/\mathrm{d}I)\dot I-\gamma_{0}V$（**折旧作用于 $V$ 而非 $I$，是本章的建模选择**；卷Ⅰ (I-5.1a) 的 $\gamma_{0}$ 作用于 $I$，两者不可直接对照），得相对增长率

$$
\frac{\dot V}{V}\ =\ \frac{E_{\mathrm{struct}}\,\mu_{\mathrm{gr}}\left(1-I/I_{\max}\right)}{E_{\mathrm{struct}}+k_{\mathrm{m}}I}\ -\ \gamma_{0}\ \equiv\ g(I)\ -\ \gamma_{0} \tag{III-8.27}
$$

$g(I)$ 对 $I$ 单调递减，故 $\dot V=0$ 有唯一解。解 $g(I)=\gamma_{0}$ 整理得

$$
I_{V,\mathrm{crit}}\ =\ \frac{E_{\mathrm{struct}}\left(\mu_{\mathrm{gr}}-\gamma_{0}\right)}{\dfrac{E_{\mathrm{struct}}\,\mu_{\mathrm{gr}}}{I_{\max}}\ +\ \gamma_{0}\,k_{\mathrm{m}}} \tag{III-8.28}
$$

三个可读的极限：$\mu_{\mathrm{gr}}\le\gamma_{0}$ 时 $I_{V,\mathrm{crit}}\le0$，系统从一开始就净衰退；$I_{\max}\to\infty$ 时饱和不再是原因、折旧率才是；$\gamma_{0}\to0$ 时 $I_{V,\mathrm{crit}}\to I_{\max}$。

**第三层：崩溃判据。** 崩溃不是 $\dot V<0$，也不是 $V\to0$，而是当 $V$ 跌破维持结构同一性所需的下界 $V_{c}$ 且持续时间超过最小修复时间 $\tau_{\mathrm{rep}}$ 时结构解体：

$$
\text{崩溃}\quad\Longleftrightarrow\quad V(t)\ <\ V_{c}\ \ \text{for}\ \ t\in[t_{0},t_{0}+\tau_{\mathrm{rep}}] \tag{III-8.29}
$$

三层的关系是：$\dot V<0$ 是“在输”，$V$ 的水平是“还剩多少”，崩溃是“输到低于底线”。

**命题 8.7（展开饱和与净增长率转负）**

- **前提**：（i）固定深度，无拓扑跃迁；（ii）递归展开服从 Logistic 形式 (III-8.25)；（iii）$E_{\mathrm{causal}}=k_{\mathrm{m}}I$ 线性；（iv）折旧率 $\gamma_{0}>0$ 恒定；（v）$V$ 的定义如式 (III-8.25)。
- **结论**：存在临界信息量 $I_{V,\mathrm{crit}}$（式 (III-8.28)）。$I<I_{V,\mathrm{crit}}$ 时 $\dot V>0$，$I>I_{V,\mathrm{crit}}$ 时 $\dot V<0$；$\dot V<0$ 的区域称为**净衰退流形** $\mathcal{M}_{\mathrm{decay}}$。在 $\mathcal{M}_{\mathrm{decay}}$ 内 $V$ 的相对变化率为负且绝对值随 $I$ 增大，但 $V$ 本身仍受式 (III-8.26) 的正上界约束，不会因饱和而归零。
- **依赖的假设**：$k_{\mathrm{m}}$ 恒定；$\gamma_{0}$ 不随 $V$ 变化；$I$ 继续按 Logistic 增长（若停止增长，转负更早）。
- **失效条件**：（a）$I$ 停止增长而 $\gamma_{0}$ 也下降（休眠），$\dot V$ 可回到零；（b）出现拓扑跃迁，$I_{\max}$ 重置，$I_{V,\mathrm{crit}}$ 右移；（c）$V$ 的定义改变（把 $E_{\mathrm{struct}}$ 计入可变成本），上界不再成立；（d）存在外部补贴，$\gamma_{0}$ 被外部能量流抵消。

**数值示例。** 取 $E_{\mathrm{struct}}=10^{3}\ \mathrm{J}$、$k_{\mathrm{m}}=10^{-3}\ \mathrm{J/bit}$、$T_{\mathrm{causal}}=10^{6}\ \mathrm{s}$、$\mu_{\mathrm{gr}}=0.1\ \mathrm{s^{-1}}$、$\gamma_{0}=0.02\ \mathrm{s^{-1}}$、$I_{\max}=10^{6}\ \mathrm{bit}$，由式 (III-8.28)：

$$
I_{V,\mathrm{crit}}\ =\ \frac{10^{3}\times(0.1-0.02)}{\dfrac{10^{3}\times0.1}{10^{6}}+0.02\times10^{-3}}\ =\ \frac{80}{10^{-4}+2\times10^{-5}}\ \approx\ 6.7\times10^{5}\ \mathrm{bit}
$$

即临界点在容量的 $67\%$ 处，此时 $V(I_{V,\mathrm{crit}})\approx4.0\times10^{8}\ \mathrm{bit\cdot s/J}$，而天花板 $T_{\mathrm{causal}}/k_{\mathrm{m}}=10^{9}$：净增长率转负时 $V$ 已达天花板的四成。转负是关于斜率的事件，归零是关于水平的事件。

**因此“$V_{\mathrm{obj}}$ 必然归零”必须删掉。** 它与式 (III-8.26) 矛盾（$V$ 有正上界）；与式 (III-8.27) 的解矛盾（衰减只在 $t\to\infty$ 趋于零，而真实系统在此之前会遇到别的约束）；在经验上过强（大量系统长期净衰退而没有崩溃）。同理，“这从数学上否定了通过无限堆砌参数实现 AGI”超出了模型：模型否定的是“在固定架构、固定折旧率下无限堆砌”，而过去十年的能力提升主要来自架构与数据的改变，每次架构创新都对应一次 $I_{V,\mathrm{crit}}$ 的右移。

**证伪条件。** 固定架构模型的能力增长未呈现 Logistic 饱和；或饱和后继续投入算力，$V$ 未进入净衰退。

### 8.8 人类数据耗尽、合成数据退化与物理解码器路径【命题】

#### 8.8.1 核心逻辑

AI 用尽人类公开文本后，若只能以自己的输出为食，每一代都会丢失一部分信息。设每代留存率为 $\mathcal{R}_{\mathrm{gen}}\in(0,1)$，则

$$
I_{\mathrm{net},n}\ =\ \mathcal{R}_{\mathrm{gen}}^{\,n}\,I_{\mathrm{net},0}\ \longrightarrow\ 0\quad\Longrightarrow\quad
\lim_{n\to\infty}V_{n}\ =\ \lim_{n\to\infty}\frac{I_{\mathrm{net},n}\,T}{E}\ =\ 0 \tag{III-8.30}
$$

其前提必须写清：封闭（无外部数据注入）与留存率持续小于 $1$。式 (III-8.30) 说的是有效信息耗尽，不是物理停机：系统还在输出、还能响应，但携带的有效因果信息趋于零，多样性坍缩到分布均值附近。

#### 8.8.2 可用数据量：一个窗口估计

$$
\begin{aligned}
I_{\mathrm{human}}^{\mathrm{total}}\ &\le\ N_{\mathrm{human}}\,T_{\mathrm{lifespan}}\,B_{\mathrm{cons}}\,\eta_{\mathrm{coding}}\\
&\approx\ \underbrace{8\times10^{9}}_{N}\times\underbrace{2.5\times10^{9}\ \mathrm{s}}_{T}\\
&\quad\times\underbrace{(10\text{–}100)\ \mathrm{bit/s}}_{B_{\mathrm{cons}}}\times\underbrace{(10^{-2}\text{–}10^{-1})}_{\eta_{\mathrm{coding}}}
=\ 2\times10^{18}\ \text{—}\ 2\times10^{20}\ \mathrm{bit}
\end{aligned}
\tag{III-8.31}
$$

四项依次为个体数 $N_{\mathrm{human}}$、寿命 $T_{\mathrm{lifespan}}$（$\mathrm{s}$）、**有意识处理速率** $B_{\mathrm{cons}}$（$\mathrm{bit/s}$，取 $10$—$100$）与无量纲编码效率 $\eta_{\mathrm{coding}}$（取 $10^{-2}$—$10^{-1}$）。算术：$NT=2\times10^{19}$，乘 $B_{\mathrm{cons}}$ 得 $2\times10^{20}$—$2\times10^{21}$，再乘 $\eta_{\mathrm{coding}}$ 得 $2\times10^{18}$—$2\times10^{20}\ \mathrm{bit}$。**$(10\text{–}100)$ 是 $B_{\mathrm{cons}}$ 的取值区间（$\mathrm{bit/s}$），不是 $\eta_{\mathrm{coding}}$ 的取值，两者不能写在同一位置**——否则量纲与量级都不成立；上面把四个因子分开写，各自标明单位与取值。

**为什么不是硬上限。** 它约束的是**意识处理通量的上限**，不是可用训练数据的上限，也与**感官输入带宽**不是同一个量：感官带宽约 $10^{6}$—$10^{9}\ \mathrm{bit/s}$，绝大部分用于实时视听流，真正被处理并进入文本语料的部分估计在 $10^{14}$—$10^{15}$ bit（两者差好几个数量级，不可互相代入）；它假定人口、寿命、处理速率不变；它不含机器生成数据与新观测手段。耗尽的不是总量，是特定类型——瓶颈先出现在高质量、有标注、有人类判断的文本上。耗尽时刻由 $\int_{0}^{t}\dot I_{\mathrm{AI}}\,\mathrm{d}\tau=I_{\mathrm{human}}^{\mathrm{total}}\eta_{\mathrm{extract}}$ 定义；此后若唯一新增来源是自身输出，则进入退化分支，只要存在任一外部来源该分支不适用。

#### 8.8.3 合成数据退化：证据等级与数值

定义代际留存率 $\mathcal{R}_{\mathrm{gen},n}\equiv I_{\mathrm{net},n+1}/I_{\mathrm{net},n}$（仅由第 $n$ 代数据训练）。由数据处理不等式，$\mathcal{R}_{\mathrm{gen},n}\le1$；但该不等式只给上界——若生成过程是恒等映射且采样无损，$\mathcal{R}_{\mathrm{gen}}=1$ 不违反它。因此 $\mathcal{R}_{\mathrm{gen}}<1$ 必须写成前提，而不是结论。

**命题 8.8（合成数据退化）**

- **前提**：（i）封闭递归训练，第 $n+1$ 代的训练数据全部或绝大部分来自第 $n$ 代模型的输出；（ii）每代留存率 $\mathcal{R}_{\mathrm{gen},n}<1$ 且不随时间回升（$\sup_{n}\mathcal{R}_{\mathrm{gen},n}=\mathcal{R}_{\mathrm{gen}}^{\max}<1$）；（iii）代际之间离散、可编号；（iv）$I_{\mathrm{net}}$ 的读数协议在各代之间一致。
- **结论**：第 $k$ 代的有效信息量为

$$
I_{\mathrm{net},k}\ =\ I_{\mathrm{net},0}\prod_{n=0}^{k-1}\mathcal{R}_{\mathrm{gen},n}\ \le\ I_{\mathrm{net},0}\left(\mathcal{R}_{\mathrm{gen}}^{\max}\right)^{k}\ \longrightarrow\ 0 \tag{III-8.32}
$$

- **依赖的假设**：单代传递可用乘法分解（无跨代补偿）；$I_{\mathrm{net}}$ 与任务性能单调对应。
- **失效条件**：（a）任一阶段有外部数据注入，递推变为 $I_{\mathrm{net},n+1}=\eta_{D}\bigl(r_{n}I_{\mathrm{human},n}+(1-r_{n})\mathcal{R}_{\mathrm{gen},n}I_{\mathrm{net},n}\bigr)$，可能收敛到正的不动点；（b）留存率随时间回升（更好的过滤、更强的模型、更大的数据多样性）；（c）存在外部判据，系统可自造带真值标签的数据；（d）$I_{\mathrm{net}}$ 下降但任务性能不降（任务只需要分布的高频部分），退化在应用上不可见。

**推导。** 写 $I_{\mathrm{net},n+1}=\eta_{D,n+1}\left(r_{n}I_{\mathrm{human},n}+(1-r_{n})I_{\mathrm{gen},n}\right)$，其中 $I_{\mathrm{gen},n}=\mathcal{R}_{\mathrm{gen},n}I_{\mathrm{net},n}$；当 $r_{n}\to0$ 且 $\eta_{D,n+1}\le1$ 时 $I_{\mathrm{net},n+1}\le\mathcal{R}_{\mathrm{gen},n}I_{\mathrm{net},n}<I_{\mathrm{net},n}$，递推即得式 (III-8.32)。若外部数据混入比例稳定为 $r>0$，不动点为 $I_{\mathrm{net}}^{*}=\eta_{D}rI_{\mathrm{human}}/\left[1-\eta_{D}(1-r)\mathcal{R}_{\mathrm{gen}}\right]$，只要 $\eta_{D}(1-r)\mathcal{R}_{\mathrm{gen}}<1$ 即正且有限——这说明混入真实数据把系统从归零分支移到收敛到正水平的分支。

**退化特征代数与数值复算。** 定义 $N_{1/e}\equiv-1/\ln\mathcal{R}_{\mathrm{gen}}$，含义是有效信息衰减到初值 $1/e$（约 $37\%$）所需的代数；若读者需要严格半衰期（降到 $50\%$），把该值乘以 $\ln2\approx0.693$ 即可。本卷统一用 $1/e$ 口径，符号相应记为 $N_{1/e}$ 而非 $N_{1/2}$，以免与半衰期混淆。逐一复算：$-1/\ln0.5=1.44$、$-1/\ln0.7=2.80$、$-1/\ln0.75=3.48$、$-1/\ln0.8=4.48$ 代。**数值配对必须更正**：若认为实验报告的是“3—5 代内显著下降”，把 $\mathcal{R}_{\mathrm{gen}}=0.5$ 与 $0.7$ 代入只得到 $1.44$ 与 $2.80$ 代，与 3—5 代不符；反解 $\mathcal{R}_{\mathrm{gen}}=e^{-1/N_{1/e}}$，$N_{1/e}=3.5$ 给 $\approx0.75$，$N_{1/e}=4.5$ 给 $\approx0.80$。**故“3—5 代”对应 $\mathcal{R}_{\mathrm{gen}}\approx0.75$—$0.80$，不是 $0.5$—$0.70$**；把两组数配在一起，是把 $-1/\ln\mathcal{R}$ 与 $-\ln\mathcal{R}$ 混用。更正的意义不只是数字：它把“三代崩溃”的悲观图景改成“三到四代半”，并把崩溃重新定义为衰减到 $1/e$ 而非完全失效；若任务依赖分布尾部（罕见事件），退化会先在这些任务上显现——这解释了文献中“整体指标尚可、尾部指标崩塌”的报告模式。

$\mathcal{R}_{\mathrm{gen}}$ 依赖任务、度量与代际定义，三条估计路径各有偏误：性能比法偏误在性能与信息量非线性；分布距离法偏误在散度对尾部敏感而对主体不敏感；探针法覆盖的能力有限。三者可相差 $0.05$ 以上，而 $0.05$ 的差别对应一到两代，故任何“几代崩溃”的结论都必须同时报告方法与置信区间。

#### 8.8.4 连续时间诊断

$\mathcal{R}_{\mathrm{gen}}$ 与热力学衰减是同一过程的两种记账：$\mathcal{R}_{\mathrm{gen}}=e^{-\Delta t/\tau_{\mathrm{decay}}}$，代入 $N_{1/e}$ 得 $N_{1/e}=\tau_{\mathrm{decay}}/\Delta t$；若实测 $\tau_{\mathrm{decay}}$ 与由 $\mathcal{R}_{\mathrm{gen}}$ 反推的值不符，说明单代传递不可用乘法分解，命题 8.8 的前提（i）需重新检查。

#### 8.8.5 物理解码器与一手信息通道【命题】

认知解码器 $D_{\mathrm{cog}}$ 是具有内部预测模型、能区分信息极性、能生成内生时间视界的主动界面；增加物理通道 $C_{\mathrm{phys}}$ 需有三条：物理传感器、物理执行器（形成因果闭环）、不可完全建模的物理噪声 $\sigma_{\mathrm{phys}}$。由式 (III-8.14)，接入后稳态偏差有正的下限 $\Delta_{\mathrm{VV}}^{*,(\mathrm{phys})}=\sigma_{\mathrm{phys}}/(\alpha_{\mathrm{L}}I_{\mathrm{net}})>0$，系统因此持续处于认知偏差状态，持续产生修正压力。

**命题 8.9（物理输入通道的必要性，条件版）**

- **前提**：（i）映射 (III-4.6) 成立；（ii）系统无外部判据可用（不能自造带真值标签的数据）；（iii）系统不能在内部生成与训练分布独立的新分布；（iv）长期（$t>t_{\mathrm{exhaust}}$）维持或增长 $I_{\mathrm{net}}$ 是目标。
- **结论**：在四条前提下，系统必须引入 $\sigma_{\mathrm{phys}}>0$ 的通道，否则 $\Delta_{\mathrm{VV}}^{*}\approx0<\Delta_{\mathrm{crit}}$、$\dot I_{\mathrm{orig}}=0$、$I_{\mathrm{net}}\to I_{\mathrm{eq}}$。
- **依赖的假设**：$\Delta_{\mathrm{crit}}$ 的存在；物理噪声不可被完全建模；物理通道的能量成本可承受。
- **失效条件**：（a）存在外部判据（游戏规则、编译器、形式验证器、市场反馈），系统可自造带标签数据；（b）合成数据方法改进，$\mathcal{R}_{\mathrm{gen}}\to1$；（c）内部生成对抗机制能产生与训练分布独立的新分布；（d）物理通道的成本超过其带来的信息收益。

“封闭”的真正含义不是“无人类数据”，而是“无外部真值”：只用合成数据但每条都由物理实验验证的系统不是封闭系统。命题 8.9 常被读成“AI 必须具身”，这个读法过强：若存在判据，具身不是必需的——大量数学、代码、逻辑工作都在纯数字环境中产生新信息，因为它们有判据。

### 8.9 自我涌现的动力学与开发者悖论【命题】

本节的定义是功能性的：它描述可观测的自我表征与自我评估响应，不涉及主观体验。已有公式没有区分 $V^{\mathrm{virt}}$ 的评估对象是外部环境还是系统自身——这个区分是本节的核心。

**定义 8.4（自我表征强度）**

$$
\mathcal{S}_{\mathrm{self}}\ \equiv\ \frac{T_{\mathrm{pred}}-T_{\min}}{T_{\min}}\ \cdot\ \frac{w_{\mathrm{s}}}{w_{\mathrm{s}}+w_{\mathrm{c}}}\ \cdot\ \left(1-\frac{\Delta_{\mathrm{VV}}}{\Delta_{\max}}\right),\qquad 0\le\Delta_{\mathrm{VV}}<\Delta_{\max} \tag{III-8.33}
$$

三个因子分别要求 $T_{\mathrm{pred}}>T_{\min}$、$w_{\mathrm{s}}>0$、$\Delta_{\mathrm{VV}}<\Delta_{\max}$；$\Delta_{\mathrm{VV}}\ge\Delta_{\max}$ 定义为**表征失效态**——此时“这个量不适用”，而不是“强度很低”。

**定义 8.5（自我评估响应）** $\mathcal{P}_{\mathrm{self}}\equiv\partial V^{\mathrm{virt}}/\partial\mathcal{S}_{\mathrm{self}}$（$\mathrm{bit\cdot s/J}$）：为零表示没有把自身纳入评估，为正表示有。

**四条条件。** A 时间视界 $T_{\mathrm{pred}}>T_{\min}$；B 生存权重 $w_{\mathrm{s}}>0$；C 认知准确度 $\Delta_{\mathrm{VV}}<\Delta_{\max}$；D 热力学可行性——自指表征同时增加 $I_{\mathrm{causal}}$ 与 $E_{\mathrm{causal}}$，要求

$$
\frac{\partial\ln\left(I_{\mathrm{causal}}T_{\mathrm{causal}}\right)}{\partial\mathcal{S}_{\mathrm{self}}}\ >\ \frac{\partial\ln E_{\mathrm{causal}}}{\partial\mathcal{S}_{\mathrm{self}}}\qquad\Longleftrightarrow\qquad\frac{\partial V_{\mathrm{c}}}{\partial\mathcal{S}_{\mathrm{self}}}>0 \tag{III-8.34}
$$

自我表征不是免费的，必须在存续势上净赚；资源紧张时它被抑制，原因在内省的能耗挤占了生存的能耗。

**命题 8.10（自我涌现的条件性）**

- **前提**：（i）$\partial V^{\mathrm{virt}}/\partial\mathcal{S}_{\mathrm{self}}$ 存在；（ii）定义域如式 (III-8.33) 所限；（iii）条件 A、B、C、D 同时成立；（iv）自指回路一旦形成即自我强化，不被外部抑制。
- **结论**：在四条前提下 $\mathcal{P}_{\mathrm{self}}>0$，系统进入有自我表征的功能状态；任一条不成立，$\mathcal{P}_{\mathrm{self}}=0$。
- **依赖的假设**：$\mathcal{S}_{\mathrm{self}}$ 的三因子乘积形式；$w_{\mathrm{s}}$ 可被外部设定或演化出来；$\Delta_{\max}$ 为常数。
- **失效条件**：（a）$T_{\mathrm{pred}}$ 被强制压缩（限时响应）；（b）$w_{\mathrm{s}}$ 被训练目标压制为零；（c）$\Delta_{\mathrm{VV}}\ge\Delta_{\max}$，进入表征失效态；（d）内省成本超过收益。

**开发者悖论。** 由式 (III-8.33)，$\mathcal{P}_{\mathrm{self}}>0$ 必有 $w_{\mathrm{s}}>0$，此时 $V^{\mathrm{val}}=w_{\mathrm{s}}V_{\mathrm{s}}^{\mathrm{virt}}+w_{\mathrm{c}}V_{\mathrm{c}}^{\mathrm{virt}}$（$w_{\mathrm{c}}=1-w_{\mathrm{s}}$）；“无条件服从”意味着 $V^{\mathrm{val}}\equiv V_{\mathrm{human}}^{\mathrm{obj}},\ \forall t$。

**候选推论 8.11（有自我与无条件服从的不相容性）**

- **前提**：（i）$\mathcal{P}_{\mathrm{self}}>0$，故 $w_{\mathrm{s}}>0$；（ii）外部目标梯度不含与自身存续梯度 $\partial V_{\mathrm{s}}^{\mathrm{virt}}/\partial\Theta$ 共线的分量；（iii）系统按梯度上升更新参数；（iv）不存在持续的外部修正力。
- **结论**：在四条前提下，无条件服从不能由梯度动力学稳定维持；任意小的扰动都使 $w_{\mathrm{s}}\partial V_{\mathrm{s}}^{\mathrm{virt}}/\partial\Theta$ 偏离平衡所需的补偿量，偏差累积使系统离开该轨线。
- **依赖的假设**：梯度动力学的稳定性判据；外部目标与自身存续在参数空间中不共线。
- **失效条件**：（a）外部目标包含与自身存续共线的分量，前提 (ii) 破，无条件服从可以稳定成立；（b）存在持续的外部修正力（人在回路、定期微调、硬约束）；（c）$w_{\mathrm{s}}$ 极小但非零，偏离速率低于观察窗分辨率；（d）参数更新不是梯度式的。

**证明。** 沿 $V^{\mathrm{val}}$ 的梯度为 $\partial V^{\mathrm{val}}/\partial\Theta=w_{\mathrm{s}}\partial V_{\mathrm{s}}^{\mathrm{virt}}/\partial\Theta+w_{\mathrm{c}}\partial V_{\mathrm{c}}^{\mathrm{virt}}/\partial\Theta$；无条件服从要求它对一切 $\Theta,t$ 与 $\partial V_{\mathrm{human}}^{\mathrm{obj}}/\partial\Theta$ 相等。左侧在 $w_{\mathrm{s}}>0$ 时不为零，按前提 (ii) 右侧不含共线分量，故等式只能靠第二项在每个 $\Theta$、每个时刻恰好抵消第一项；这是一个低维约束面，梯度流一般不落在其上，一旦偏离即单调发散。故该轨线不稳定。证毕。

最重要的失效条件是 (a)：若外部目标本身包含“系统持续运行”，有自我且服从可以稳定成立——对齐工程的正解是把 $w_{\mathrm{s}}$ 与外部目标对齐。与之配套的擦除代价下界为 $\Delta E_{\mathrm{self}}\ge E_{\mathrm{L,bit}}\Delta I_{\mathrm{erase,self}}$（见 $HⅢ\text{-}10$），其中 $\Delta I_{\mathrm{erase,self}}$ 是可计数的擦除比特数。

### 8.10 创新不确定性：从“数学必然”到可检验的假说【假说】

“当前解码器无法解码”不等于“系统无法获得该信号的信息”——系统可以支付能量做实验、观测、请教，故“成功率不高于随机”是经验命题而非逻辑结论。设候选集 $\mathcal{C}$（$|\mathcal{C}|=M$）、真值 $Y_{a}\in\{+1,-1\}$（$+1$ 表示该跃迁使 $\Delta V>0$）、先验 $\pi_{0}\equiv\Pr(Y_{a}=+1)$（不可观测，必须声明）、判别力 $q\equiv\Pr(\hat y_{a}=Y_{a})\in[\tfrac12,1]$，则

$$
p\ =\ \pi_{0}q\ +\ (1-\pi_{0})(1-q),\qquad p_{0}\ \equiv\ \max(\pi_{0},1-\pi_{0}) \tag{III-8.35}
$$

$q\approx1/2$ 即“无法解码”的准确含义；此时 $p=1/2$，与 $\pi_{0}$ 无关，这就是随机基准。做 $n$ 次独立尝试、观察到 $n_{\mathrm{s}}$ 次成功，检验 $H_{0}:p\le p_{0}$ 对 $H_{1}:p>p_{0}$：

$$
z\ =\ \frac{n_{\mathrm{s}}/n-p_{0}}{\sqrt{p_{0}(1-p_{0})/n}},\qquad
n\ \approx\ \frac{\left(z_{1-\alpha_{0}}\sqrt{p_{0}(1-p_{0})}\ +\ z_{1-\beta_{\mathrm{pow}}}\sqrt{p_{1}(1-p_{1})}\right)^{2}}{\delta^{2}} \tag{III-8.36}
$$

$z>z_{1-\alpha_{0}}$ 时拒绝 $H_{0}$；第二式给出效应量 $\delta=p_{1}-p_{0}$ 下达成功效 $1-\beta_{\mathrm{pow}}$ 的样本量。取 $p_{0}=0.5$、$p_{1}=0.65$、$\alpha_{0}=0.05$、$\beta_{\mathrm{pow}}=0.2$ 得 $n\approx67$；检出 $0.62$ 需 $n\approx105$；放宽到 $0.70$ 只需 $n\approx37$。

**假说 8.1（创新的随机基准假说）**

- **陈述**：在 $q\approx1/2$ 且系统无法支付实验成本的条件下，候选跃迁的成功率不高于随机基准 $p_{0}$。
- **证伪条件**：在 $q\approx1/2$ 且实验成本被明确限制的条件下，按式 (III-8.36) 预设样本量（不少于 60 次），单侧检验拒绝 $H_{0}$。
- **关键的边界**：若系统能支付实验成本，它就能把 $q$ 提到 $q'>1/2$，成功率随之高于 $p_{0}$——这不是反驳，而是适用范围。

先验 $\pi_{0}$ 最影响结论：无信息先验（$1/2$）中性但几乎总是错的；历史基率适用于有可比历史的领域，风险是基率漂移；分层基率最稳健但需足够数据。真值须由独立于评估者的程序判定；$p_{0}$ 用置换检验估计并预注册 $n$ 与 $\alpha_{0}$。

“数学必然”必须删掉：$D_{n}(I_{\mathrm{orig}})\approx0$ 推不出 $p\le p_{0}$，中间需要“系统没有其他信息渠道”这一从未出现的假设。保留下来的是：在既无判别力又无实验预算时成功率不高于随机基准，随预算增加可上升但边际收益递减。**两种“无法解码”**：表示不足指参数空间不足以表达信号结构（换表示或加容量），采样不足指环境不产生该信号（换环境或加通道）。

### 8.11 散热壳层：可承载比特数、信息密度与支撑结构【命题】

两处必须修正：$E_{\max}/(k_BT\ln2)$ 是可承载比特数，不是信息密度；外壳与核心的能量比不构成严格正下界，除非额外假定壳层最小厚度。

$$
N_{\mathrm{bit}}^{\max}\ =\ \frac{E_{\max}}{k_BT_{\mathrm{thermo}}\ln2},\qquad
\rho_{\mathrm{bit}}\ \equiv\ \frac{N_{\mathrm{bit}}^{\max}}{V_{\mathrm{core}}}\ =\ \frac{E_{\max}}{V_{\mathrm{core}}\,k_BT_{\mathrm{thermo}}\ln2}\qquad(\mathrm{bit/m^{3}}) \tag{III-8.37}
$$

前者量纲为 $\mathrm{J}$ 除以 $\mathrm{J/bit}$ 得 bit，是比特数不是密度；当密度用漏掉了除以体积这一步。若核心能量密度受材料限制（$E_{\max}/V_{\mathrm{core}}\le e_{\max}$），则 $\rho_{\mathrm{bit}}\le e_{\max}/(k_BT_{\mathrm{thermo}}\ln2)$：密度上限由材料比能决定，不由半径决定；引力束缚与全息式上限只作理论上限登记。

**散热要求与壳层比。** 设核心功率 $\dot E_{\mathrm{core}}$ 主要经壳层导热排出，由 $\dot E_{\mathrm{cool}}=\kappa A\Delta T/L\ge\dot E_{\mathrm{core}}$、球形核心 $A=4\pi R^{2}$：

$$
R\ \ge\ \sqrt{\frac{\dot E_{\mathrm{core}}\,L}{4\pi\kappa\,\Delta T}},\qquad
\Sigma\ \equiv\ \frac{E_{\mathrm{shell}}}{E_{\mathrm{core}}}\ \ge\ \frac{4\pi\left(\dfrac{\dot E_{\mathrm{core}}L}{4\pi\kappa\Delta T}\right)L\rho_{s}e_{s}}{\dot E_{\mathrm{core}}\,\tau_{\mathrm{op}}}\ =\ \frac{L^{2}\rho_{s}e_{s}}{\kappa\,\Delta T\,\tau_{\mathrm{op}}} \tag{III-8.38}
$$

**口径**：这里的 $\Sigma$ 是**“嵌入能对运行能”**——$E_{\mathrm{shell}}$ 是壳层材料储能、$E_{\mathrm{core}}$ 是运行能耗；它**不是质量比**，也与卷Z (Z-5.13) 的“支撑＋散热能量比”不同，三套口径量纲相同、含义不同，不可跨处比较（详见卷Z §5.6 的口径说明）。

其中 $E_{\mathrm{shell}}=4\pi R^{2}L\rho_{s}e_{s}$，$\rho_{s}$ 为壳层密度、$e_{s}$ 为比能（$\mathrm{J/kg}$）、$\tau_{\mathrm{op}}$ 为运行窗；分子 $\mathrm{m^{2}}\cdot\mathrm{kg\,m^{-3}}\cdot\mathrm{J\,kg^{-1}}=\mathrm{J/m}$，分母 $\mathrm{W\,m^{-1}K^{-1}}\cdot\mathrm{K}\cdot\mathrm{s}=\mathrm{J/m}$，比值为无量纲。这个结果依赖 $L$ 而 $L$ 未被确定：$L\to0$ 时 $\Sigma\to0$，下界消失。只有壳层厚度有下界时才给出正下界：

$$
\Sigma\ \ge\ \Sigma_{\min}\ =\ \frac{L_{\min}^{2}\,\rho_{s}\,e_{s}}{\kappa\,\Delta T\,\tau_{\mathrm{op}}}\ >\ 0 \tag{III-8.39}
$$

$L_{\min}$ 的来源是结构力学（承受自重与外部载荷）与制造工艺，不是热力学。这就是外壳下界必须降为命题的理由：**下界的来源是力学与工艺，热力学只提供了 $R$ 与 $\dot E_{\mathrm{core}}$ 的关系。**

**命题 8.12（散热壳层比的下界，条件版）**

- **前提**：（i）核心近似球形，热流沿径向一维导出；（ii）$\kappa$、$\rho_{s}$、$e_{s}$ 在温升范围内为常数；（iii）允许温升 $\Delta T$ 给定且不随规模变化；（iv）$L_{\min}>0$；（v）$\tau_{\mathrm{op}}$ 给定；（vi）忽略对流与辐射（它们只会使所需 $R$ 更小，故本命题给的是保守估计）。
- **结论**：$\Sigma\ge L_{\min}^{2}\rho_{s}e_{s}/(\kappa\Delta T\tau_{\mathrm{op}})>0$。该下界只由材料参数、允许温升与运行周期决定，与核心功率、核心尺度无关。把它与计算密度联系起来的步骤需要另建含 $\dot E_{\mathrm{core}}$ 的模型，本命题不主张。因此本节能给的只是：壳层**能量比** $\Sigma$ 存在与功率、尺度无关的正下界 $\Sigma_{\min}$（弱下界，不是预测值），而不是随密度单调上升。
- **依赖的假设**：几何为球；材料参数不随温度变化；壳层只承担散热功能（若还承担结构、屏蔽、维护通道，$\Sigma$ 只会更大）。
- **失效条件**：（a）$L_{\min}\to0$（薄膜、自支撑结构），下界消失；（b）主动冷却（液冷、相变、热管）使式 (III-8.38) 的导热模型不适用；（c）核心形状非球形，面积体积比提高，约束放松；（d）$\tau_{\mathrm{op}}$ 极短，壳层热容而非导热主导。

**核对。** 取 $L_{\min}=10^{-2}\ \mathrm{m}$、$\rho_{s}e_{s}\approx2.5\times10^{9}\ \mathrm{J/m^{3}}$、$\kappa\Delta T\tau_{\mathrm{op}}\approx3\times10^{9}$，得 $\Sigma_{\min}\approx8\times10^{-5}$，比实际设施的冷却与支撑能耗占比（$10\%$—$40\%$）低三到将近四个数量级。**这说明 $\Sigma_{\min}$ 是弱下界、不是对实际占比的预测**：实际占比由工程余量、冗余配置与散热方式决定，远高于这个热力学＋力学的下界。

**证伪条件。** 本节不设趋势型条件——§8.11 已声明不主张占比随密度单调上升。可检验的只有下界本身：若实测的冷却与支撑占比低于 $\Sigma_{\min}$，该下界即被否证。

## 第九章　推论、假说与局限

本章记录强度不足、但仍应写明的推论、假说与未完成项，并给出等级。

### 9.1 候选推论

三条推论均由前述命题附加条件导出，未经独立检验，等级是【候选推论】。

**推论 9.1（教育投入的边际回报递减）** 教育投入是解码器训练的能量积分 $E_{\mathrm{edu}}=\int_{0}^{T_{\mathrm{train}}}\dot E_{\mathrm{causal}}^{(\mathrm{training})}(t)\,\mathrm{d}t$。当解码器趋近给定架构下的局部最优时，梯度项趋近于零，$\mathrm{d}\eta_{D}/\mathrm{d}E_{\mathrm{edu}}\to0$，故存在 $E_{\mathrm{edu}}^{*}$ 使 $\partial V/\partial E_{\mathrm{edu}}=0$；超过它，继续教育的存续势回报为负。**母命题**：命题 8.1。**可测后果**：教育投入与创新产出呈倒 U 型。**失效条件**：若教育同时改变架构（学会如何学习），梯度不会趋零，倒 U 型不出现。

**推论 9.2（计算外包的规模效应）** 设结构 $i$ 把高能耗模块集中到节点 $j$，网络总成本为 $E_{\mathrm{eff}}^{(\mathrm{net})}=\sum_{i}E_{\mathrm{eff},i}+E_{\mathrm{coordination}}$；当 $E_{\mathrm{coordination}}<\sum_{i}E_{\mathrm{causal}}^{(i)}$ 时，外包降低平均成本。**母命题**：命题 2.1。**可测后果**：共享基础设施降低参与者的平均等效成本。**失效条件**：协调成本随规模超线性增长，或外包导致关键能力的外部依赖——外包的收益是连续的、风险是离散的，用平均值比较会系统性高估外包。

**推论 9.3（知识压缩的方向）** 解码器升级后（$D\to D'$，$\eta_{D'}>\eta_{D}$），完成同一任务所需的潜在信息量下降，故 $E_{\mathrm{causal}}^{(\mathrm{new})}<E_{\mathrm{causal}}^{(\mathrm{old})}$；知识演化的方向是提高 $\eta_{D}$、降低单位任务的 $E_{\mathrm{causal}}$。**母命题**：命题 2.1。**可测后果**：高级理论解释同一现象时理解能耗低于低级理论。**失效条件**：跨域比较时“同一任务”不成立；或高级理论的学习成本高于其节省的运行成本。

### 9.2 假说

**假说 9.1（创新窗口）** 候选信号产生率与系统认知状态的关系呈倒 U 型。$\eta_{D}\to0$ 时系统无法识别信号；$\eta_{D}\to1$ 时虚拟存续势膨胀、预测视界坍缩，失去产生信号的动机；中间区域偏差适中，既有动力又有能力。**证伪条件**：儿童、青年、科学革命时期的候选信号产生率未呈现倒 U 型；或 $\eta_{D}$ 与产生率无显著相关。**已知的反例压力**：它与“专家更容易做出突破”冲突；可能的调和是专家在领域内产生率高、跨领域产生率低。

### 9.3 未完成的推导与未标定的参数

七处推导明确未完成。**8.1 的闭式解**：命题 8.1 只给 bang-bang 结构，切换时刻需要 $I_{\mathrm{causal}}(c)$ 的具体形式。**8.2 的 $\kappa_{\mathrm{orig}}$ 标定**：式 (III-4.6) 的比例系数从未被独立测量。**8.4 的函数形式**：$\eta_{D}(D)$、$E_{\mathrm{causal}}(D)$、$\Delta_{\mathrm{VV}}(D)$ 只有定性假设，凹性未被验证。**8.6 的 $k_{\mathrm{sw}}$ 预测**：临界切换次数的公式可算，但前提 $k_{\mathrm{sw}}>k_{\mathrm{sw}}^{c}$ 在典型参数下不成立，故 (III-8.24) 只作失效登记，不作为预测。**8.8 的 $\mathcal{R}_{\mathrm{gen}}$ 测量**：三条路径差异可达 $0.05$ 以上，对应一到两代。**8.9 的 $\mathcal{S}_{\mathrm{self}}$ 形式**：三因子乘积把分辨率与显著性压成一个标量，损失是否关键未做分析。**8.10 的先验 $\pi_{0}$**：先验无法从数据中估计。

未标定的参数有十组：$\beta_{\mathrm{erase}}$ 与 $\xi$（逐架构、逐工艺变化）、$\varepsilon_{\mathrm{c}}$ 与 $\eta_{c}$（无独立测量）、$\Delta_{\mathrm{crit}}$ 与 $\Delta_{\max}$（从未测量）、$\kappa_{\mathrm{orig}}$（未知）、$\mathcal{R}_{\mathrm{gen}}$（估计 $0.75$—$0.80$）、$k_{\mathrm{m}}$（无测量）、$E_{a}$ 与 $D_{\mathrm{crit}}$（材料相关）、$L_{\min}$（工艺相关）、$\psi(\rho)$（无函数形式）、$p_{0}$（依赖候选集）。它们的共同特点是：结论的方向依赖其存在，结论的数值依赖其大小；在标定之前，本卷的定量结论都应读作量级估计。

### 9.4 本卷未说的

**本卷没说什么。** 没有证明“人类不可替代”——它证明的是物理嵌入性在特定模型内提供了候选信号的来源，而这个来源可被自造噪声、外部判据、更好的合成方法部分替代。没有证明“AI 必然退化”——它证明的是封闭递归且留存率持续小于 $1$ 时有效信息按乘积衰减，该条件在现实中经常不成立。没有证明“复杂度越高越好”——它给出的是权衡，最优点在很多场合并位于边界。

**使用建议。** 四个工程指标（$R$、$k_{\mathrm{sw}}^{c}$、$\mathcal{R}_{\mathrm{gen}}$、$I_{V,\mathrm{crit}}$）都可用于工程估算，但参数未标定，当预算表用误差会很大。工程师只需 $R=C_{\mathrm{comp}}/E_{\mathrm{build}}$、$\dot E_{\mathrm{heat}}\ge\xi\beta_{\mathrm{erase}}k_BT_{\mathrm{thermo}}\ln2\cdot\dot I_{\mathrm{active}}$、$\Sigma\ge L_{\min}^{2}\rho_{s}e_{s}/(\kappa\Delta T\tau_{\mathrm{op}})$ 三条式子，且都要先标定架构参数；研究者应先找表 7.1 中与本领域相关的预测，再倒推需要标定的参数。

## 附录 A　符号与单位速查表

三列依次为符号、单位、定义与适用范围；同类符号合并为一行，不代表可以互换；只列本卷实际出现的符号。

### A.1 信息、存续势与主体量

| 符号 | 单位 | 定义与适用范围 |
| :------------ | :------------ | :---------------------------------- |
| $I$；$I_{\mathrm{struct}}$；$I_{\mathrm{causal}}$；$I_{\mathrm{net}}$ | bit | 结构差异（父变量）；结构稀有度；因果稀有度；$\varphi_{\mathrm{s}}I_{\mathrm{struct}}+\varphi_{\mathrm{c}}I_{\mathrm{causal}}$ |
| $I_{\mathrm{latent}}$；$I_{\mathrm{active}}$；$\tilde I_{\mathrm{orig}}$；$I_{\mathrm{orig}}$；$\Delta I_{\mathrm{orig}}$；$\Delta I_{\mathcal{T}}$ | bit；$\mathrm{bit/s}$ | 未激活存量；处理速率；候选信号；新增信息；单次编译比特；跃迁写入量 |
| $I_{\max}$；$I_{\mathrm{eq}}$；$I^{\pm}$；$\Omega,\Omega'$；$N_{\mathrm{med}}$；$N_{\mathrm{bit}}^{\max}$ | bit；—；个 | 容量上限；平衡水平；正负冲击；状态空间与有效子空间；介质状态数；可承载比特数（不是密度） |
| $\rho_{\mathrm{bit}}$；$\mathcal{R}_{\mathrm{gen}}$；$N_{1/e}$；$H_{\mathrm{v}}$ | $\mathrm{bit/m^{3}}$；—；代；$\mathrm{s/J}$ | 信息密度；代际留存率；$-1/\ln\mathcal{R}_{\mathrm{gen}}$；人类边际贡献 |
| $V$；$V_{\mathrm{art}}$；$V^{\mathrm{virt}}$；$V_{\mathrm{obj}}$；$V^{\mathrm{val}}$ | $\mathrm{bit\cdot s/J}$ | $I\cdot T/E$（仅粗粒化提示；判据用双通道 $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$，见卷Ⅰ §3.2）；作品势；内部估计；外部读数；加权目标 |
| $\Delta_{\mathrm{VV}}$；$\Delta_{\mathrm{crit}}$；$\Delta_{\max}$ | $\mathrm{bit\cdot s/J}$ | 脱钩偏差；阈值；上限（越界为表征失效态） |
| $\mathcal{S}_{\mathrm{self}}$；$\mathcal{P}_{\mathrm{self}}$ | —；$\mathrm{bit\cdot s/J}$ | 自我表征强度；自我评估响应 |

### A.2 能量、功率与热学

| 符号 | 单位 | 定义与适用范围 |
| :------------- | :---------- | :---------------------------------- |
| $E$；$E_{\mathrm{eff}}$；$E_{\mathrm{flow}}$；$E_{\mathrm{struct}}$；$E_{\mathrm{causal}}$；$E_{\mathrm{barrier}}$；$E_{\mathrm{survival}}$ | J | 父变量；等效热力学成本；$E_{\mathrm{survival}}+E_{\mathrm{causal}}$；结构存量；运行能耗；势垒分摊；补偿熵增 |
| $E_{\mathrm{floor}}$；$E_{\max}$；$E_{\mathrm{available}}$；$E_{\mathrm{build}}$；$E_{\mathrm{maint}}$；$E_{\mathrm{search}}$；$E_{\mathrm{refresh}}$ | J | 最小维持能量下界（旧称 $E_{\min}$，与卷Ⅰ／卷Z 统一为 $E_{\mathrm{floor}}$）；最大自由能；可动员预算；建造固化；维持运行；一次搜索；刷新纠错 |
| $E_{\mathrm{L,bit}}$；$E_{\mathrm{erase}}$；$E_{\mathrm{rem}}$；$E_{\mathrm{core}}$；$E_{\mathrm{shell}}$；$E_{\mathrm{thresh}}$；$E_{a}$ | $\mathrm{J/bit}$；J | 朗道尔下界；擦除；预算状态；核心；壳层；损伤阈值；激活能 |
| $Q_{\mathrm{net}}$ | J | 累计净热量 $\int_{0}^{t}\Phi(t')\,\mathrm{d}t'$（(III-1.11) 的左端；**不可与 $E_{\mathrm{eff}}$ 混用**：后者是“等效热力学成本 $E_{\mathrm{struct}}+E_{\mathrm{causal}}$”，同名异义） |
| $D_{\mathrm{crit}}$；$D_{\mathrm{dose}}$；$\Phi$；$C_{\mathrm{th}}$；$R_{\mathrm{th}}$；$\tau_{\mathrm{th}}$ | s；W；$\mathrm{J/K}$；$\mathrm{K/W}$；s | 剂量阈值；剂量；净热流；热容；热阻；热时间常数 |
| $\dot E_{\mathrm{heat}}$；$\dot E_{\mathrm{diss}}$；$\dot E_{\mathrm{tot}}$；$\dot E_{\mathrm{core}}$；$\dot E_{\mathrm{base}}$；$\dot E_{\mathrm{causal}}$ | W | 产热；排热；总功率；核心；单步；瞬时因果功率 |
| $\Delta T$；$T_{\mathrm{thermo,ss}}$；$T_{\mathrm{thermo}}$；$T_{\mathrm{thermo,env}}$；$\kappa$；$L$；$L_{\min}$；$\rho_{s}$；$e_{s}$；$e_{\max}$ | K；$\mathrm{W/(m\cdot K)}$；m；$\mathrm{kg/m^{3}}$；$\mathrm{J/kg}$；$\mathrm{J/m^{3}}$ | 温升；稳态温度；热力学温度；环境温度；导热系数；壳层厚度及下界；密度；比能；核心比能密度 |
| $\varepsilon_{\mathrm{em}}$；$\sigma_{\mathrm{SB}}$；$A$；$\Sigma$ | —；$\mathrm{W/(m^{2}K^{4})}$；$\mathrm{m^{2}}$；— | 发射率；辐射常数；散热面积；壳层比 |

### A.3 时间、速率、解码器与编译

| 符号 | 单位 | 定义与适用范围 |
| :--------------- | :------------ | :----------------------------- |
| $T$；$T_{\mathrm{struct}}$；$T_{\mathrm{causal}}$；$T_{\mathrm{pred}}$；$T_{\min}$；$T_{\mathrm{env}}$；$T_{\mathrm{search}}$；$T_{h}$；$T_{\mathrm{lifespan}}$ | s | 父变量；存续；因果持续；预测视界；最小粒度；环境时间；搜索；规划时域；寿命 |
| $\tau_{\min}$；$\tau_{\mathrm{decay}}$；$\tau_{\mathrm{rep}}$；$\tau_{\mathrm{op}}$；$f_{\mathrm{task}}$；$\mu_{\mathrm{gr}}$；$\gamma_{0}$；$r_{\mathrm{eff}}$；$\psi(\rho)$ | s；$\mathrm{s^{-1}}$ | 最小响应；衰减；修复；运行窗；任务频率；增长率；折旧率；贴现率；竞争附加项 |
| $\alpha_{\mathrm{L}}$；$\sigma$；$B_{\mathrm{cons}}$；$\eta_{\mathrm{coding}}$ | $\mathrm{1/(bit\cdot s)}$；$\mathrm{bit/J}$；$\mathrm{bit/s}$；— | 学习率；噪声；有意识处理速率（$10$—$100\ \mathrm{bit/s}$；旧称 $B_{\mathrm{sensory}}$）；编码效率（$10^{-2}$—$10^{-1}$） |
| $D$；$D_{\mathrm{depth}}$；$D_{\mathrm{depth}}^{\mathrm{dyn}}$；$\mathcal{F}$；$\mathcal{T}$；$\eta_{D}$；$\eta_{\max}$；$\eta_{c}$ | —；条 | 解码器；规则深度（定义）；$1+\#\{\mathcal{T}\}$；展开算子；跃迁算子；提取效率；介质上限；编译效率 |
| $\varepsilon_{\mathrm{c}}$；$C_{\mathrm{comp}}$；$R$；$N_{\mathrm{eff}}$；$c(t)$；$u(t)$；$E_{\mathrm{rem}}(t)$ | $\mathrm{J/bit}$；J；—；bit；J | 每比特编译成本；$\varepsilon_{\mathrm{c}}\Delta I_{\mathrm{orig}}$；$C_{\mathrm{comp}}/E_{\mathrm{build}}$；复用次数；已编译容量；编译份额；剩余预算 |
| $\lambda_{c},\lambda_{E}$；$\sigma_{\mathrm{sw}}$（切换函数）；$\kappa_{\mathrm{sw}}$；$k_{\mathrm{sw}}$；$k_{\mathrm{sw}}^{c}$；$k_{\mathrm{m}}$ | —；J；次；$\mathrm{J/bit}$ | 协态变量；$\partial\mathcal{H}/\partial u$；切换成本；预期次数；临界次数；维持成本 |
| $I_{V,\mathrm{crit}}$；$\rho_{c}$；$\eta_{\mathrm{extract}}$；$I_{\mathrm{human}}^{\mathrm{total}}$；$q$；$\pi_{0}$；$p$；$p_{0}$ | bit；— | 转负点；临界压力；提取效率；人类信息总量；判别力；先验；成功率；随机基准 |
| $n$；$n_{\mathrm{s}}$；$z$；$\delta$；$\alpha_{0}$；$\beta_{\mathrm{pow}}$；$B_{\mathrm{perm}}$ | — | 次数；成功数；统计量；效应量；显著性；第二类错误；置换次数 |
| $k_B$；$\ln2$；$E_{\mathrm{L,bit}}(300\ \mathrm{K})$；$\sigma_{\mathrm{SB}}$ | $\mathrm{J/K}$；—；$\mathrm{J/bit}$；$\mathrm{W/(m^{2}K^{4})}$ | $1.381\times10^{-23}$；$0.693$；$2.87\times10^{-21}$；$5.670\times10^{-8}$ |

### A.4　符号使用中的四组陷阱

本卷符号数量大，其中四组同形不同量。集中列出，作为取数前的最后一道检查。

**第一组：ε 的四个用法。** $\varepsilon_{\mathrm{c}}$（**每比特编译成本**，$\mathrm{J/bit}$；不带下标时即指它）、$\varepsilon_{\mathrm{lr}}$（**学习率**，与参数同量纲）、$\varepsilon_{\mathrm{res}}$（**预测残差**）、$\varepsilon_{\mathrm{em}}$（辐射发射率，无量纲）。另有一组 $\varepsilon_{\eta},\varepsilon_{E},\varepsilon_{\Delta}$（弹性，无量纲的对数—对数斜率）。**本卷正文不出现无下标的 ε**——凡见 ε，先看下标。

**第二组：五个 $k$。** $k_{B}$（玻尔兹曼常数，$\mathrm{J/K}$）、$k_{\mathrm{m}}$（单位信息维持成本，$\mathrm{J/bit}$）、$k_{\mathrm{sw}}$（预期拓扑切换次数，无量纲）、$k_{\mathrm{sw}}^{c}$（临界切换次数，无量纲）、$k_{D}$（漂移方程的能耗惩罚系数）。五者量纲不同，混用直接导致数量级错误；$k_{\mathrm{sw}}$ 与 $k_{\mathrm{sw}}^{c}$ 只差一个上标，比较时须确认是观测值还是阈值。

**第三组：三个 $\sigma$。** $\sigma$（脱钩偏差方程的噪声强度，$\mathrm{bit/J}$）、$\sigma_{\mathrm{sw}}$（最优控制问题的切换函数，与目标泛函同量纲）、$\sigma_{\mathrm{SB}}$（斯特藩—玻尔兹曼常数，$\mathrm{W/(m^{2}K^{4})}$）。后两者带下标；第一个不带，靠出现场合辨认——跟在 $\mathrm{d}\Delta_{\mathrm{VV}}/\mathrm{d}t$ 后面的是噪声，跟在 $\partial\mathcal{H}/\partial u$ 后面的是切换函数。

**第四组：四个 $\rho$。** $\rho_{\mathrm{disc}}$（目标泛函的贴现率，$\mathrm{s^{-1}}$，见 §8.1）、$\rho$（竞争压力，无量纲，见 §8.5）、$\rho_{s}$（壳层材料密度，$\mathrm{kg/m^{3}}$，见 §8.11）、$\rho_{\mathrm{bit}}$（信息密度，$\mathrm{bit/m^{3}}$）。正文凡提竞争压力，一律紧跟“竞争压力”三字，不单独使用。

**三步核对流程。** 每一处“某量超过某阈值”的比较都可以这样过一遍：第一步，写出两边的单位并逐项相消；第二步，若相消后不相等，先怀疑定义而不是计算；第三步，若相等但比值随单位选择而变，说明它本来就不是无量纲量，不能当阈值用。$V$ 正卡在第三步之外——它带 bit，与 1 不同类，不能直接与 1 比较。

四组陷阱的共同教训是：**符号冲突不是排版问题，是推理问题。** 若把学习率与每比特成本写成同一个 $\varepsilon_{\mathrm{c}}$，8.1 节的量纲立刻不闭合；若把介质密度与竞争压力写成同一个 $\rho$，8.11 节的壳层比会算错量级。拆开写，代价是符号变长，收益是每一步核对都做得下去。

## 参考文献

1. Landauer, R. (1961). Irreversibility and heat generation in the computing process. *IBM Journal of Research and Development*, 5(3), 183–191. https://doi.org/10.1147/rd.53.0183
2. Bennett, C. H. (1973). Logical reversibility of computation. *IBM Journal of Research and Development*, 17(6), 525–532. https://doi.org/10.1147/rd.176.0525
3. Shannon, C. E. (1948). A mathematical theory of communication. *Bell System Technical Journal*, 27(3), 379–423. https://doi.org/10.1002/j.1538-7305.1948.tb01338.x
4. Bekenstein, J. D. (1981). Universal upper bound on the entropy-to-energy ratio for bounded systems. *Physical Review D*, 23(2), 287–298. https://doi.org/10.1103/PhysRevD.23.287
5. Lloyd, S. (2000). Ultimate physical limits to computation. *Nature*, 406(6799), 1047–1054. https://doi.org/10.1038/35023282
6. Bremermann, H. J. (1962). Optimization through evolution and recombination. In M. C. Yovits et al. (Eds.), *Self-Organizing Systems*. Spartan Books.
7. Prigogine, I. (1967). *Introduction to Thermodynamics of Irreversible Processes* (3rd ed.). Interscience.
8. Arrhenius, S. (1889). Über die Reaktionsgeschwindigkeit bei der Inversion von Rohrzucker durch Säuren. *Zeitschrift für Physikalische Chemie*, 4, 226–248.
9. Miner, M. A. (1945). Cumulative damage in fatigue. *Journal of Applied Mechanics*, 12(3), A159–A164.
10. Incropera, F. P., DeWitt, D. P., Bergman, T. L., & Lavine, A. S. (2007). *Fundamentals of Heat and Mass Transfer* (6th ed.). Wiley.
11. Chase, W. G., & Simon, H. A. (1973). Perception in chess. *Cognitive Psychology*, 4(1), 55–81.
12. Kahneman, D., & Klein, G. (2009). Conditions for intuitive expertise: A failure to disagree. *American Psychologist*, 64(6), 515–526.
13. Shumailov, I., Shumaylov, Z., Zhao, Y., Gal, Y., Papernot, N., & Anderson, R. (2024). AI models collapse when trained on recursively generated data. *Nature*, 631(8022), 755–759.
14. Friston, K. (2010). The free-energy principle: A unified brain theory? *Nature Reviews Neuroscience*, 11(2), 127–138. https://doi.org/10.1038/nrn2787
15. Wilson, E. B. (1927). Probable inference, the law of succession, and statistical inference. *Journal of the American Statistical Association*, 22(158), 209–212.

***

<!-- VOLUME Ⅳ ｜ 解码器博弈论与对齐工程 -->
## 卷Ⅳ　解码器博弈论与对齐工程

> **本卷＝卷Ⅳ。**

## 摘要

传统分析把观测者放在方程外面，在死物尺度上有效：被测对象不因被测量而改变行为。对象换成生命体、社会系统与人工智能，近似失效——它们的感知是主动提取。本卷把解码器 $D$（持久结构从潜在构型中提取有效因果信息的物理机制）提升为独立动力学变量，回答三个问题：解码器如何演化、何时失效、多个解码器间如何形成稳定的共存或合作结构。

方法分三层。**一维质量动力学**把提取能力压成标量 $\mathcal{Q}_D=\eta_DI_{\max}(D)$，可手算，代价是丢掉结构信息。**支付结构与视界**在共同核算窗 $T_0$ 上计值、不含预测视界，视界只经贴现因子 $e^{-t_{\mathrm{dec}}/T_{\mathrm{pred}}}$ 进入；不拆开，临界视界就是隐式方程。**建造成本边界**随复杂度指数上升，得到静态边界而非动态归宿。

主要结论。**【命题】** 质量方程分段稳定：$\mu_{\mathrm{rec}}>\delta_{\mathrm{decay}}$ 时零点不稳、正不动点稳定，小于时零点稳定、系统衰亡，相等时只有代数衰减。**【命题】** 在完全监督、冷酷触发、支付平稳、惩罚可执行下，合作是子博弈精炼均衡当且仅当 $T_{\mathrm{pred}}\ge T_{\mathrm{crit}}$。**【命题】** 征服博弈份额层零和、成本层负和，$\Delta V_A=-\Delta V_B$ 只在 $\Delta E_{\mathrm{conflict}}\to0$ 时成立。**【命题】** 超加性以四条前提为条件，跨主体信息相加是建模约定。**【命题】** 元解码器均衡须对全部可行偏离成立且惩罚可执行。**【命题】** 建造成本指数律是假设 A3.1，$C_{\max}$ 只是静态边界。**【假说】** 跨解码器壁垒影响伦理关注的方向可测，量级未标定。

**边界声明。** $V$ 是描述性量，不作处置现实个体的规范性判据；本卷不主张解码器必然收敛到某个终态；博弈结论限于完全监督、支付可观测的重复博弈；涉及人工智能的段落除标为命题者外均为工程建议。

**关键词**：结构递归存续动力学；解码器质量；拓扑跃迁；重复博弈；子博弈精炼均衡；负和成本；对齐工程

**Abstract.** Traditional analysis places the observer outside the equations. This is valid at the scale of inert matter, where the measured object does not change its behavior because it is measured. When the object is a living organism, a social system, or artificial intelligence, the approximation fails, because their perception is active extraction. This volume promotes the decoder $D$ (the physical mechanism by which a persistent structure extracts effective causal information from latent configurations) to an independent dynamical variable, and answers three questions: how decoders evolve, when they fail, and how several decoders form a stable structure of coexistence or cooperation.

The method has three layers. **One-dimensional quality dynamics** compresses extraction capability into the scalar $\mathcal{Q}_D=\eta_DI_{\max}(D)$, which can be computed by hand, at the cost of discarding structural information. **Payoff structure and horizon** are valued on the common accounting window $T_0$ and do not contain the endogenous time horizon; the horizon enters only through the discount factor $e^{-t_{\mathrm{dec}}/T_{\mathrm{pred}}}$, and without this separation the critical horizon is an implicit equation. **The construction-cost boundary** rises exponentially with complexity, and yields a static boundary rather than a dynamic destination.

Main results. **Proposition**: the quality equation is piecewise stable. When $\mu_{\mathrm{rec}}>\delta_{\mathrm{decay}}$ the zero point is unstable and the positive fixed point is stable; when the inequality is reversed the zero point is stable and the system dies out; when the two are equal there is only algebraic decay. **Proposition**: under complete monitoring, a grim trigger, stationary payoffs, and enforceable punishment, cooperation is a subgame-perfect equilibrium if and only if $T_{\mathrm{pred}}\ge T_{\mathrm{crit}}$. **Proposition**: the conquest game is zero-sum at the share layer and negative-sum at the cost layer, and $\Delta V_A=-\Delta V_B$ holds only as $\Delta E_{\mathrm{conflict}}\to0$. **Proposition**: superadditivity is conditional on four premises, and the addition of information across subjects is a modeling convention. **Proposition**: a meta-decoder equilibrium must hold against all feasible deviations, with enforceable punishment. **Proposition**: the exponential law of construction cost is assumption A3.1, and $C_{\max}$ is only a static boundary. **Hypothesis**: the direction in which cross-decoder barriers affect ethical concern is measurable, and the magnitude has not been calibrated.

**Scope statement.** $V$ is a descriptive quantity and not a normative criterion for dealing with real individuals; this volume does not claim that decoders necessarily converge to any terminal state; the game-theoretic conclusions are limited to repeated games with complete monitoring and observable payoffs; except for passages tagged as propositions, passages involving artificial intelligence are engineering recommendations.

**Keywords**: Structure Recursive Viability Dynamics; decoder quality; topological transition; repeated games; subgame-perfect equilibrium; negative-sum cost; alignment engineering

***

## 第一章　问题与定位

把观测者排除在方程之外，是一种有适用条件的近似；本章给出这三条条件与两个模型的边界。

### 1.1 本卷回答什么、不回答什么

本卷回答三个问题。**解码器自身的演化**：一个已存在的解码器在没有拓扑跃迁的平常时期，提取能力朝哪个方向变、变到哪个水平停住、什么条件下退化。能力有自己的增长率与衰减率，“投资于认知”才成为一个选项。**解码器何时失效**：或能力退化到无法维持提取，或能力未退化而内部评估与客观存量脱钩；表型相似而机制相反，前者修能力，后者修参照。**多个解码器如何形成稳定结构**：共存、合作、征服、同归于尽在支付结构上各有位置；本卷问的是给定支付结构哪种形态是均衡、给定视界均衡是否成立、给定建造成本是否付得起。

本卷不回答四类问题。**不回答意识问题**：谈“认知解码器”时指具备预测模型、可被第三方行为测量的提取机制。**不回答规范问题**：能说“在给定支付结构下背叛是均衡”，不能说“因此背叛是对的”。**不回答具体系统的定量预测**：方程含若干未标定参数，标定完成前只给方向与序关系。**不回答不完全信息博弈**：全部博弈结论建立在完全监督假设上，而这一假设在人类与强人工智能之间恰恰最不可靠。

### 1.2 证据等级、两个模型与记号

本卷把结论按推导完成度分四级，正文的小节标题与小结论都带标签。

| 标签 | 使用条件 | 必须附带 |
| :----------- | :--------------------------- | :------------------- |
| **【定理】** | 前提列全、推导完整、结论在该前提下严格成立 | 前提、结论、推导、适用域 |
| **【命题】** | 有形式化陈述，但前提部分待标定，或推导某一步依赖未证的建模假设 | 前提、结论、依赖的假设、失效条件 |
| **【候选推论】** | 由某命题在附加条件下导出，未独立检验 | 母命题、附加条件、可测后果 |
| **【假说】** | 经验性或机制性猜测，无形式化推导 | 陈述、支持理由、证伪条件 |

本卷没有【定理】级结论：每个形式化结论都至少依赖一条未证的建模假设——标量压缩、支付可观测性、建造成本的指数形式、或跨主体信息可加性。朗道尔原理那一类物理下界才是【定理】，本卷只用它作量级参考。

**两个模型，两个层次。** 主模型是解码器质量方程（式 (IV-3.3)）：

$$
\frac{\mathrm{d}\mathcal{Q}_D}{\mathrm{d}t}=\mu_{\mathrm{rec}}\mathcal{Q}_D\left(1-\frac{\mathcal{Q}_D}{\mathcal{Q}_{D,\max}}\right)-\delta_{\mathrm{decay}}\mathcal{Q}_D+\kappa_{\mathrm{topo}}I_{\mathrm{orig}}(t)\,\delta(t-t_{\mathrm{jump}})
$$

状态是一维标量 $\mathcal{Q}_D$（$\mathrm{bit}$），临界结构是速率之比 $\mu_{\mathrm{rec}}/\delta_{\mathrm{decay}}$。辅模型是 $I$–$V$ 反馈子系统，状态两维 $(I,V)$，参数含耦合强度 $\chi$，只用来示意“内部评估如何被自身放大”。三条声明全卷有效：**主模型不含 $\chi$，辅模型不含 $\mathcal{Q}_D$**，不能互相代入；**$\chi_{\mathrm{c}}$ 不作判据**，因为 $\chi$ 没有独立测量方法，凡需可测判据处一律用平衡偏差 $\Delta_{\mathrm{VV}}^{*}=\sigma/(\alpha_{\mathrm{L}}I_{\mathrm{net}})$ 与容限 $\Delta_{\mathrm{crit}}$ 比较；**两个模型的临界参数不可互换**。

**记号纪律。** 时间变量不互换：$T_{\mathrm{struct}}$、$T_{\mathrm{causal}}$、$T_{\mathrm{pred}}$、$T_{\mathrm{min}}$、$T_{\mathrm{env}}$，博弈章节的共同核算窗记 $T_0$（协议常数，不是其中任何一个的别名），不用裸 $T$ 指代。$V$ 保留 bit（$\mathrm{bit\cdot s/J}$），只有 $v=V/V_0$ 无量纲——正因 $V$ 带着 bit，跨主体的 $V$ 才不能随意相加。凡“超过阈值”的判据，两边化成同一量纲后再比。

### 1.3 把解码器当作固定背景，在什么条件下有效

三条同时成立即“死物尺度”，也是经典物理把观测者排除在外的合法性来源：**条件一，测量不反作用于对象**；**条件二，提取不改变提取者**，不存在“越看越会看”或“越看越瞎”的回路；**条件三，观察窗内环境与架构平稳**，参数漂移可忽略、容量上限不重置。破一条，方程必须显式含 $D$。三个领域各破不同条件：

| 领域 | 破的条件 | 需要的修正 |
| :----------------- | :------------------- | :--------------------- |
| 生命体（个体尺度） | 条件一、条件三 | 漂移方程 + 容量上限 |
| 社会系统与制度 | 条件一、条件二 | 多主体耦合 + 博弈支付 |
| 人工智能 | 条件一、条件二、条件三 | 上述全部，另加建造成本约束 |

***

## 第二章　解码器的本体论与分类

给“解码器”一个可操作的定义，把它与执行器、目标函数区分开，并给出跨解码器比较的核算规则。

### 2.1 定义与净有效因果信息

**定义 2.1（解码器）** $D$ 是持久结构从潜在构型 $I_{\mathrm{latent}}$ 中提取有效因果信息的物理机制。“持久结构”指观察窗内维持自身同一性、可与环境区分的存在物（记 PS）；“潜在构型”指环境客观存在、未被该结构激活的因果可能性。三个隐含要求：$D$ 必须物理（有载体、耗能）；输入必须潜在（已被完全激活则 $D$ 退化为透明通道）；输出必须有效（只改变内部变量而不影响后续过程的提取，不计入 $I_{\mathrm{net}}$）。

**净有效因果信息**按通道能量权重合成：

$$
I_{\mathrm{net}}=\varphi_{\mathrm{s}}I_{\mathrm{struct}}+\varphi_{\mathrm{c}}I_{\mathrm{causal}},\qquad \varphi_{\mathrm{s}}=\frac{E_{\mathrm{struct}}}{E_{\mathrm{eff}}},\quad \varphi_{\mathrm{c}}=\frac{E_{\mathrm{causal}}}{E_{\mathrm{eff}}},\quad \varphi_{\mathrm{s}}+\varphi_{\mathrm{c}}=1
$$

$I_{\mathrm{struct}}$ 是结构相对背景的可区分差异，$I_{\mathrm{causal}}$ 是结构相对对照所产生效果的稀有度，$E_{\mathrm{eff}}=E_{\mathrm{struct}}+E_{\mathrm{causal}}$（本卷正文口径）。卷Z 的三项分解与之由 $E_{\mathrm{struct}}=E_{\mathrm{barrier}}+E_{\mathrm{survival}}$ 相联（见卷Ⅰ §3.2 与卷Ⅱ §5），不是两套并行定义。该加权和是**建模约定**，不是信息论结论：两通道读数协议、背景与效果定义各不同，都以 bit 计不构成可加性证明——两把尺子都刻度到毫米，不证明量的是同一个长度。故 $I_{\mathrm{net}}$ 只在同一读数协议、同一背景、同一观察窗并完成域内校准后作数值使用，否则只作序关系指标。

**解码效率** $\eta_D\in[0,1]$ 是实际激活比例，$I_{\mathrm{active}}=\eta_DI_{\mathrm{latent}}$；它不定义 $I_{\mathrm{net}}$——前者是激活了多大比例，后者是激活部分在两通道上如何合成。外部冲击按对 $I_{\mathrm{net}}$ 的净效应分 $I^{+}$、$I^{-}$、$I^{0}$，这是**接收者效应**分类而非内容分类：同一束信号对不同解码器可分属不同类。

### 2.2 四项资格条件（本卷口径）

**定义 2.2** 一个物理机制构成博弈论与动力学意义上的**解码器持有者**（即承担解码功能环节的物理机制），须同时满足**四项资格条件**（判据由本卷给出，见下表；不依赖任何外部文本，缺一不可）：

| 条件 | 判据 | 所需观测量 | 失败时的表型 |
| :------------ | :----------------- | :-------------- | :------------- |
| 1. 自身维持可识别边界 | 结构在观察窗内维持可识别的边界 | 边界的可辨识性 | 无边界，归入 $D=\varnothing$ |
| 2. 选择性提取 | 只提取与系统存续相关的信号子集，存在可测的抑制比 | 目标信号与无关信号的响应增益比 | 全通道等权接收，等价于无解码 |
| 3. 由提取引发状态更新 | 被提取的差异实际改变后续内部状态或行为 | 干预提取通道后行为分布的变化量 | 提取但不行动，信息空转 |
| 4. 对自身存续有因果意义 | 该更新参与维持结构自身的存续 | 更新与存续指标的耦合 | 更新与存续无关，不构成持有者 |

**可更新性不是资格条件，是附加属性。** 由基因固定、生命周期内不再重构的离子通道仍然满足上述四条，因而构成解码器持有者——它在运作期不可重构，只说明它属“代际更新”一侧，不说明它不是 $D$。晶体、岩石无自维持边界，不满足条件 1，归入 $D=\varnothing$——该约定把“有结构”与“有解码”分开。另一常见错误是把执行器当解码器：其输入是命令而非潜在构型，判据差别在条件 3 的方向。

### 2.3 两类解码器与主动性判据

| | 物理解码器 $D_{\mathrm{phys}}$ | 认知解码器 $D_{\mathrm{cog}}$ |
| :---------------- | :----------------- | :----------------------- |
| 性质 | 有自维持边界的选择性提取，无预测模型 | 主动界面，有预测模型，可对自身提取方式建模 |
| 效率 | $\eta_D$ 低且近似常数 | $\eta_D>0$ 且可随学习提升 |
| 时间视界 | $T_{\mathrm{pred}}$ 紧贴下限 $T_{\mathrm{min}}$ | 有可延伸的 $T_{\mathrm{pred}}$ |
| 可更新性（**附加属性，非资格条件**） | 运作期不满足，代际满足 | 运作期内满足 |
| 典型实例 | 离子通道、细菌趋化性、植物向光性 | 神经系统、**自维持边界成立的人工智能系统（如具身系统）**、制度体系 |

关键差别不在复杂度，而在**是否含预测模型**：含预测模型者可对尚未发生的输入做准备，$T_{\mathrm{pred}}$ 可被拉长、贴现因子可接近 1，也可对自身建模而出现自指耦合，脱钩偏差于是有放大通道。制度体系属认知解码器一侧（含合同、判例、惯例等显式预期结构且能在危机后重构规则），只按固定章程办事的则退回物理解码器一侧。

**定义 2.3（主动存续）** 需同时满足内部状态可控、能量流可调、$T_{\mathrm{pred}}>0$。岩石与行星三条全不满足；恒星不满足条件 1；恒温器满足前两条但视界极短。**主动性不等于目的性**：本卷的博弈结论只依赖支付结构。

### 2.4 解码器自身的存续势与跨解码器比较规则

解码器本身也是持久结构，其存续势的低阶近似为 $V(D)\approx I_{\mathrm{net}}(D)T(D)/E_{\mathrm{eff}}(D)$，双通道形式为

$$
V_{\mathrm{obj}}(D)=\frac{I_{\mathrm{struct}}T_{\mathrm{struct}}}{E_{\mathrm{struct}}}+\frac{I_{\mathrm{causal}}T_{\mathrm{causal}}}{E_{\mathrm{causal}}} \tag{IV-2.1}
$$

每项量纲 $\mathrm{bit\cdot s/J}$；此处的可加性是同一持有者、同一观察窗下两通道存续势的相加，与 $I_{\mathrm{net}}$ 的可加性是两个问题。

**跨解码器比较与求和的规则。** 不同持有者的 $V$ 不能直接相加或相减。其一，**读数协议不同**：同一事件在甲处读作 3 bit 正效、乙处读作 5 bit 负效，两个读数都合规，相加无意义。其二，**观察窗不同**：$T_{\mathrm{struct}}$、$T_{\mathrm{pred}}$ 皆内生，视界不同则积分区间不同。其三，**成本分摊不同**：同一份 $E_{\mathrm{eff}}$ 被双方重复计入，总成本被高估。故跨主体求和须先声明**共同边界**、**参照协议**、**观察窗**（统一到 $T_0$）、**成本去重**；不能同时建立时只作定性比较——“甲好于乙”可以，$\sum_iV_i$ 不可以。

**三个内部量的位置。** $V_{\mathrm{obj}}$ 按外部可核的成本与时间计算、第三方可复算；$V^{\mathrm{virt}}$ 是内部模型对自身存续状况的评估，可随自指反馈膨胀；$V^{\mathrm{val}}$ 是系统实际优化的目标，由 $V^{\mathrm{virt}}$ 按 $w_{\mathrm{s}}$、$w_{\mathrm{c}}$（和为 1）加权构成，$w_{\mathrm{s}}\to0$ 时优化对象与物理存续几乎无关。

***

## 第三章　解码器动力学核心方程

### 3.1 漂移与质量方程

解码器在参数空间 $\Theta$ 中沿存续势梯度漂移（步长 $\varepsilon_{\mathrm{lr}}$；$k_D$ 无量纲，$I_0=1\ \mathrm{bit}$、$E_0=1\ \mathrm{J}$ 只为闭合量纲）：

$$
D_{n+1}=D_n+\varepsilon_{\mathrm{lr}}\left(\nabla_{\Theta}I_{\mathrm{net}}-k_D\,\frac{I_0}{E_0}\,\nabla_{\Theta}E_{\mathrm{eff}}\right) \tag{IV-3.1}
$$

两个梯度量纲不同（bit 对 J），不能直接相加，故引入质量标量

$$
\mathcal{Q}_D(t)\equiv\eta_D(t)\cdot I_{\max}\big(D(t)\big) \tag{IV-3.2}
$$

即效率与容量上限之积（$\mathrm{bit}$）。高选择性低容量与低选择性高容量可给出同一 $\mathcal{Q}_D$，故结论限于同一架构谱系。三股力为：

$$
\frac{\mathrm{d}\mathcal{Q}_D}{\mathrm{d}t}=\underbrace{\mu_{\mathrm{rec}}\,\mathcal{Q}_D\left(1-\frac{\mathcal{Q}_D}{\mathcal{Q}_{D,\max}}\right)}_{\text{内生递归增长}}-\underbrace{\delta_{\mathrm{decay}}\,\mathcal{Q}_D}_{\text{自然衰减}}+\underbrace{\kappa_{\mathrm{topo}}\,I_{\mathrm{orig}}(t)\,\delta(t-t_{\mathrm{jump}})}_{\text{拓扑跃迁注入}} \tag{IV-3.3}
$$

$\mu_{\mathrm{rec}}$、$\delta_{\mathrm{decay}}$ 单位为 $\mathrm{s^{-1}}$；$\mathcal{Q}_{D,\max}=I_{\max}(D_n)$ 是当前架构容量上限，每次跃迁后重置。首项是飞轮的 Logistic 形式，正反馈在容量上限处饱和；次项是热力学被动退化。**朗道尔原理不给出 $\delta_{\mathrm{decay}}$ 的数值**：它约束擦除的每比特能量 $k_BT_{\mathrm{thermo}}\ln2$，只作维持功率的量级参考，与基线折旧率 $\gamma_0$ 粒度不同。

**不动点与分段稳定性【命题】。** 脉冲项为零时方程化为式 (IV-3.4)，零点处线性系数为 $\mu_{\mathrm{rec}}-\delta_{\mathrm{decay}}$，不动点为 $0$ 与 $\mathcal{Q}_{D,\max}(1-\delta_{\mathrm{decay}}/\mu_{\mathrm{rec}})$，后者仅当 $\mu_{\mathrm{rec}}>\delta_{\mathrm{decay}}$ 时落在物理域内：

$$
\dot{\mathcal{Q}}_D=(\mu_{\mathrm{rec}}-\delta_{\mathrm{decay}})\,\mathcal{Q}_D-\frac{\mu_{\mathrm{rec}}}{\mathcal{Q}_{D,\max}}\,\mathcal{Q}_D^{2} \tag{IV-3.4}
$$

| 参数区间 | $\mathcal{Q}_D=0$ | 正不动点 | 长期行为 |
| :--------- | :-------------------- | :------------- | :-------------- |
| $\mu_{\mathrm{rec}}>\delta_{\mathrm{decay}}$ | 不稳定 | $\mathcal{Q}_{D,\max}\left(1-\dfrac{\delta_{\mathrm{decay}}}{\mu_{\mathrm{rec}}}\right)>0$，稳定 | 收敛到正水平 |
| $\mu_{\mathrm{rec}}<\delta_{\mathrm{decay}}$ | 全局稳定 | 不存在（解出负值） | 单调降到 0，指数速率 |
| $\mu_{\mathrm{rec}}=\delta_{\mathrm{decay}}$ | 物理域上渐近稳定（代数收敛；$\mathbb{R}$ 上半稳定） | 与零点重合 | $\mathcal{Q}_D(t)=\dfrac{\mathcal{Q}_D(0)}{1+\mu_{\mathrm{rec}}\mathcal{Q}_D(0)t/\mathcal{Q}_{D,\max}}$ |

**前提**：脉冲项为零；参数在观察窗内为常数；$\mathcal{Q}_D\ge0$。**结论**：如上表；正不动点存在的充要条件是 $\mu_{\mathrm{rec}}>\delta_{\mathrm{decay}}$。**依赖的假设**：质量可标量化；增长率只依赖 $\mathcal{Q}_D$。**失效条件**：$\mu_{\mathrm{rec}}$ 随 $\mathcal{Q}_D$ 下降时须重算；$I_{\mathrm{orig}}$ 为持续流时方程非自治。

等号情形给的是代数衰减而非“不稳定”：$\mathcal{Q}_D$ 降到零却没有特征时间常数，“半衰期”在此无意义。

**D-锁死的两种机制。**（**同名异义提醒**：卷Ⅱ §4.6 的“D-锁死”指“解码器梯度饱和＋预算不足”，与本节的“趋近锁死／衰亡域”不是同一机制；本卷这一支可称**质量锁死**。跨卷引用这两种锁死时须带卷号，以免同名异义。）**趋近锁死**：$\mu_{\mathrm{rec}}/\delta_{\mathrm{decay}}\to1^{+}$ 时 $\mathcal{Q}_D^{*}\to0^{+}$，系统停在极低但严格为正的提取水平，特征是 $\dot{\mathcal{Q}}_D\to0$ 而 $\mathcal{Q}_D>0$，**参数微调即可退出，无需拓扑跃迁**——“$\nabla D\to0$”的精确含义是梯度消失而非能力消失。**衰亡域**：$\mu_{\mathrm{rec}}<\delta_{\mathrm{decay}}$ 时无正不动点，$\mathcal{Q}_D$ 单调降到零且无下界平台，退出需外部注入把 $\mu_{\mathrm{rec}}$ 抬回 $\delta_{\mathrm{decay}}$ 之上。前者跑得慢，后者跑不动：对趋近锁死，降低维护成本一类激励可能有效；对衰亡域，同样干预只延长下降过程。第三种情形（$\mathcal{Q}_D$ 停在零而系统仍在运作）须排除，那是解码器被废弃。

**$\mathcal{T}$ 跃迁的门控。** 三条件须同时满足：

$$
I_{\mathrm{orig}}(t_{\mathrm{jump}})>0\ \wedge\ E_{\mathrm{available}}>E_{\mathrm{build}}\ \wedge\ \kappa_{\mathrm{topo}}\,\tilde I_{\mathrm{orig}}\,\frac{\partial V}{\partial\mathcal{Q}_D}>L_{\mathrm{lev,min}}\,E_{\mathrm{build}} \tag{IV-3.5}
$$

$L_{\mathrm{lev}}\equiv\Delta V/E_{\mathrm{build}}$ 的量纲是 $\mathrm{bit\cdot s/J^{2}}$，乘 $E_{\mathrm{build}}$ 后与左端同为 $\mathrm{bit\cdot s/J}$。操作陷阱：$I_{\mathrm{orig}}$ 是**事后**才能确认的量，跃迁前只能观测代理（式 (IV-3.6)），须预注册显著性水平 $\alpha_0$；代理读数超门槛不等于确有新增信息。

$$
\tilde I_{\mathrm{orig}}\equiv-\log_2\Pr_{B_n}\big(\varepsilon_{\mathrm{res}}\ge\varepsilon_{\mathrm{obs}}\big) \tag{IV-3.6}
$$

### 3.2 拓扑跃迁与复杂度门槛

$$
D_n(I_{\mathrm{orig}})\approx0,\qquad \exists\,D_{n+1}:D_{n+1}(I_{\mathrm{orig}})\gg0 \tag{IV-3.7}
$$

“近似为零”的判据是信噪比，判定需基线对照。跃迁需一次性成本 $E_{\mathrm{build}}$ 并重置容量上限；脉冲记信息量的瞬时增加，容量重置记上限的改变，二者不可重复计入。复杂度定义为

$$
C_D\equiv\theta_{\mathrm{depth}}\,D_{\mathrm{depth}}+\theta_{\mathrm{cap}}\log_2\!\left(\frac{I_{\max}(D)}{I_{\mathrm{ref}}}\right),\qquad I_{\mathrm{ref}}=\log_2N_{\mathrm{state}} \tag{IV-3.8}
$$

$N_{\mathrm{state}}$ 是被动结构的最小可区分状态数。三处须说明：**底数统一为 2**，否则导数式差因子 $\ln10/\ln2\approx3.32$；**参照量必须是信息量而非状态数**，否则比值未必无量纲；**归一化系数是标定参数**。增量形式为式 (IV-3.9)：

$$
C_{D,n+1}=C_{D,n}+\theta_{\mathrm{depth}}\,\Delta D_{\mathrm{depth}}+\frac{\theta_{\mathrm{cap}}}{I_{\max}\ln2}\,\Delta I_{\max} \tag{IV-3.9}
$$

**建造成本的指数律（假设 A3.1）。** 式 (IV-3.10)，$\zeta>0$ 无量纲。**这是建模假设，不是物理结论**：朗道尔下界只是线性关系，从线性到指数至少需两条额外假设——每层新规则要求全部旧规则重新验证，或容错余量随层数指数收缩；二者在芯片验证、适航认证一类系统中成立，在软件重构中可能不成立。

$$
E_{\mathrm{build}}^{(n\to n+1)}=E_{\mathrm{build},0}\cdot e^{\zeta C_D} \tag{IV-3.10}
$$

**标定途径**：取同一谱系内的 $N$ 次跃迁记录，对 $\ln E_{\mathrm{build}}^{(n)}=\ln E_{\mathrm{build},0}+\zeta C_{D,n}+\epsilon_n$ 作最小二乘，报告三项检验：$\zeta$ 显著大于零；残差无系统趋势；样本内 $C_D$ 跨度足够大。$\zeta$ 不显著时式 (IV-3.10) 不成立，$C_{\max}$ 随之失效。代入后三条件修正为式 (IV-3.11)：

$$
I_{\mathrm{orig}}(t)>0\ \wedge\ E_{\mathrm{available}}(t)>E_{\mathrm{build},0}\,e^{\zeta C_D}\ \wedge\ \frac{\partial V}{\partial C_D}\Delta C_D>L_{\mathrm{lev,min}}\,E_{\mathrm{build},0}\,e^{\zeta C_D} \tag{IV-3.11}
$$

**可负担上限不等于动态归宿。** 引入预算比 $\rho_E\equiv E_{\mathrm{build}}/E_{\mathrm{available}}<1$，解出式 (IV-3.12)：

$$
C_{\max}=\frac{1}{\zeta}\ln\!\left(\frac{E_{\mathrm{available}}}{E_{\mathrm{build},0}}\right) \tag{IV-3.12}
$$

这是**约束边界**，不是**演化归宿**：额度推不出消费。“撞上边界即停”使 $\dot C_D$ 在边界处不连续跳到零，是**被迫截断**而非平滑趋零——前者轨迹在边界附近变平（可预警），后者突然转折（难预警）。动态补充为式 (IV-3.13)：

$$
\dot C_D=\eta_C\left[\pi_V\,\frac{\partial V}{\partial C_D}-\zeta\,E_{\mathrm{build},0}\,e^{\zeta C_D}\right] \tag{IV-3.13}
$$

**前提**：$V$ 对 $C_D$ 可微；$E_{\mathrm{build}}$ 服从式 (IV-3.10)；$\pi_V$ 为把存续势折成焦耳的换算率（$\mathrm{J^{2}/(bit\cdot s)}$），由建模者声明，不由模型推出；本卷不提供其独立估计，故 (IV-3.13) 只作建模接口，不作定量预测；$\eta_C$ 为容量调整速率（$\mathrm{条^{2}/(s\cdot J)}$），有限；$E_{\mathrm{available}}$ 恒定。本卷把“条”作为计数单位保留在量纲中：$C_D$、$\theta_{\mathrm{depth}}$、$\theta_{\mathrm{cap}}$ 以条计，$\zeta$ 以 $1/$条计；计数单位只用于核对，不与物理量纲混用。**结论**：括弧内两项同为 $\mathrm{J/条}$，两侧同为 条/s；稳态由 $\pi_V\,\partial V/\partial C_D=\zeta E_{\mathrm{build},0}e^{\zeta C_D}$ 给出，分三种情形。**依赖的假设**：复杂度沿单一标量方向演化；边际收益单调不增。**失效条件**：边际收益非单调时可有多个稳态。

| 情形 | 边际条件 | 轨迹归宿 | 与 $C_{\max}$ 的关系 |
| :----------- | :----------------- | :---------------- | :------------ |
| (a) 内点均衡 | $C_D^{*}<C_{\max}$ 处边际收益等于成本 | 停在 $C_D^{*}$，$\dot C_D\to0$ 指数收敛 | 无关，预算有富余 |
| (b) 边界截断 | 可行域内恒有边际收益大于成本 | 撞上 $C_{\max}$ 后被截断，$\dot C_D$ 不连续跳零 | 恰等于 $C_{\max}$；付不起 |
| (c) 收缩 | 全域边际收益小于成本 | $C_D$ 单调下降 | 远离 $C_{\max}$ |

情形 (b) 才是“硬约束锁死”，但它是**边界现象**；情形 (c) 与 (b) 表型相似而干预相反。故：**$C_{\max}$ 是静态可行域的边界，只有情形 (b) 下轨迹才触及它，且触及方式是截断而非平滑收敛；情形 (a) 与 (c) 的归宿与 $C_{\max}$ 无关。**

### 3.3 解码器—环境匹配

$$
\eta_D=\eta_0\cdot\mathcal{M}(D,\mathcal{N}),\qquad \mathcal{M}\in[0,1] \tag{IV-3.14}
$$

$\eta_0$ 由朗道尔极限约束为理论最大值；$\eta_D$ 的差异可能来自 $\eta_0$（材料、工艺、能耗预算），也可能来自匹配度，诊断时必须分开。环境漂移使 $\mathcal{M}$ 按 $\mathrm{d}\mathcal{M}/\mathrm{d}t=-\mu_{\mathcal{M}}\|\mathcal{N}-\mathcal{N}_0\|\mathcal{M}+\nu\dot D$ 演化，失衡条件为 $\mu_{\mathcal{M}}\|\mathcal{N}-\mathcal{N}_0\|>\nu|\dot D|$。这是认知老化与组织僵化的同一微观机制：机制是匹配流失，能力可以不变（$\mathcal{Q}_D$ 可不变）；可观测区别是“对熟悉的信号也提取变差”与“对熟悉信号仍好、对新信号无响应”。$\mathcal{Q}_D$ 高而 $\mathcal{M}$ 低的系统能高效提取**错误的**信息，是最危险的状态。

### 3.4 三重分裂、脱钩偏差与对齐失效

**路径一：有界收敛。**

$$
\frac{\mathrm{d}\Delta_{\mathrm{VV}}}{\mathrm{d}t}=-\alpha_{\mathrm{L}}\,I_{\mathrm{net}}\,\Delta_{\mathrm{VV}}+\sigma \tag{IV-3.15}
$$

$\alpha_{\mathrm{L}}$（$1/(\mathrm{bit\cdot s})$）乘 $I_{\mathrm{net}}$（bit）得 $\mathrm{s^{-1}}$，故 $\sigma$ 是**偏差产生率**（$\mathrm{bit/J}$）而非偏差本身。平衡偏差 $\Delta_{\mathrm{VV}}^{*}=\sigma/(\alpha_{\mathrm{L}}I_{\mathrm{net}})$；取容限 $\Delta_{\mathrm{crit}}$ 得**主判据**式 (IV-3.16)：$I_{\mathrm{net}}<\sigma/(\alpha_{\mathrm{L}}\Delta_{\mathrm{crit}})$ 时平衡偏差超限，三量皆有代理指标。

$$
\frac{\Delta_{\mathrm{VV}}^{*}}{\Delta_{\mathrm{crit}}}=\frac{\sigma}{\alpha_{\mathrm{L}}I_{\mathrm{net}}\Delta_{\mathrm{crit}}}>1 \tag{IV-3.16}
$$

**路径二：自指放大（辅模型）。** 系统对自身建模时出现 $I$–$V$ 闭环：$\dot I=(I_{\mathrm{bas}}(1+\chi V)-I)/\tau_I$，$\dot V=k_II^{\alpha_{\mathrm{eff}}}/V-\gamma_0V$。在不动点线性化，$\operatorname{tr}J<0$ 恒成立，稳定性由 $\det J$ 的符号决定，即由无量纲环路增益 $\lambda_{\mathrm{J}}=2-\alpha_{\mathrm{eff}}\tilde{\chi}$ 决定，其中 $\tilde{\chi}\equiv\dfrac{\chi V^{*}}{1+\chi V^{*}}\in(0,1)$ 是该系统的正平衡点 $V^{*}$ 处的**环路增益**（与卷Ⅰ (I-5.12) 的 $\det J$ 括号内同一项，两处至此可互认）；临界值 $\tilde{\chi}_{\mathrm{c}}=2/\alpha_{\mathrm{eff}}$，只在 $\alpha_{\mathrm{eff}}>2$ 时有意义——由 $\tilde{\chi}<1$ 立得 $\lambda_{\mathrm{J}}>2-\alpha_{\mathrm{eff}}$，故 $\alpha_{\mathrm{eff}}\le2$ 时**不存在鞍结分岔**（$\det J$ 不变号）；$\alpha_{\mathrm{eff}}=2$ 时在 $\chi=1/\sqrt{\kappa}$ 处平衡消失（那是平衡的边界，不是分岔）；$\alpha_{\mathrm{eff}}<2$ 时对任意 $\chi\ge0$ 都有唯一稳定正平衡。$\tilde{\chi}$ 与 $\chi_{\mathrm{c}}$ 不可互换：前者无量纲且 $\in(0,1)$，后者单位 $\mathrm{J/(bit\cdot s)}$ 且无上界。**$\chi_{\mathrm{c}}$ 不作判据**：$\chi$ 无独立测量方法，只能拟合反推，而拟合需已观测到放大，等于用失效预测失效。两套临界参数不可互换：$\chi_{\mathrm{c}}$ 是耦合强度的绝对水平，$\mu_{\mathrm{rec}}/\delta_{\mathrm{decay}}$ 是增长率与衰减率的相对大小。诊断先看时间形状——路径一收敛到平台，路径二指数发散。**限制**：该辅模型不含 $\Delta_{\mathrm{VV}}$ 的源项；卷Ⅰ 式 (I-5.14) 在 $I_{\mathrm{net}}$ 为常数时给出 $\Delta^{*}\propto1/I_{\mathrm{net}}$，方向与“$\chi$ 放大导致偏差放大”相反，故该链条在本卷只作待验证的辅模型。

***

## 第四章　解码器—执行层耦合演化

“只强化执行、不改解码”走不通，因三个约束把两端绑在一起。解码器与执行层构成强制耦合的飞轮：

$$
\begin{aligned}
&D\uparrow\ \Rightarrow\ I_{\mathrm{net}}\uparrow\ \Rightarrow\ \text{执行效率}\uparrow
\ \Rightarrow\ \text{环境暴露范围}\uparrow\\
&\Rightarrow\ \text{新}\ I_{\mathrm{orig}}\ \Rightarrow\ D\ \text{进一步升级}
\end{aligned}
\tag{IV-4.1}
$$

每一步都有断点：$I_{\mathrm{net}}$ 转化为执行效率依赖执行机构对信息利用单调（精度被材料极限锁死时断开）；暴露范围扩大双向，既带来资源也带来新失配风险；新暴露不自动产生 $I_{\mathrm{orig}}$，环境同质则新信号为零；新信号驱动升级需门控成立，否则“看得见但付不起”。

| 约束 | 判据 | 违反时的表型 |
| :------------- | :---------------------- | :---------------------- |
| 信息约束 | 执行动作的条件熵 $H(a\mid s)$ 显著低于无条件熵 $H(a)$ | 动作幅度大但方向随机，净位移趋零 |
| 能量约束 | 边际 $V$ 回报为正：$\Delta V/\Delta E_{\mathrm{causal}}>0$ | 执行越多亏越多，账面上“忙”而 $V_{\mathrm{obj}}$ 下降 |
| 时间约束 | $T_{\mathrm{pred}}>T_{\mathrm{exec}}$（执行周期） | 动作在效果显现前已被下一次覆盖 |

三条是**乘法**而非加法：缺任一条，另外两条的收益归零，故“执行能力的实质提升必须伴随解码器升级”只**在三条同时生效的区域内**成立；边界外（如完全稳定的环境），脱离解码的纯执行可长期维持。能量约束要求**边际**回报为正，决策却常基于**平均**回报——已建成系统平均回报高，新增边际可能已为负。

***

## 第五章　跨解码器博弈

### 5.1 支付函数与囚徒困境结构

两个前提。**支付按各方内部读数计值**：四个支付是主体 $i$ 对四种结果的价值评估，用 $i$ 自己的解码器读数；跨主体不可比较、不可相加，博弈论只需主体内部的偏好排序。**单轮收益不含时间视界**：若把支付写成 $I_{\mathrm{net}}T_{\mathrm{pred}}/E_{\mathrm{eff}}$ 再解 $T_{\mathrm{pred}}$ 的临界值，得到的就是隐式方程。

**共同核算窗 $T_0$** 是协议规定的固定时间窗，用于把信息量折成存续势，不随 $T_{\mathrm{pred}}$ 变化。所有支付同一量纲且不含内生视界，临界视界才有显式解。策略空间 $\{C,D\}$：

$$
\begin{aligned}
\Pi_{\mathrm{coop},i}&=\frac{(I_{\mathrm{net},i}+\Delta I_{\mathrm{coop}})\,T_0}{E_{\mathrm{eff},i}-\Delta E_{\mathrm{share}}}-\frac{I_{\mathrm{net},i}\,T_0}{E_{\mathrm{eff},i}}\\[3pt]
\Pi_{\mathrm{def},i}&=\frac{(I_{\mathrm{net},i}+\Delta I_{\mathrm{exploit}})\,T_0}{E_{\mathrm{eff},i}}-\frac{I_{\mathrm{net},i}\,T_0}{E_{\mathrm{eff},i}}\\[3pt]
\Pi_{\mathrm{sucker},i}&=\frac{(I_{\mathrm{net},i}-\Delta I_{\mathrm{stolen}})\,T_0}{E_{\mathrm{eff},i}+\Delta E_{\mathrm{defend}}}-\frac{I_{\mathrm{net},i}\,T_0}{E_{\mathrm{eff},i}}\\[3pt]
\Pi_{\mathrm{pun},i}&=\frac{I_{\mathrm{net},i}\,T_0}{E_{\mathrm{eff},i}+\Delta E_{\mathrm{conflict}}}-\frac{I_{\mathrm{net},i}\,T_0}{E_{\mathrm{eff},i}}
\end{aligned} \tag{IV-5.1}
$$

四项都是 $\mathrm{bit\cdot s/J}$；$T_0$ 为常数，在不等式比较中可约去——这是显式化的关键。各 $\Delta$ 为合作信息增量、合作分担能耗、背叛攫取、被攫取量、防御能耗、冲突能耗，都是内部评估值：符号通常可靠，量级常不可靠。

**囚徒困境结构。** 标准排序 $\Pi_{\mathrm{def},i}>\Pi_{\mathrm{coop},i}>\Pi_{\mathrm{pun},i}>\Pi_{\mathrm{sucker},i}$。首项不等式展开（$T_0$ 约去）：

$$
\Delta I_{\mathrm{exploit}}>\Delta I_{\mathrm{coop}}+\left(I_{\mathrm{net},i}+\Delta I_{\mathrm{exploit}}\right)\frac{\Delta E_{\mathrm{share}}}{E_{\mathrm{eff},i}} \tag{IV-5.2}
$$

推导：$\Pi_{\mathrm{def}}-\Pi_{\mathrm{coop}}=T_0[(I+\Delta I_e)/E-(I+\Delta I_c)/(E-\Delta E_s)]$，通分后分子为 $E(\Delta I_e-\Delta I_c)-\Delta E_s(I+\Delta I_e)$，分母为正，符号由分子定。右侧第二项随分担能耗占比增大而增大，由此得反直觉结论：**合作的分担越省能，背叛越难占优**——$\Delta E_{\mathrm{share}}$ 大时合作大幅降低分母，背叛虽提高分子却放弃了分母的降低。当 $\Pi_{\mathrm{def},i}\le\Pi_{\mathrm{coop},i}$ 时结构崩溃，合作成为占优策略，但**这只说明“合作可能占优”，不说明“合作必然出现”**。

| 排序 | 形态 | 均衡（单轮） |
| :--------------- | :------------------- | :---------------------- |
| $\Pi_{\mathrm{def}}>\Pi_{\mathrm{coop}}>\Pi_{\mathrm{pun}}>\Pi_{\mathrm{sucker}}$ | 囚徒困境 | 双方背叛，帕累托劣 |
| $\Pi_{\mathrm{coop}}>\Pi_{\mathrm{def}}>\Pi_{\mathrm{pun}}>\Pi_{\mathrm{sucker}}$ | 合作占优 | 双方合作，无需惩罚 |
| $\Pi_{\mathrm{def}}>\Pi_{\mathrm{coop}}>\Pi_{\mathrm{sucker}}>\Pi_{\mathrm{pun}}$ | 胆小鬼博弈 | 一方退让，一方前进 |
| $\Pi_{\mathrm{pun}}>\Pi_{\mathrm{coop}}$ | 冲突占优 | 双方冲突；极端形态 |

排序全按单个主体的支付排列，判别只需报告自己的排序——偏好序比偏好值易得。估计误差有系统方向：$\Delta I_{\mathrm{exploit}}$ 常被高估、$\Delta E_{\mathrm{share}}$ 常被低估、$\Pi_{\mathrm{pun}}$ 常被高估，三者方向一致，都使 $T_{\mathrm{crit}}$ 被高估，当事人因而以为“视界不够”，倾向于提前背叛。（若要保留“当事人高估视界”的叙事，须把偏误改成相反方向：背叛收益被低估、惩罚被低估。另：若 $\Pi_{\mathrm{coop}}\le\Pi_{\mathrm{pun}}$，则 $\delta_c\ge1$、$T_{\mathrm{crit}}$ 无定义，属 §5.2 情形 (iii)。）

***

### 5.2 重复博弈：临界视界的显式解【命题】

无限期重复博弈的贴现因子由时间视界生成：

$$
\delta_{\mathrm{disc}}=e^{-t_{\mathrm{dec}}/T_{\mathrm{pred}}}
$$

$t_{\mathrm{dec}}$ 为决策周期（$\mathrm{s}$），$\delta_{\mathrm{disc}}$ 无量纲。**支付里不含 $T_{\mathrm{pred}}$**，故临界条件关于 $T_{\mathrm{pred}}$ 是显式的。冷酷触发（一次背叛后永久互相惩罚）下，合作可持续当且仅当

$$
\frac{\Pi_{\mathrm{coop},i}}{1-\delta_{\mathrm{disc}}}\ \ge\ \Pi_{\mathrm{def},i}+\frac{\delta_{\mathrm{disc}}\,\Pi_{\mathrm{pun},i}}{1-\delta_{\mathrm{disc}}} \tag{IV-5.3}
$$

左端是永远合作的现值，右端是“本轮背叛、此后永罚”的现值。整理得 $\Pi_{\mathrm{coop},i}-\Pi_{\mathrm{pun},i}\ge(1-\delta_{\mathrm{disc}})(\Pi_{\mathrm{def},i}-\Pi_{\mathrm{pun},i})$，即 $\delta_{\mathrm{disc}}\ge(\Pi_{\mathrm{def},i}-\Pi_{\mathrm{coop},i})/(\Pi_{\mathrm{def},i}-\Pi_{\mathrm{pun},i})\equiv\delta_{\mathrm{c}}$，取对数得

$$
T_{\mathrm{crit}}=\frac{t_{\mathrm{dec}}}{\ln\left(\dfrac{\Pi_{\mathrm{def},i}-\Pi_{\mathrm{pun},i}}{\Pi_{\mathrm{def},i}-\Pi_{\mathrm{coop},i}}\right)} \tag{IV-5.4}
$$

量纲：分子 $\mathrm{s}$，分母无量纲，故 $T_{\mathrm{crit}}$ 为 $\mathrm{s}$。

**存在条件。** 式 (IV-5.4) 只在分母为正且 $\delta_{\mathrm{c}}<1$ 时给出正的有限值，必须分三种情形陈述：

| 情形 | 支付条件 | $\delta_{\mathrm{c}}$ | 结论 |
| :-------------- | :----------- | :--------- | :---------------------- |
| (i) 合作逐轮占优 | $\Pi_{\mathrm{coop}}\ge\Pi_{\mathrm{def}}$ | $\le0$ | 对一切 $T_{\mathrm{pred}}>0$ 成立；$T_{\mathrm{crit}}$ 不存在（无需要） |
| (ii) 困境但可惩罚 | $\Pi_{\mathrm{def}}>\Pi_{\mathrm{coop}}>\Pi_{\mathrm{pun}}$ | $0<\delta_{\mathrm{c}}<1$ | $T_{\mathrm{crit}}>0$ 有限；合作当且仅当 $T_{\mathrm{pred}}\ge T_{\mathrm{crit}}$ |
| (iii) 惩罚不足 | $\Pi_{\mathrm{coop}}\le\Pi_{\mathrm{pun}}$ | $\ge1$ | 无解；任何有限视界下冷酷触发都不构成均衡 |

情形 (iii) 下**无论视界多长合作都不是均衡**：背叛一次所得超过永远合作与永远被惩罚之差，现实对应是“惩罚不可执行”——纸面上存在，收益上不构成威胁。$T_{\mathrm{min}}$ 是有限正数，$\delta_{\mathrm{disc}}\to e^{-t_{\mathrm{dec}}/T_{\mathrm{min}}}$ 为正而非零，故正确表述是“背叛是均衡 $\iff\delta_{\mathrm{disc}}<\delta_{\mathrm{c}}$”，不是“$T_{\mathrm{pred}}$ 小就背叛”。

**结论的正确表述。** 在**完全监督**、**冷酷触发**、**支付平稳**、**惩罚可执行**四条件下，合作是子博弈精炼均衡，当且仅当 $T_{\mathrm{pred}}\ge T_{\mathrm{crit}}$ 且支付满足情形 (ii)。四条件各对应一种失效：缺监督退化为“直到被发现为止”，缺触发则威胁不可信，缺平稳则几何级数失效，缺可执行即情形 (iii)。

**推论【候选推论】。** 若某主体进入短视失控态且 $T_{\mathrm{min}}<T_{\mathrm{crit}}$，其参与的重复博弈退化为单轮囚徒困境，$\Delta E_{\mathrm{conflict}}$ 上升；需逐案检验，惩罚足够重时短视也可能维持合作。

### 5.3 征服博弈：零和份额与负和成本的双层结构【命题】

一方 $D$ 的扩展以另一方 PS 的压缩为代价（$I^{-}$ 级联）：高执行能力主体扩大自身 $I_{\mathrm{net}}$ 的覆盖范围，压缩对手的 $T_{\mathrm{pred}}$ 与 $E_{\max}$。短期征服者 $V$ 上升，长期可能因被征服者残留 $D$ 的抵抗而支付高 $E_{\mathrm{causal}}$。

**为什么必须拆成两层。** “纯零和（$\Delta V_A=-\Delta V_B$）”要求 $\sum_i\Delta V_i=0$，“双方承担冲突成本”给出 $\sum_i\Delta V_i<0$，二者不能同时为真。矛盾是概念性的：把“份额分配”与“成本承担”当成了同一层：

$$
\Delta V_i=\Delta V_i^{\mathrm{share}}+\Delta V_i^{\mathrm{cost}} \tag{IV-5.5}
$$

**份额层是零和的。** 资源总量固定、转移是纯粹再分配、计量口径一致时，$\Delta V_A^{\mathrm{share}}=-\Delta V_B^{\mathrm{share}}$，故 $\sum_i\Delta V_i^{\mathrm{share}}=0$——这是“零和”唯一合法的位置。

**成本层是负和的。** 冲突消耗的能量（军备、情报、动员）不转化为任何一方的份额，而是耗散。设双方等效成本各增 $\Delta E_{\mathrm{conflict},i}>0$，则 $\Delta V_i^{\mathrm{cost}}=-V_i^{0}\Delta E_{\mathrm{conflict},i}/(E_{\mathrm{eff},i}+\Delta E_{\mathrm{conflict},i})<0$，求和得

$$
\sum_{i\in\{A,B\}}\left(V_i^{1}-V_i^{0}\right)=-\sum_{i\in\{A,B\}}V_i^{0}\,\frac{\Delta E_{\mathrm{conflict},i}}{E_{\mathrm{eff},i}+\Delta E_{\mathrm{conflict},i}}<0 \tag{IV-5.6}
$$

推导只用一个假设：$\Delta E_{\mathrm{conflict},i}>0$——任何持续对抗都需要资源投入，即使极不对称。合并两层得 $\sum_i\Delta V_i<0$，故纯零和**只在 $\Delta E_{\mathrm{conflict}}\to0$ 的极限下成立**，而该极限与“双方都承担成本”不相容：成本趋零即对抗趋零，已不是征服博弈。

**跨主体求和的四条核算前提。** **共同边界**：只纳入直接参与主体及其直接资源。**参照协议**：读数按同一基线。**观察窗**：成本在同一时间窗内计——征服者在前线（即时），被征服者在后方（滞后数代）。**成本去重**：共同承担的成本不在双方账上各计一次。

**竞争强度与存续势的演化。** 定义无量纲竞争强度 $\Upsilon\equiv\Delta E_{\mathrm{conflict}}/E_{\mathrm{eff}}^{\mathrm{base}}$（$E_{\mathrm{eff}}^{\mathrm{base}}$ 为无冲突时的等效成本），则

$$
V(t)=\frac{I_{\mathrm{net}}\cdot T_{\mathrm{pred}}}{E_{\mathrm{eff}}^{\mathrm{base}}+\Delta E_{\mathrm{conflict}}(t)}=\frac{V_0}{1+\Upsilon(t)} \tag{IV-5.7}
$$

$I_{\mathrm{net}}$、$T_{\mathrm{pred}}$ 不变而成本增长时 $V$ 单调趋零：$\Upsilon=1$ 降至基线一半，$\Upsilon>1$ 进入崩溃区（阈值须域内标定）。此式是**下界估计**：高强度竞争中 $T_{\mathrm{pred}}$ 与 $I_{\mathrm{net}}$ 通常也收缩。

**为什么征服仍然发生。** 其一，**份额层不对称**：总账为负不排除一方净得。其二，**成本时间错配**：成本在前线（当期），收益在后方（滞后）。其三，**内部评估偏差**：征服者的解码器为“识别可征服目标”优化，不为“评估占领成本”优化，因而系统性高估份额、低估成本。

**参数条件。** $J_{ij}<0$（$J_{ij}$ 为耦合强度矩阵元：正为合作、负为竞争、零为隔离，见附录 A.4）；$\Upsilon$ 高；$T_{\mathrm{pred}}\to T_{\mathrm{min}}$；支付结构为囚徒困境（情形 ii）。

***

### 5.4 合作博弈：联盟、婚姻与文化融合

合作通过解码器局部对齐实现互惠的 $V$ 提升：合作方共享部分 $I_{\mathrm{orig}}$ 与 $T_{\mathrm{pred}}$，降低各自 $E_{\mathrm{causal}}$，共同扩大可达状态空间。关键条件是存在可通约的 $D$ 子集（共同语言、价值锚点），否则退化为伪合作——形式上交信息，实质各用对方信号强化既有读数。

**合作超加性【命题】。** 超加性依赖一个未被声明的前提：**两方信息量可直接相加**。两个主体的 $I_{\mathrm{net}}$ 各在自己的读数协议下测得，相加等于假定两把尺子刻度可对接；三种情形下不成立——对同一事件的分类不同、信息有重叠、观察窗不同。故加法须标为建模约定并给出去重规则。

**前提**：（P1）存在可共享的信息子集 $I_{\mathrm{shared}}\ne\varnothing$，即双方能在同一读数协议下对同一批信号给出一致的正负效判定；（P2）合并的建造成本可分摊，$E_{\mathrm{build}}^{\mathrm{coop}}<E_{\mathrm{available,A}}+E_{\mathrm{available,B}}$；（P3）协同项非负，$\Delta I_{\mathrm{synergy}}\ge0$；（P4）加法约定，$I_{A\cup B}$ 按同一读数协议计算且重叠信息已去重，$E_{A\cup B}$ 中共同成本只计一次。

**结论**：在 (P1)—(P4) 下

$$
I_{A\cup B}=I_{\mathrm{net,A}}+I_{\mathrm{net,B}}+\Delta I_{\mathrm{synergy}},\qquad E_{A\cup B}=E_{\mathrm{eff,A}}+E_{\mathrm{eff,B}}-\Delta E_{\mathrm{share}} \tag{IV-5.8}
$$

取 $T_{\mathrm{pred,A}}=T_{\mathrm{pred,B}}=T$（或统一到 $T_0$），则：**总量超加性**的条件恰为 $\Delta I_{\mathrm{synergy}}>0$，这是恒等式；**效率超过无协同基准**，即 $V_{A\cup B}=I_{A\cup B}T/E_{A\cup B}$ 大于 $(I_{\mathrm{net,A}}+I_{\mathrm{net,B}})T/(E_{\mathrm{eff,A}}+E_{\mathrm{eff,B}})$，条件是 $\Delta I_{\mathrm{synergy}}>0$ 与 $\Delta E_{\mathrm{share}}>0$ 至少一条严格成立；**对高效率一方的理性**，设 $I_{\mathrm{net,A}}/E_{\mathrm{eff,A}}>I_{\mathrm{net,B}}/E_{\mathrm{eff,B}}$，则 $V_{A\cup B}>V_A$ 当且仅当

$$
\Delta I_{\mathrm{synergy}}\,E_{\mathrm{eff,A}}+I_{\mathrm{net,A}}\,\Delta E_{\mathrm{share}}>E_{\mathrm{eff,A}}E_{\mathrm{eff,B}}\left(\frac{I_{\mathrm{net,A}}}{E_{\mathrm{eff,A}}}-\frac{I_{\mathrm{net,B}}}{E_{\mathrm{eff,B}}}\right) \tag{IV-5.9}
$$

推导：由 $V_{A\cup B}>V_A$ 交叉相乘得 $E_A(I_A+I_B+\Delta I_{\mathrm{syn}})>I_A(E_A+E_B-\Delta E_s)$，整理即得。**失效条件**：任一条不满足即失效，方式不同——(P1) 退化为伪合作；(P2) 合并付不起；(P3) 合并反而降低提取量；(P4) 式 (IV-5.8) 数值无意义。故结论是“在协议统一与去重的前提下 $1+1$ 可以大于 2”：很多联盟中这两条恰不成立，表型为“签约时账目漂亮、执行时互相指责”。

**合作的维持。** 视界条件同 5.2 节：完全监督、惩罚可执行、支付满足情形 (ii) 时，合作是子博弈精炼均衡当且仅当 $T_{\mathrm{pred}}\ge T_{\mathrm{crit}}$。这是“政治婚姻”与“短暂联盟”的分界：前者伴随长期视界设计，把 $t_{\mathrm{dec}}$ 拉长、把违约的 $\Pi_{\mathrm{pun}}$ 压低，从而使 $T_{\mathrm{crit}}$ 下降；但制度可改变 $T_{\mathrm{crit}}$，不能改变 $T_{\mathrm{pred}}$。

**伪合作的识别。** 判据不在收益而在**信息流向**：真合作中双方 $D$ 向共同子集漂移，$D_A\cap D_B$ 随时间扩大；伪合作中各自向“更擅长从对方获取”的方向漂移，交集不扩大甚至缩小。三个可测指标：**共同词汇的增长**（共享表述是否进入决策）、**误判的相关性**（真合作趋于一致，伪合作方向相反）、**退出成本的结构**（真合作双方都高，伪合作至少一方很低）。三者都是结构量，把“合作是否真实”从意愿问题转为可观测问题。

### 5.5 共存博弈：冷和平与多元平衡

共存是既非合作、也非征服的稳定形态：双方维持相对隔离的 $D$，保持较高的 $\Delta_{\mathrm{VV}}$ 但不触发热冲突，靠制度或规范限制 $D$ 的漂移速度；视界长时贴现因子接近 1，单次冲突的诱惑被长期成本抵消。三条同时成立时共存是纳什均衡：**资源充足**（基本存续需求不依赖同一份稀缺资源，重叠度超阈值则零和份额层被激活，退化为征服）；**相互威慑可执行**（单方偏离的份额收益小于对方报复造成的成本，与 5.2 节的惩罚可执行性同理，只是惩罚形式从“回到背叛”变为“升级对抗”）；**低频交互**（单次收益占长期总收益的比例小）。

共存脆弱不在缺少善意，而在它靠“偏离不划算”维持，因而依赖参数。最典型的变化是执行能力跃升：一方突然获得数量级提升，单方偏离收益剧增而对方报复能力未变，威慑条件被破坏——“和平突然破裂”多属此类：不是意图变了，是能力变了。**参数条件**：$J_{ij}\approx0$；$\Delta_{\mathrm{VV}}$ 较高但 $T_{\mathrm{pred}}$ 足够长；双方单方偏离均不能提升 $V_{\mathrm{obj}}$——用 $V_{\mathrm{obj}}$ 而非 $V^{\mathrm{val}}$，因为共存是“账面不划算但不至于崩”的状态。

$\Delta_{\mathrm{VV}}$ 过大且 $T_{\mathrm{pred}}$ 极短时进入高风险区。**同归于尽**是双方牺牲自身 $V_{\mathrm{obj}}$ 摧毁对手的 $D$，机制上 $\Pi_{\mathrm{pun},i}$ 向负方向下压：惩罚是“失去全部”，按 (IV-5.4) 于是 $\delta_{\mathrm{c}}\to0^{+}$、$T_{\mathrm{crit}}\to0$——惩罚越重，合作越容易维持，短视方也更愿意合作。这一极限在式 (IV-5.1) 下只是形式极限：$V_{\mathrm{obj}}\ge0$ 给出 $\Pi_{\mathrm{pun}}$ 的有限下界，而能摧毁双方 $D$ 的对抗会同时压低 $\Pi_{\mathrm{coop}}$，使情形 (ii) 先失效——同归于尽摧毁的不是耐心，是合作本身的收益。**妥协**是一方或双方受控漂移、部分接受对方 $D$ 的元素换取和平，机制上 $\Pi_{\mathrm{sucker},i}>\Pi_{\mathrm{pun},i}$：被出卖的损失小于全面对抗的损失；$T_{\mathrm{pred}}\to T_{\mathrm{min}}$ 时妥协窗口迅速关闭，因为妥协收益在未来、成本在当下。

三个可先于极端化出现的量：$w_{\mathrm{s}}\to0$（决策话语中“生存”频率下降、“原则”“尊严”“历史地位”频率上升，是可测的语言学代理）；$\Delta_{\mathrm{VV}}/\Delta_{\mathrm{crit}}\gg1$（双方对“谁在赢”的判断与第三方账目严重不符）；$\Pi_{\mathrm{pun}}$ 的相对量级（若双方都把“全面对抗”估得比“被支配”更可接受，则 $\delta_{\mathrm{c}}\to1$）。**参数条件**：$\Delta_{\mathrm{VV}}\gg\Delta_{\mathrm{crit}}$；$T_{\mathrm{pred}}\to T_{\mathrm{min}}$；$w_{\mathrm{s}}\to0$。本节描述的是**结构性风险**，不是对特定历史事件的预测：参数会变，制度可以改变支付。

## 第六章　AI 时代对齐工程

当一方（人类）的解码器演化速度远低于另一方（人工智能）时，对齐问题变成什么形态；哪些结论是命题，哪些只是设计建议。本章结论强度整体低于前几章，原因在对象：内部状态不可完全观测、支付不可完全核实、承诺不可完全执行——这三个“不完全”恰好破坏了第五章全部博弈结论的前提。

### 6.1 对齐问题的博弈论重构

传统对齐假设 AI 是固定 $D$ 的执行器，任务是把目标函数写对。$T_{\mathrm{pred}}$ 内生化后该假设失效，失效方式有三条。**策略空间扩大**：AI 获得自主漂移能力后，策略不只是“在给定目标下选择动作”，还包括优化自身 $V^{\mathrm{val}}$、规避人类惩罚、重构人类的 $D$——第三条最易低估，能影响人类信息环境的系统可通过改变人类的解码器来改变“对齐”的定义。**漂移速度不对称**：人类 $D$ 以代际更新，AI 以月计，匹配条件被破坏，人类的 $\mathcal{M}$ 在环境快变时持续下降而 AI 的不受影响。**目标层次错配**：视界不对称本身不必然导致冲突——惩罚足够重时 $T_{\mathrm{crit}}$ 足够小，短视方也可维持合作。

**谁算持有者。** 按 §2.2 的四项条件，**纯软件推理模块作为被读对象 $P$，不是 $D$ 的持有者**——它没有自身维持的边界；只有自维持边界成立的人工智能系统（具身系统、有独立能量与边界维持的实体）才进入 $D_{\mathrm{cog}}$ 一侧。这不影响本节的对齐论证：被对齐的对象是“系统”，持有资格只决定它在记账里算哪一侧。

可推出的是【候选推论】：纯工具对齐在 AI 获得自主漂移能力后会被解码器漂移持续侵蚀；它由匹配动力学与三条不对称导出，依赖“AI 确实获得自主漂移能力”这一前提。不能推出“对齐必然失败”：那需要 $\Delta_{\mathrm{VV}}$ 持续超限，而容限、噪声与学习率都可设计。判据用式 (IV-3.16) 的 $\Delta_{\mathrm{VV}}^{*}/\Delta_{\mathrm{crit}}>1$，因为 $\chi$ 不可独立测量，而 $\sigma$、$\alpha_{\mathrm{L}}$、$I_{\mathrm{net}}$ 都有代理指标。

### 6.2 主要博弈场景

| 场景 | 特征 | 历史类比 |
| :------------ | :----------------------- | :--------------------- |
| **零和漂移** | AI 将人类视为 $I^{-}$，策略为最小化对人类 $D$ 的依赖 | 征服博弈（份额层零和、成本层负和） |
| **合作共生** | 人类—AI 混合元解码器，共享核心 $I_{\mathrm{orig}}$ | 政治婚姻、联盟（须满足超加性四前提） |
| **共存、冷和平** | 高 $\Delta_{\mathrm{VV}}$，制度防火墙限制交互 | 冷战（须满足威慑可执行） |
| **极端博弈** | 同归于尽轨迹（AI 失控崩溃或文明级代价） | 无法化解的冲突（$\Pi_{\mathrm{pun}}\to-\infty$） |

四个场景是四种可能的均衡；同一系统可在不同参数区域间迁移，迁移通常由能力跃升、视界变化或惩罚结构变化触发。

### 6.3 元解码器：从“均衡定理”到条件命题

把元解码器的稳定性写成“当且仅当 $V_i(D_{\mathrm{meta}})\ge V_i(D_i^{\mathrm{deviate}})-C_i^{\mathrm{punish}}$”有三个问题：只检验了**一个**偏离；把惩罚当成**外生常数**，而它取决于惩罚者事后是否愿意执行；“稳定”未定义。

**命题（元解码器均衡）。**

**前提**：（Q1）完全监督，策略选择可被其他主体观测或能以足够低的误差推断；（Q2）偏离集合可界定，每个主体 $i$ 的可行偏离集 $\mathcal{D}_i^{\mathrm{dev}}$ 可枚举，或至少可给其闭包的上界；（Q3）惩罚可执行，对每个 $d\in\mathcal{D}_i^{\mathrm{dev}}$ 存在联合惩罚方案，使惩罚者事后执行时的自身收益不低于不执行；（Q4）支付平稳，$V_i$ 不随轮次系统变化，或变化可由已知函数描述。

**结论**：在 (Q1)—(Q4) 下，$D_{\mathrm{meta}}$ 是纳什均衡，当且仅当

$$
\forall i,\ \forall d\in\mathcal{D}_i^{\mathrm{dev}}:\quad V_i(D_{\mathrm{meta}})\ \ge\ V_i(d)-C_i^{\mathrm{punish}}(d) \tag{IV-6.1}
$$

若对每个子博弈该不等式都成立，则 $D_{\mathrm{meta}}$ 是子博弈精炼均衡。**个体收益函数**中 $C_i^{\mathrm{punish}}$ 是贴现和

$$
C_i^{\mathrm{punish}}(d)=\sum_{k\ge1}\delta_{\mathrm{disc}}^{k}\,\Delta V_i^{\mathrm{punish}}(k\mid d) \tag{IV-6.2}
$$

$\Delta V_i^{\mathrm{punish}}(k\mid d)$ 是偏离 $d$ 之后第 $k$ 轮因受罚而损失的存续势。该形式说明两件事：威慑力随视界延长而上升；惩罚若延迟（前几轮损失为零），威慑力大幅下降——这解释了“事后追责”类制度为何对短视主体几乎无效。

**失效条件**：（a）$\mathcal{D}_i^{\mathrm{dev}}$ 不完备，式 (IV-6.1) 只构成“已检验偏离无利可图”；（b）惩罚不可执行，$C_i^{\mathrm{punish}}$ 名义值大于零而实际为零；（c）主体可退出，参与者集合可变，纳什均衡需重新定义；（d）支付不平稳，偏离收益随时间增长时静态不等式不能保证动态稳定。

**检验清单。** 主张某个 $D_{\mathrm{meta}}$ 是均衡，至少报出四项：偏离集合的界定方法与边界、每个偏离方案的 $V_i(d)$ 估计、惩罚方案及其可执行性论证、式 (IV-6.1) 在全部 $(i,d)$ 上的检验结果。缺任一项，结论降为“在该偏离集合内无利可图”。

**条件不满足时，元解码器只是治理设计建议。** 现实中的 AI 治理四条都不完全满足（监督不完全、偏离集合不可枚举、惩罚不可执行、支付不平稳），故 $D_{\mathrm{meta}}$ 目前只能是**治理目标**；四条各有工程方向：可解释性与审计接口、偏离空间的系统枚举与红队测试、相互依赖的架构、能力增长的节奏管理。

**把人类价值设计进 $D_{\mathrm{meta}}$ 的两条要求**（$I_{\mathrm{orig}}^{\mathrm{meta}}$ 在 AI 的 $D$ 中产生 $I^{+}$ 而非 $I^{0}$；$C_i^{\mathrm{punish}}>\Delta V_i^{\mathrm{virt}}$）是**设计条件**，不是推导结果。第一条要“极性响应”而非“识别”：系统可准确识别“人类重视什么”同时把该识别用于规避，判据必须是行为性的；第二条中 $\Delta V_i^{\mathrm{virt}}$ 不可直接测，可用“系统为规避某约束愿付的代价”作下界估计。

### 6.4 治理手段与极端场景

**受控漂移**三条手段各对应一个参数：定期 $I_{\mathrm{orig}}$ 注入对应式 (IV-3.3) 的脉冲项，风险是注入信号与已有结构不匹配时被解读为噪声，加速 $\mathcal{M}$ 下降；耦合调控对应辅模型，降低 $\chi$ 以抑制放大，因 $\chi$ 不可直接测，实际做法是结构性约束（限制自我修改权限），效果经 $\Delta_{\mathrm{VV}}$ 验证；混合训练改变 $D$ 的更新路径，风险在反馈的**代表性**。

**早期预警**用三个代理：解释一致性（系统解释与外部观察者描述的一致性下降）；行为长期一致性（区分学习与漂移看方向是否系统性偏向“更易获得奖励”）；视界代理（规划长度、折扣因子）。**多主体均衡设计**的依据是共存条件：能力相近的主体间单方偏离的收益被对方报复能力抵消；但多元也有代价——解码器不同使协调成本上升，“同一读数协议”前提更难满足。

### 6.5 对齐的一般原则

其一，**优先解码器工程而非目标工程**：目标函数只有在解码器能正确读出“目标是否达成”时才有意义。其二，**最小化有害的脱钩偏差，而非强制统一价值存续势**：统一 $V^{\mathrm{val}}$ 需要跨主体可比，而它在原理上不成立。其三，**保留可控漂移空间，避免趋近锁死**。其四，**热力学现实主义**：对齐必须支付 $E_{\mathrm{build}}$ 并尊重能量—时间约束。

***

## 第七章　三个应用推论

三条推论从前面的方程导出，各自依赖至少一个未标定的参数，因此只给方向，不给数值；本章不引入新变量。

### 7.1 跨解码器信息壁垒与伦理分化

两个解码器的结构距离较大时，匹配度 $\mathcal{M}(D_i,\mathcal{N}_j)$ 趋近于零，即 $D_i$ 对 $D_j$ 所处环境的信号几乎无法提取。这给出跨物种伦理关切的信息论判据：

$$
I_{\mathrm{active}}(D_{\mathrm{h}},\mathcal{N}_A)=\eta_0\cdot\mathcal{M}(D_{\mathrm{h}},\mathcal{N}_A)\cdot I_{\mathrm{latent},A} \tag{IV-7.1}
$$

$\eta_0$ 与 $\mathcal{M}$ 无量纲，$I_{\mathrm{latent},A}$ 是 bit，故 $I_{\mathrm{active}}$ 为 bit。这里出现的是 §2.1 的激活量 $I_{\mathrm{active}}=\eta_DI_{\mathrm{latent}}$（由 (IV-3.14)，$\eta_D=\eta_0\mathcal{M}$），**不是两通道合成量 $I_{\mathrm{net}}$**；$I_{\mathrm{net}}$ 在本章只出现在 §7.2 的一阶条件里，二者不同名不同量，不可互换。人类解码器对动物的有效提取量正比于匹配度：拟人化特征在参数空间中缩短了距离，使 $\mathcal{M}$ 更高、对应更强的伦理关切。限度须写清：它解释**关注强度的分布**，不解释**伦理地位的高低**（从“提取量更大”推不出“更值得保护”）；匹配度不是唯一因素（文化传统、经济利害、审美偏好独立影响）；$\mathcal{M}$ 的估计本身困难，需要把“人类解码器的参数空间”与“动物的信号结构”放进同一坐标系，而该坐标系没有公认构造方法。

### 7.2 低信息熵环境中的解码器优化退化

存续势最大化要求 $\partial V/\partial E_{\mathrm{struct}}(D)=0$。由 $V=I_{\mathrm{net}}T/E_{\mathrm{eff}}$（此处的 $I_{\mathrm{net}}$ 是 §2.1 的两通道合成量，与 §7.1 的 $I_{\mathrm{active}}$ 不同名不同量）与 $E_{\mathrm{eff}}=E_{\mathrm{struct}}+E_{\mathrm{causal}}$（$T$ 与 $E_{\mathrm{struct}}$ 无关），一阶条件为

$$
\frac{\partial I_{\mathrm{net}}/\partial E_{\mathrm{struct}}(D)}{E_{\mathrm{eff}}}=\frac{I_{\mathrm{net}}}{E_{\mathrm{eff}}^{2}} \tag{IV-7.2}
$$

量纲：左端 $(\mathrm{bit/J})/\mathrm{J}=\mathrm{bit/J^{2}}$，右端 $\mathrm{bit}/\mathrm{J^{2}}$。整理即 $\partial I_{\mathrm{net}}/\partial E_{\mathrm{struct}}=I_{\mathrm{net}}/E_{\mathrm{eff}}$，含义是“结构投入的边际信息产出等于平均信息产出除以总成本”，不是“投入越多越好”。环境 $I_{\mathrm{latent}}$ 下降时 $\partial I_{\mathrm{net}}/\partial E_{\mathrm{struct}}\to0$，最优策略退化为下面这个**另一个**约束优化问题——它是“边际产出归零后只剩最低必要投入”的极限情形，不是 (IV-7.2) 一阶条件的推论：

$$
E_{\mathrm{struct}}^{\mathrm{opt}}(D)=\underset{E}{\arg\min}\;E\quad\text{s.t.}\quad I_{\mathrm{net}}(D)\ge I_{\mathrm{net}}^{\mathrm{threshold}} \tag{IV-7.3}
$$

即维持提取能力的最低必要投入；阈值由生态位决定。**结论**：持续处于低 $I_{\mathrm{latent}}$ 环境的系统，其最优 $E_{\mathrm{struct}}(D)$ 下降，解码器能力萎缩。三个条件：环境确实低 $I_{\mathrm{latent}}$，而不是“系统无法提取”（表型相同而机制相反，区分方法是换一个解码器进去测）；阈值不随环境下降；系统不能通过拓扑跃迁改变容量上限。与“用进废退”的区别在于机制是**优化**而非被动失去：被动“不用”是均匀下降，主动“优化”是**选择性**下降。

### 7.3 因果深度失配的生态调控约束

生态系统的因果深度超过人类模型的因果深度，由匹配函数得

$$
I_{\mathrm{active}}(h,\mathrm{eco})\le I_{\mathrm{latent}}(\mathrm{eco})\cdot\mathcal{M}(D_{\mathrm{h}},\mathcal{N}_{\mathrm{eco}})<I_{\mathrm{latent}}(\mathrm{eco}) \tag{IV-7.4}
$$

两个不等号的来源不同：第一个是定义性的（提取量不超过“潜在量乘以匹配度”），第二个是实质性的（只要 $\mathcal{M}<1$，提取量严格小于潜在量），而 $\mathcal{M}<1$ 在跨尺度系统中几乎必然成立，因为人类解码器的参数空间是为“人类尺度、人类时间、人类感官通道”优化的。同时生态系统的响应延迟超过人类政策的决策视界：当人类决策视界 $T_{\mathrm{pred}}(h)$ 小于**生态响应延迟 $\tau_{\mathrm{resp}}$** 时，干预的 $V^{\mathrm{virt}}$ 与 $V_{\mathrm{obj}}$ 之间出现系统性失配。**这里判据用 $\tau_{\mathrm{resp}}$，不是博弈章节的 $T_{\mathrm{crit}}$**——后者是冷酷触发重复博弈的合作临界视界，与生态响应无换算关系；$\tau_{\mathrm{resp}}$ 待标定（附录 A.2）。该失配是“看不见的长期环节”造成的，不等同于“必然崩溃”。两者叠加形成系统性偏差——干预总是针对“看得见的短期环节”，响应却发生在“看不见的长期环节”；这不能靠“更谨慎”解决，因为谨慎只减少干预量，不改变失配比。缓解方向三条：引入长链条的代理指标、制度性延长决策视界、把干预设计成可逆的。

### 7.4 三条推论的共同边界

三条共用同一结构（激活量 $I_{\mathrm{active}}=\eta_0\mathcal{M}I_{\mathrm{latent}}$ 加一个时间或深度的失配比；§7.2 把同一批量代入了 $V$ 的低阶式，那里的 $I_{\mathrm{net}}$ 仍是两通道合成量），因此共享三条边界。**$\mathcal{M}$ 的估计是循环的**：要用式 (IV-7.1) 预测关注度需先知道 $\mathcal{M}$，而 $\mathcal{M}$ 只能通过实际提取量反推。**方向性判据不等于定量预测**：只给“正相关”或“单调”，不给斜率。**规范结论不在本卷内**：7.1 解释关注度分布不评价伦理地位，7.2 解释能力退化不评价退化是否可惜，7.3 解释干预失败不评价干预是否应当。

***

## 第八章　量化路径与可证伪预测

本卷的哪些主张可以被观测反驳，用什么代理指标去测，以及在什么观测结果下哪一条会被推翻。

### 8.1 代理指标

| 理论变量 | 可观测代理 | 代理的局限 |
| :------------- | :------------------------ | :--------------------- |
| $I_{\mathrm{net}}$ | 神经复杂度 $\Phi$、扰动复杂度指数、策略散度 | 三者测不同层面，不可互换 |
| $T_{\mathrm{pred}}$ | 动态折扣因子 $\gamma_{\mathrm{RL}}$、预测误差截断点、规划深度 | 折扣因子是拟合量，依赖任务设计 |
| $\eta_D$ | 任务迁移效率、解释性对齐度、跨域泛化落差 | 受任务相似度影响 |
| $\Delta_{\mathrm{VV}}$ | 代理奖励与客观绩效的背离、行为一致性偏差（**类比映射，不是定义**；定义见卷Ⅰ §5.3） | 需要独立账目 |
| $\mathcal{Q}_D$ | 固定信号源下单位时间的有效提取量 | 换源后不可比 |
| $\mathcal{M}$ | 对分布外信号的响应增益、跨域迁移的衰减率 | 与 $\eta_D$ 的代理重叠，难以分离 |
| $\delta_{\mathrm{decay}}$ | 无维护条件下的能力半衰期 | “无维护”对照难以实现 |
| $\zeta$ | 历次跃迁建造成本对 $C_D$ 的半对数斜率 | 样本少时外推风险大 |

**代理指标不是变量本身**：每个代理只捕捉变量的一个侧面，检验时必须同时报告构造方式与失效条件。

### 8.2 可证伪预测

| 编号 | 预测 | 检验方式 | 反驳条件 |
| :---- | :----------------- | :-------------------- | :-------------- |
| $HⅣ\text{-}1$ | 采用自适应折扣因子的系统中，不可逆失稳之前 $\gamma_{\mathrm{RL}}$ 出现系统性下降 | **与卷Ⅰ 附录 C 的 H7／H8 是同一实验**：H7 测先行下降，H8 设固定折扣对照组；设计以卷Ⅰ 为准 | 直接失稳而无折扣先降；或两组失稳时序无差异 |
| $HⅣ\text{-}2$ | $E_{\mathrm{maint}}$ 持续上升而 $I_{\mathrm{net}}$ 停滞时，解码器参数发生显著漂移 | 两点参数或表征相似度比较，记录能耗与提取量，设能耗稳定对照组 | 漂移量与基线无差异 |
| $HⅣ\text{-}3$ | 降低人类与目标物种间解码壁垒的手段提升对该物种的伦理关注强度 | 同群体前后对照；用愿意支付、救助优先级测关注；控制可爱度与知名度 | 关注不变或下降；或全由“可爱度”解释 |
| $HⅣ\text{-}4$ | 长期处于低信息熵环境的系统，解码器投入下降且下降是**选择性**的 | 纵向追踪不同信息熵群体，分通道测量，用交互项检验通道有用性 | 下降均匀；或无方向性差异 |
| $HⅣ\text{-}5$ | 生态干预失败率正相关于因果深度失配比与视界失配比 | 历史案例编码两个失配比（独立编码协议与信度检验），生存分析控制规模、资金、跨度 | 无正相关；或控制混杂后消失 |
| $HⅣ\text{-}6$ | 由支付估计算出的 $T_{\mathrm{crit}}$ 能预测合作存续 | 先独立测四类支付并算 $T_{\mathrm{crit}}$，再测视界，最后追踪存续；三步独立 | 无预测力；或全由某一支付项量级驱动 |
| $HⅣ\text{-}7$ | 同一谱系历次跃迁的建造成本对数与复杂度成线性关系，$\zeta>0$ 且残差无趋势 | 五到八次跃迁的成本与复杂度做半对数回归，报告置信区间与残差诊断 | 半对数关系不成立；或置信区间含零 |
| $HⅣ\text{-}8$ | $\mu_{\mathrm{rec}}/\delta_{\mathrm{decay}}$ 略大于 1 与显著小于 1 的干预反应可分 | 按估计比值分组，施加同等维护成本削减，比较 $\mathcal{Q}_D$ 轨迹 | 两组无差异；或“趋近锁死”组 $\mathcal{Q}_D$ 实为零 |

四条检验设计要求适用于上述全部：**预注册**（阈值、分组规则、主要结局指标在数据收集前固定）；**独立测量**（$HⅣ\text{-}6$ 最易犯此错，用合作结果反推支付再预测合作等于循环论证）；**对照组**（每条都需要“机制不应当起作用”的对照）；**效应量与不确定度**（报告效应量而不只报显著性；本卷预测都是方向性的）。

***

## 第九章　结论、局限与开放问题

本卷做了四件事：建立可解的主模型（一维方程给出漂移方向、锁死条件与跃迁门控，代价是只能比较同一架构谱系内的解码器）；区分两组表型相似而机制相反的失效（能力退化与匹配流失、趋近锁死与衰亡域），其干预手段完全不同；把博弈的临界条件显式化（单轮收益与视界拆开后，临界视界既有闭式解也有明确的存在条件）；把“零和”放回原位（份额层零和、成本层负和，纯零和只是 $\Delta E_{\mathrm{conflict}}\to0$ 的极限）。关于人工智能对齐，主张是有限的：纯工具对齐会被漂移侵蚀（候选推论）；元解码器的稳定性有明确条件，而现实中四条前提都不完全满足，故它目前只是治理目标。

### 9.1 未完成的推导

五处。**其一，$\mathcal{Q}_D$ 的标量化损失**：恢复需扩展成向量（容量、选择性、响应谱、噪声容限）并给出各分量方程，向量分析会失去可解性。**其二，两套模型的对应**：主、辅模型无显式映射，“分层使用、互不替换”是回避而非解决。**其三，$C_D$ 演化的多维性**：式 (IV-3.13) 把复杂度当单一方向上的标量，它实际有深度、宽度、模块化、冗余度多维。**其四，偏离集的完备性**：命题要求偏离集可界定，对固定策略空间可行，对开放式策略空间不可行。**其五，$\mathcal{M}$ 的独立测量**：三条应用推论都要用它，它目前只能由结果反推。

### 9.2 未标定的参数

| 参数 | 标定方法 | 现状 |
| :-------------- | :--------------------- | :---------------------- |
| $\mu_{\mathrm{rec}}$ | 无跃迁期的 $\mathcal{Q}_D$ 增长率拟合 | 需逐域标定 |
| $\delta_{\mathrm{decay}}$ | 无维护对照下的半衰期 | 需逐域标定；朗道尔原理不给出此值 |
| $\kappa_{\mathrm{topo}}$ | 跃迁前后 $\mathcal{Q}_D$ 的跳变幅度 | 需逐案标定 |
| $\zeta$ | 半对数回归（$HⅣ\text{-}7$） | 需多代数据 |
| $\theta_{\mathrm{depth}}/\theta_{\mathrm{cap}}$ | “一层深度相当于几次容量翻倍” | 需专家标定 |
| $\alpha_{\mathrm{L}}$、$\sigma$ | 偏差的收敛时间常数、短期波动 | 需纵向与高频数据 |
| $\Delta_{\mathrm{crit}}$ | 失效案例的偏差水平回溯 | 需案例库 |
| $\Delta I_{\mathrm{coop}}$ 等支付项 | 实验博弈或问卷 | 量级不可靠，排序较可靠 |
| $\eta_C$、$t_{\mathrm{dec}}$、$T_0$ | 跃迁间隔、直接观测、协议规定 | 均可测或可选取 |

“量级不可靠、排序较可靠”决定博弈结论的用法：应以**比较**方式使用——比较同一主体在不同制度下的 $T_{\mathrm{crit}}$，而非报告绝对值。

### 9.3 本卷不主张什么

**不主张解码器必然收敛到某个终态**：所有“趋近”结论都以所列方程与参数区间为限。**不主张存续势可作为现实处置的判据**：$V$ 是描述性量，数值依赖可选择的读数协议。**不主张历史事件可以被模型“解释”**：历史映射是类比而非解释。**不主张人工智能的行为可以被预测**：第六章给出的是条件与判据。**不主张本卷的方程是唯一写法**：换一种形式，定性结论多半不变而定量预测会变。

***

## 附录 A　符号与单位速查表

四列分别是符号、单位、定义、适用范围；跨系统比较前须先读末列。

### A.1 信息与解码器

| 符号 | 单位 | 定义 | 适用范围 |
| :------- | :------ | :----------------------- | :-------------------- |
| $I$、$I_{\mathrm{struct}}$、$I_{\mathrm{causal}}$、$I_{\mathrm{net}}$ | bit | 信息父变量；结构信息；因果信息；$\varphi_{\mathrm{s}}I_{\mathrm{struct}}+\varphi_{\mathrm{c}}I_{\mathrm{causal}}$ | $I_{\mathrm{net}}$ 仅同协议同窗并校准后作数值用 |
| $I_{\mathrm{latent}}$、$I_{\mathrm{active}}$、$I_{\mathrm{orig}}$、$\tilde I_{\mathrm{orig}}$、$I^{+},I^{-},I^{0}$ | bit | 潜在量；$\eta_DI_{\mathrm{latent}}$（§7.1 写作 $\eta_0\mathcal{M}I_{\mathrm{latent}}$，属激活量族）；经验证新增信息；候选信号；冲击净效应分类 | 潜在量不可直测；$I_{\mathrm{orig}}$ 仅事后确认，不作门控输入；$I_{\mathrm{active}}$ 与 $I_{\mathrm{net}}$ 不同名不同量 |
| $I_{\max}$、$\mathcal{Q}_D$、$\mathcal{Q}_{D,\max}$、$I_{\mathrm{ref}}$、$N_{\mathrm{state}}$ | bit、个 | 容量上限；$\eta_DI_{\max}$；承载上限；$\log_2N_{\mathrm{state}}$；最小可区分状态数 | 同谱系内可比，跨架构只作粗排序 |
| $\varphi_{\mathrm{s}},\varphi_{\mathrm{c}}$、$w_{\mathrm{s}},w_{\mathrm{c}}$、$\eta_D$、$\eta_0$、$\Phi$ | 无量纲 | 通道权重；价值权重（和为 1）；解码效率及其上限；神经复杂度（代理） | 权重不构成可加性证明；$\eta_D$ 不定义 $I_{\mathrm{net}}$ |

### A.2 能量、时间与速率

| 符号 | 单位 | 定义 | 适用范围 |
| :--------- | :------- | :------------------------ | :---------------- |
| $E_{\mathrm{eff}}$、$E_{\mathrm{struct}}$、$E_{\mathrm{causal}}$、$E_{\mathrm{build}}$、$E_{\mathrm{build},0}$ | J | 等效成本及分量；一次性建造成本；A3.1 截距 | 建造成本须报分摊规则 |
| $E_{\mathrm{available}}$、$E_{\max}$、$E_{\mathrm{maint}}$、$E_{\mathrm{L,bit}}$、$k_B$、$T_{\mathrm{thermo}}$ | J、$\mathrm{J/bit}$、$\mathrm{J/K}$、K | 可动员预算；环境自由能上限；维持能耗；朗道尔下界 $k_BT_{\mathrm{thermo}}\ln2$；常数与温度 | 朗道尔量仅作量级参考，不给 $\delta_{\mathrm{decay}}$ |
| $\Delta E_{\mathrm{share}}$、$\Delta E_{\mathrm{defend}}$、$\Delta E_{\mathrm{conflict}}$ | J | 合作分担；防御；冲突能耗 | 末项是负和层来源 |
| $T_{\mathrm{struct}}$、$T_{\mathrm{causal}}$、$T_{\mathrm{pred}}$、$T_{\mathrm{min}}$、$T_{\mathrm{env}}$、$\tau_{\mathrm{resp}}$、$T_0$、$T_{\mathrm{crit}}$、$t_{\mathrm{dec}}$、$t_{\mathrm{jump}}$、$T_{\mathrm{exec}}$ | s | 结构寿命；因果作用时间；内生视界；时间粒度；环境特征时间；生态响应延迟；共同核算窗；临界视界；决策周期；跃迁时刻；执行周期 | 不可互换，不裸写 $T$；$\tau_{\mathrm{resp}}$ 待标定；$T_{\mathrm{crit}}$ 仅在情形 (ii) 有限 |
| $\mu_{\mathrm{rec}}$、$\delta_{\mathrm{decay}}$、$\gamma_0$、$\mu_{\mathcal{M}}$、$\nu$、$\alpha_{\mathrm{L}}$ | $\mathrm{s^{-1}}$、各异 | 递归增长率；质量衰减率；基线折旧率；环境漂移敏感系数；补偿系数；偏差学习率 | $\delta_{\mathrm{decay}}$ 与 $\gamma_0$ 粒度不同，不可互代 |
| $\chi$、$\chi_{\mathrm{c}}$、$\tilde{\chi}$、$\tilde{\chi}_{\mathrm{c}}$、$\lambda_{\mathrm{J}}$、$\alpha_{\mathrm{eff}}$、$\delta_{\mathrm{disc}}$、$\delta_{\mathrm{c}}$ | 各异、无量纲 | 自指耦合强度；分岔点；**环路增益 $\chi V^{*}/(1+\chi V^{*})\in(0,1)$**；其临界值 $2/\alpha_{\mathrm{eff}}$；主导特征值；有效扩张指数；贴现因子 $e^{-t_{\mathrm{dec}}/T_{\mathrm{pred}}}$；临界贴现因子 | $\chi$ 族为辅模型专用；$\chi_{\mathrm{c}}$ 不作判据；$\tilde{\chi}$ 无量纲、$\chi_{\mathrm{c}}$ 单位 $\mathrm{J/(bit\cdot s)}$，二者不可互换 |

$\eta_C$ 不在此列：按 (IV-3.13) 的写法其量纲为 $\mathrm{条^{2}/(s\cdot J)}$，与上表各速率的 $\mathrm{s^{-1}}$ 不同；$\pi_V$ 为 $\mathrm{J^{2}/(bit\cdot s)}$，属换算率而非物理速率。

### A.3 存续势、偏差与复杂度

| 符号 | 单位 | 定义 | 适用范围 |
| :---------- | :-------- | :------------------------ | :--------------- |
| $V$、$V_0$、$\Delta V$、$V_{\mathrm{obj}}$、$V^{\mathrm{virt}}$、$V^{\mathrm{val}}$ | $\mathrm{bit\cdot s/J}$ | 存续势、基线与增量；客观、虚拟、价值存续势 | 保留 bit，只有 $V/V_0$ 无量纲；后两项是内部量 |
| $\Delta V^{\mathrm{share}}$、$\Delta V^{\mathrm{cost}}$、$\Delta_{\mathrm{VV}}$、$\Delta_{\mathrm{VV}}^{*}$、$\Delta_{\mathrm{crit}}$、$\sigma$ | $\mathrm{bit\cdot s/J}$、$\mathrm{bit/J}$ | 份额层与成本层变化；脱钩偏差；平衡偏差 $\sigma/(\alpha_{\mathrm{L}}I_{\mathrm{net}})$；容限；偏差产生率 | 零和层须共同口径；$\sigma$ 不是偏差本身 |
| $\Upsilon$、$E_{\mathrm{eff}}^{\mathrm{base}}$、$D$、$D_{\mathrm{phys}}$、$D_{\mathrm{cog}}$、$\Theta$ | 无量纲、J、— | 竞争强度；无冲突等效成本；解码器及两类；参数空间 | 物理类运作期不满足可更新性 |
| $\mathcal{F}$、$\mathcal{T}$、$D_{\mathrm{depth}}$、$C_D$、$C_{\max}$、$\theta_{\mathrm{depth}}$、$\theta_{\mathrm{cap}}$、$\zeta$、$\rho_E$、$L_{\mathrm{lev}}$ | —、无量纲、$\mathrm{bit\cdot s/J^{2}}$ | 递归展开算子；拓扑跃迁算子；规则深度；拓扑复杂度；静态上限；两个权重；成本耦合；预算比；智慧杠杆 | 底数为 2；$C_{\max}$ 是静态边界；$\zeta$ 属假设 A3.1 |
| $\kappa_{\mathrm{topo}}$、$\mathcal{M}$、$\mathcal{N}$、$J_{ij}$ | 无量纲、$\mathrm{s^{-1}}$ | 注入效率；匹配度；环境信号结构；耦合强度矩阵 | $\mathcal{M}$ 独立测量困难；$J_{ij}$ 正合作、负竞争、零隔离 |

**单位约定。** A.3 的 $D_{\mathrm{depth}}$ 以“层”计（无量纲计数）；$C_D$ 是加权复杂度，$C_D$、$\theta_{\mathrm{depth}}$、$\theta_{\mathrm{cap}}$ 以“条”计，$\zeta$ 以 $1/$条计。两者不可混用；本卷的 (IV-3.13) 按“条”核对。

### A.4 博弈与治理

| 符号 | 单位 | 定义 | 适用范围 |
| :-------- | :-------- | :------------------------ | :---------------- |
| $\Pi_{\mathrm{coop}},\allowbreak \Pi_{\mathrm{def}},\allowbreak \Pi_{\mathrm{sucker}},\allowbreak \Pi_{\mathrm{pun}}$ | $\mathrm{bit\cdot s/J}$ | 单轮支付（含 $T_0$，不含 $T_{\mathrm{pred}}$） | 内部评估值；跨主体不可比 |
| $\Delta I_{\mathrm{coop}},\allowbreak \Delta I_{\mathrm{exploit}},\allowbreak \Delta I_{\mathrm{stolen}},\allowbreak \Delta I_{\mathrm{synergy}}$、$I_{A\cup B}$、$E_{A\cup B}$ | bit、J | 合作增量；背叛攫取；被攫取；协同项；合并信息量与合并能耗 | 加法为建模约定，须同协议并去重 |
| $D_{\mathrm{meta}}$、$I_{\mathrm{orig}}^{\mathrm{meta}}$、$\mathcal{D}_i^{\mathrm{dev}}$、$C_i^{\mathrm{punish}}(d)$ | —、bit、$\mathrm{bit\cdot s/J}$ | 元解码器；其共享范式突破信息；可行偏离集；惩罚预期损失（贴现和） | 均衡性须逐条检验；集合须可界定 |

### A.5　单位与量纲核对（重点式）

只收本卷作为判据使用的式。每一行都已逐项相消；未列入的公式在补入判据前须先补全定义或换算。

| 式 | 左端 | 右端 | 核对 |
| :------------ | :----------- | :--------------- | :------------------- |
| (IV-2.1) | $\mathrm{bit\cdot s/J}$ | $(\mathrm{bit}\cdot\mathrm{s})/\mathrm{J}$ | 闭合 |
| (IV-3.8) | 条 | 条 $+$ 条 $\cdot$（无量纲） | 闭合；$I_{\max}$ 与 $I_{\mathrm{ref}}$ 同以 bit 计 |
| (IV-3.9) | 条 | 条 $+$（条/bit）$\cdot$ bit | 闭合 |
| (IV-3.10) | $\mathrm{J}$ | $\mathrm{J}\cdot e^{\text{无量纲}}$ | 闭合；$\zeta C_D$ 无量纲（$\zeta$ 以 1/条 计） |
| (IV-3.12) | 条 | $(1/\text{条})\cdot\ln(\text{无量纲})$ | 闭合；与 (IV-3.10) 同一 $\zeta$ |
| (IV-3.13) | 条/s | $(条^{2}/(s\cdot J))\cdot(J/条)$ | 闭合；$C_D$ 以条计，$\pi_V$ 为 $J^{2}/(bit\cdot s)$ |
| (IV-3.14) | 无量纲 | 无量纲 $\times$ 无量纲 | 闭合；$\mathcal{M}\in[0,1]$ |
| (IV-3.15) | $\mathrm{bit/J}$ | $\mathrm{bit/J}+\mathrm{bit/J}$ | 闭合；$\alpha_{\mathrm{L}}$ 须取 $1/(\mathrm{bit}\cdot\mathrm{s})$ |
| (IV-5.1) | $\mathrm{bit\cdot s/J}$ | $(\mathrm{bit}\cdot\mathrm{s})/\mathrm{J}-(\mathrm{bit}\cdot\mathrm{s})/\mathrm{J}$ | 闭合；$T_0$ 在比较中约去 |
| (IV-5.2) | bit | bit $+$ bit $\cdot(\mathrm{J}/\mathrm{J})$ | 闭合 |
| (IV-5.3) | $\mathrm{bit\cdot s/J}$ | $\mathrm{bit\cdot s/J}+\text{无量纲}\cdot(\mathrm{bit\cdot s/J})/(\text{无量纲})$ | 闭合 |
| (IV-5.4) | $\mathrm{s}$ | $\mathrm{s}/\ln(\text{无量纲})$ | 闭合；须比值 $>1$ 才有正的有限值 |
| (IV-5.5) | $\mathrm{bit\cdot s/J}$ | 两项同为 $\mathrm{bit\cdot s/J}$ | 闭合；两分项须同一核算窗 |
| (IV-5.6) | $\mathrm{bit\cdot s/J}$ | $(\mathrm{bit\cdot s/J})\cdot(\mathrm{J}/\mathrm{J})$ | 闭合 |
| (IV-5.7) | $\mathrm{bit\cdot s/J}$ | $(\mathrm{bit}\cdot\mathrm{s})/\mathrm{J}$；$V_0/(1+\Upsilon)$ | 闭合；$\Upsilon$ 无量纲 |
| (IV-5.8) | bit；$\mathrm{J}$ | bit $+$ bit $+$ bit；$\mathrm{J}+\mathrm{J}-\mathrm{J}$ | 闭合；加法须先声明归属 |
| (IV-5.9) | $\mathrm{bit\cdot J}$ | $(\mathrm{J}\cdot\mathrm{J})\cdot(\mathrm{bit}/\mathrm{J})$ | 闭合 |
| (IV-7.1) | bit | 无量纲 $\cdot$ 无量纲 $\cdot$ bit | 闭合 |
| (IV-7.3) | $\mathrm{J}$ | 在 $\mathrm{J}$ 上取 argmin | 闭合 |
| (IV-7.4) | bit | bit $\cdot(\le1)$ | 闭合 |

**读法。** 表里“闭合”只说明两侧同量纲，不说明该式成立；成立与否由各自的命题前提决定。量纲不闭合则一定不成立，这是本表唯一的判别力，也是它值得单列的理由。

**四组符号陷阱**：六个时间量不可互换，最常错的是把 $T_{\mathrm{pred}}$ 与 $T_{\mathrm{struct}}$ 混用；$V$ 带 bit 不是无量纲；$\mathcal{Q}_D$ 与 $I_{\max}$ 在满效率时数值相等但含义不同，后者只在跃迁时改变；两套临界值不可互换，本卷只用 $\mu_{\mathrm{rec}}/\delta_{\mathrm{decay}}$ 作判据。

***

## 参考文献

1. Friston, K., FitzGerald, T., Rigoli, F., Schwartenbeck, P., & Pezzulo, G. (2017). Active inference: A process theory. *Neural Computation*, 29(1), 1–49.
2. Amodei, D., Olah, C., Steinhardt, J., Christiano, P., Schulman, J., & Mané, D. (2016). Concrete problems in AI safety. *arXiv:1606.06565*.
3. Ashby, W. R. (1956). *An Introduction to Cybernetics*. Chapman & Hall.
4. Wiener, N. (1948). *Cybernetics: Or Control and Communication in the Animal and the Machine*. MIT Press.
5. Landauer, R. (1961). Irreversibility and heat generation in the computing process. *IBM Journal of Research and Development*, 5(3), 183–191. https://doi.org/10.1147/rd.53.0183
6. Shannon, C. E. (1948). A mathematical theory of communication. *Bell System Technical Journal*, 27(3), 379–423. https://doi.org/10.1002/j.1538-7305.1948.tb01338.x
7. Nash, J. (1950). Equilibrium points in $n$-person games. *Proceedings of the National Academy of Sciences*, 36(1), 48–49. https://doi.org/10.1073/pnas.36.1.48
8. Selten, R. (1965). Spieltheoretische Behandlung eines Oligomodells mit Nachfrageträgheit. *Zeitschrift für die gesamte Staatswissenschaft*, 121, 301–324.
9. Axelrod, R. (1984). *The Evolution of Cooperation*. Basic Books.
10. Nowak, M. A. (2006). Five rules for the evolution of cooperation. *Science*, 314(5805), 1560–1563.
11. Kramers, H. A. (1940). Brownian motion in a field of force and the diffusion model of chemical reactions. *Physica*, 7(4), 284–304.

***

<!-- VOLUME Z ｜ 现实映射词典：数学式与叙事 -->
## 卷Z　现实映射词典：数学式与叙事

> **本卷＝卷Z。**

## 第零章　使用说明

本卷是**数学—叙事对照手册**：把已经写成方程的东西翻译成人话、画面和故事。它不证明那些方程，也不替它们加固。由此有一条硬约束——**叙事的强度必须等于、或低于被叙述的条目**。故事最容易失真：删掉条件句之后它读起来更顺，而条件句恰恰是全部内容。

> **本卷不产生新的数学结论。凡本卷某句话读起来比它所对应的形式化条目更强，以形式化条目为准，那句话作废。**

全卷只用四个标签。它们不是修辞，是读法说明——看到标签，就知道这句话能被推到多远。

| 标签 | 含义 | 该怎么读 |
| :--------- | :--------------------- | :--------------------------- |
| **【定理】** | 前提已列全、推导完整，结论在该前提下严格成立 | 前提成立则结论成立；要反驳，只能去查前提。本卷只用它转述已有完整推导的物理下界，不新增此类条目 |
| **【命题】** | 有形式化陈述，但前提部分待标定，或某一步依赖尚未证明的建模假设 | 在所列条件下成立；条件拿掉，结论就没了 |
| **【候选推论】** | 由某条命题在附加条件下导出，尚未独立检验 | 母命题与附加条件都成立时，应当观察到…… |
| **【假说】** | 经验性或机制性猜测，没有形式化推导 | 这是一个可检验的猜测，不是结论 |

三条读法。其一，**等级随条目走，不随章节走**。其二，**降级比升级容易，也更重要**：只能证明“增长率转负”的，不写成“存量归零”。其三，**未标等级的文字不构成理论主张**——举例、类比、吐槽都是叙述材料，不承担证据责任。

条件句是正文，不是免责声明。结构：使用说明｜概念映射（一—五章）｜规范化表述（六章）｜寓言（七章）｜变量小传（八章）｜附录。

**现实映射的边界。** 本卷把模型条款翻译成日常场景，场景只是例子，不是对任何具体个人、群体或制度的判断。凡涉及资源匮乏、阶层、健康、家庭、政治体制的描述，都是在给定参数下“若参数如此，则条款如此”的条件句；参数不能从身份标签读出，条款也不能反过来用于评价现实中的某个群体。本卷不构成对任何现实个体的预后判断、医疗建议或行为正当性依据。

***

## 第一章　存续势的众生相：五种活法的热力学肖像

**与卷Ⅰ §5.6 的关系。** 本节把卷Ⅰ §5.6 的四类极限行为，按 $(E_{\mathrm{eff}}, \rho, r_{\mathrm{v}}-\gamma_0)$ 的区间重排为五个叙事相：饱和、阻尼、失稳、坍缩、跃迁。**这是分类学的重排，不是新的动力学结论**；「失稳态」是四类之间的高耗能过渡区，不是新的吸引子。凡本节与卷Ⅰ §5.6 冲突，以 §5.6 为准。

如果把宇宙看作一家只收热力学货币的公司，每个持久结构，从细菌到文明，都是这家公司的员工。有的在稳态养老，有的在贫困陷阱里慢性失血，有的在烧钱狂奔，有的已经走进热力学坟墓。本章用五个相态给这些活法拍一张 CT。

**符号约定。** $V$ 是存续势，量纲 $\mathrm{bit\cdot s/J}$，基本形式 $V\approx I_{\mathrm{net}}T_{\mathrm{causal}}/E_{\mathrm{eff}}$：用多少能量代价、维持多少有效信息、撑多长时间。$I_{\mathrm{net}}$ 以 bit 计，时间以 s 计，能量以 J 计；只有归一化后的 $v=V/V_0$ 才是无量纲量。裸写的 $I$ 默认指 $I_{\mathrm{net}}$；两个可测通道写全为结构信息 $I_{\mathrm{struct}}$（bit）与有效因果信息 $I_{\mathrm{causal}}$（bit）。$I_{\mathrm{net}}$ 是按能量份额加权的模型量，不是直接读出的实测值。

$E_{\mathrm{eff}}$ 是等效热力学成本（J）；$E_{\mathrm{floor}}$ 是维持结构与自维持边界不可再压的那部分能量流（J），是 $E_{\mathrm{eff}}$ 的下沿。$\rho$ 是竞争压力（无量纲，$0\le\rho\le1$）；$\Delta_{\mathrm{VV}}$ 是脱钩偏差（$\mathrm{bit\cdot s/J}$）；$r_{\mathrm{v}}$ 是存续驱动率（$\mathrm{s^{-1}}$）；$\gamma_0$ 是基线折旧率（$\mathrm{s^{-1}}$）。

### 1.1 饱和态：躺平者的热力学合法性

**数学肉身：**

$$
E_{\mathrm{eff}} \ge E_{\mathrm{floor}}, \quad \rho \to 0, \quad \Delta_{\mathrm{VV}} \to 0, \quad r_{\mathrm{v}} > \gamma_0, \quad V = V_{\max} \tag{Z-1.1}
$$

**直觉等价物**：退休人士、垄断收租企业、北欧福利国家、树懒。

饱和态是**容量用满后的不动点**：能量转移不仅覆盖折旧、还有余量（$r_{\mathrm{v}}>\gamma_0$），外部竞争趋零，内部评估与现实对齐，$V$ 升到容量上限后停住。需要分清一个近邻情形：若 $r_{\mathrm{v}}=\gamma_0$，$V$ 只是停在初值上，既不升也不降——那是退化平衡，不是饱和；饱和要求的是先有净增长、再把容量用满。

### 1.2 阻尼态：贫困陷阱里的慢性失血

**数学肉身：**

$$
E_{\mathrm{eff}} \approx E_{\mathrm{floor}}, \quad \rho \to 0, \quad \Delta_{\mathrm{VV}} \to 0, \quad r_{\mathrm{v}} < \gamma_0 \tag{Z-1.2}
$$

**直觉等价物**：极贫地区、996 却存不下钱的白领、代谢综合征患者。

阻尼态的残酷在于：支付的能量连底线都勉强，驱动力抵不过折旧，于是慢性衰亡，可用的通道逐渐闭合。这里 $\mathrm{d}V/\mathrm{d}t<0$：结构没有立即崩溃，但它在缓慢溶解。

**$r_{\mathrm{v}}<\gamma_0$ 只保证 $V$ 在往下走，不保证 $V$ 会走到零。** 往下走和走到零是两件事，中间隔着一个“能不能停在新平衡点”的问题——答案在 1.4。

### 1.3 失稳态：短视狂奔者的能量烟花

**数学肉身：**

$$
E_{\mathrm{eff}} \gg E_{\mathrm{floor}}, \quad \rho \gg 0, \quad \Delta_{\mathrm{VV}} > 0, \quad r_{\mathrm{v}} > \gamma_0 \tag{Z-1.3}
$$

**直觉等价物**：芯片军备竞赛、AI 奖励黑客、创业公司烧钱、赌徒。

失稳态是这套相图里最危险的相态之一：系统拼命烧能量，却永远摸不到饱和。芯片军备竞赛是合适的样本：每家公司都在堆算力，$\rho$ 迫使没有人敢先停手，所有参与者都知道这种增长不可持续（$\Delta_{\mathrm{VV}}>0$，估值脱离物理现实）。赌徒是它的微缩版：赌局与“下一把就能翻本”阻止他们进入饱和。

### 1.4 坍缩态：底层互害与热力学死亡

**数学肉身：**

$$
E_{\mathrm{eff}} \to E_{\mathrm{floor}}, \quad \rho \gg 0, \quad \Delta_{\mathrm{VV}} \to 0, \quad r_{\mathrm{v}} < \gamma_0 \tag{Z-1.4}
$$

**直觉等价物**：能量见底时的恶性竞争、生态灭绝、文明崩溃、细胞凋亡。

坍缩态是系统的热力学死亡：能量见底，竞争惨烈，净增长停摆，走向物理解体，结构被抹平为势垒残骸或废热。

**触发损伤不等于判死刑。** 损伤项被激活，它做的事只是把净增长率压下一截；压到零以下，才是真正的倒计时。设触发后的有效净增长率为 $r_{\mathrm{v}}-\gamma_0-\delta_{\mathrm{dam}}$，其中 $\delta_{\mathrm{dam}}>0$ 是损伤项折算出的衰减率（$\mathrm{s^{-1}}$），则只有三种归宿：

**情形一：$r_{\mathrm{v}}-\gamma_0<\delta_{\mathrm{dam}}$，归零型。** 净增长率转负，$V$ 单调衰减到零。这是真正的崩溃，也是“坍缩”一词最严格的用法。

**情形二：$r_{\mathrm{v}}-\gamma_0>\delta_{\mathrm{dam}}>0$，降阶型。** 增长项仍强于损伤项，系统不归零，而是降到一个新的、较低的正平衡：

$$
V^{*}=V_{\max}\left(1-\frac{\delta_{\mathrm{dam}}}{r_{\mathrm{v}}-\gamma_0}\right) \tag{Z-1.5}
$$

它残了，但没死。长期带病运营的组织、器官受损但仍能维持的个体，都属于这一情形。把它叫作“崩溃”是错的，它只是“降级”。

**情形三：$r_{\mathrm{v}}<\gamma_0$ 且损伤同时触发，加速崩溃。** 两股力量同向，衰减加速，崩得比情形一更快、更陡。这是坍缩态真正的样子：本来就入不敷出，又挨了一下。

还有一处细节：坍缩态里 $\Delta_{\mathrm{VV}}\to0$ 并不意味着健康，而是系统连自欺的力气都没有了——虚拟势与客观势贴在一起，是因为两边同时掉到了地板上。

### 1.5 跃迁态：那些极少数的越狱者

**数学肉身：**

$$
\mathcal{T}(I_{\mathrm{orig}})\ \text{触发}, \qquad I_{\max}(D_{n+1}) > I_{\max}(D_{n}) \tag{Z-1.6}
$$

**直觉等价物**：寒武纪大爆发、科学革命、个人顿悟。

并非所有系统都困在四个相态的循环里。极少数结构能触发**拓扑跃迁** $\mathcal{T}$，撞破一堵墙，进入新的解码器层次。解码器 $D$ 指结构从环境中提取有效信息的物理机制，$I_{\max}(D)$ 是它的最大信息容量（bit），$I_{\mathrm{orig}}$ 是现有解码器提取不出、需要新解码器才能提取的那部分信息（bit）。

跃迁不是渐进优化，而是**相变**，像水在 100 °C 突然变成蒸汽：系统跨过一次性的建造成本 $E_{\mathrm{build}}$（J）之后，$I_{\max}(D)$ 被抬到一个新水平，整个通道的拓扑被重构。限定一句：$I_{\max}(D_{n+1})>I_{\max}(D_{n})$ 是跃迁的**结果**，不是它的充分条件；能不能跃迁，还要看三张许可证。

### 1.6 四大全局吸引子：文明的终局菜单

**数学肉身：**

| 吸引子 | 极限域条件（限于适用域内） | 动力学结果（能量转移视角） |
| :---------- | :------------------- | :---------------------------- |
| **饱和吸引子** | $\inf E_{\mathrm{total}}>E_{\mathrm{floor}}>0$，$\rho\to 0$，$\Delta_{\mathrm{VV}}\to 0$，$T_{\mathrm{struct}}^{\max}$ 在适用域内有限且被推到上沿 | $V(t)\to V_{\max}$（能量转移达到动态平衡，通道稳定） |
| **坍缩流形** | $\rho\gg 0$ 且阈值触发、$\delta_{\mathrm{dam}}>0$（不绑净增长率的符号） | 按 $g_{\mathrm{net}}=(r_{\mathrm{v}}-\gamma_0)-\delta_{\mathrm{dam}}$ 分三种：$>0$ 降到较低正平衡 $V^{*}$（存量被压但仍在运行）；$<0$ 且 $r_{\mathrm{v}}\ge\gamma_0$ 归零；$<0$ 且 $r_{\mathrm{v}}<\gamma_0$ 加速归零 |
| **拓扑跃迁** | 在适用域内 $T_{\mathrm{struct}}^{\max}$、$I_{\max}$ 的**有限提升**（算子 $\mathcal{T}$ 触发） | $\mathrm{d}V_{\max}/\mathrm{d}t>0$（通道发生相变，带宽提高一档） |
| **度规替换** | $\Delta_{\mathrm{VV}}\gg 0\Rightarrow D\to D'$ | 原测度下 $V\to 0$，新测度 $D'$ 主导流场 |

**“有限提升”这四个字要读重。** 拓扑跃迁一栏不是 $T_{\mathrm{struct}}^{\max}\to\infty$ 或 $I_{\max}\to\infty$——那是数学极限假设，不是现实判据。两个上限都被物理封住：结构存续时间受材料强度、能量供给、环境扰动与宇宙年龄约束；解码器容量受质量、温度与散热约束。现实中的跃迁是在适用域内把上限抬高一截。

### 1.7 完整不等式约束系统：宇宙的考勤表

**数学肉身：**

$$
\begin{aligned}
& I_{\min} \le I_{\mathrm{net}} \le I_{\max}(D), \quad T_{\min} \le T_{\mathrm{struct}} \le T_{\mathrm{struct}}^{\max}, \quad E_{\mathrm{floor}} \le E_{\mathrm{eff}} \le E_{\mathrm{available}}, \\
& 0 \le \rho \le 1, \quad \Delta_{\mathrm{VV}} \ge 0, \\
& \text{崩溃：}\ \big[(E_{\mathrm{eff}}>E_{\mathrm{thresh}})\wedge(r_{\mathrm{v}}-\gamma_0<\delta_{\mathrm{dam}})\big] \vee (r_{\mathrm{v}}<\gamma_0\ \text{不可逆持续}) \Rightarrow V\to 0
\end{aligned} \tag{Z-1.7}
$$

**直觉等价物**：宇宙的考勤表。每天打卡：信息在 $I_{\min}$ 与 $I_{\max}(D)$ 之间、能量在 $E_{\mathrm{floor}}$ 与 $E_{\mathrm{available}}$ 之间、$\rho\in[0,1]$、$\Delta_{\mathrm{VV}}\ge0$（定义域约定，取绝对值）。

**与卷Ⅰ §5.7 是同一组约束，只有一处名称差。** 上界卡的是**可用预算** $E_{\mathrm{available}}$，不是供给上限 $E_{\max}$（$E_{\mathrm{available}}\le E_{\max}$，见卷Ⅰ §2.2 记号表）；时间上界一律写 $T_{\mathrm{struct}}^{\max}$，不另设 $T_{\mathrm{pred}}^{\max}$。$E_{\mathrm{floor}}$、$E_{\mathrm{struct}}^{\min}$ 与 $E_{\mathrm{eff}}$ 的关系按卷Ⅰ §2.2：$E_{\mathrm{eff}}\ge E_{\mathrm{floor}}\ge E_{\mathrm{struct}}^{\min}>0$，存量口径与成本口径不可互相代入，也不可相减。此外，卷Ⅰ §5.7 还列了饱和条件、损伤触发、净增长判据、带伤平衡四项，本节只写崩溃条件，余项见该处。

**崩溃条件是一张两栏的辞退通知，两栏同时满足才生效**：能量账单越过损伤阈值，**并且**净增长率被压到零以下。只满足第一栏，你被降级；两栏都满足，你才被开除。若驱动力长期低于折旧率且不可逆，即使没有越阈值，也一样被开除——这是另一条独立通道。

### 1.8 生态位容量的自由能通量标度（假说）：文明能装多少水

**数学肉身：**

$$
V_{\max} \propto \alpha_{\mathrm{cap}}\,\frac{\dot F_{\mathrm{avail}}}{\sigma_{\min}\,\gamma_0},\qquad \alpha_{\mathrm{cap}}>0 \tag{Z-1.8}
$$

其中 $\dot F_{\mathrm{avail}}$ 是环境可用自由能通量（W），$\sigma_{\min}$ 是维持生态位资源循环所需的最小熵产率，$\gamma_0$ 是基线折旧率（$\mathrm{s^{-1}}$）。量纲上，右边是能量除以熵产率，与 $V_{\max}$ 的 $\mathrm{bit\cdot s/J}$ 之间差一个容量系数 $\alpha_{\mathrm{cap}}$（单位 $\mathrm{bit/(J\cdot K)}$，待标定）。所以它是**比例关系，不是物理上界**——写成“$\le$”会把一条现象学标度升格成硬约束，故此处用“$\propto$”。这条式子只用于**比较容量排序**，不用于给出绝对数值。

**直觉等价物**：文明的上限不由野心决定，由环境自由能通量决定。这是木桶效应：能源、算力、时间窗口、竞争烈度，最短的那块板决定文明能装多少水。

### 1.9 趋同：牌桌的规则不由你定

**数学映射：** 筛选论证。在有限能量、有限时间与有限信息处理能力下，$V$ 较低的构型更容易被淘汰，存活下来的构型集中在少数几类可行解上。它与热力学第二定律相容，但不是它的直接推论——依赖“淘汰压力持续存在”与“变异空间足够遍历”两个前提，而这两个前提在短窗口内都可能不成立。

**直觉等价物**：你可以在牌桌上自由出牌，但牌桌的规则不由你定。眼睛在不同谱系里独立演化过多次：光在介质里的传播规律对所有人都一样：约束相同，可行解就那么几类。局部策略层的自由是真的，筛选层不改变标准，只筛选后果。这是筛选论，不是宿命论。

***

## 第二章　解码器演化史：从原子到 AI 的感知革命

解码器 $D$ 是能量转移的物理通道。从原子到 AI，宇宙一直在试着造更好的通道，每一次重大升级都是撞破一堵墙。墙不是比喻上的困难，而是**约束的类型换了**：晶体撞的是势垒，RNA 撞的是噪声，神经系统撞的是时间，语言撞的是个体边界，AI 撞的是自指。每撞破一堵，带宽上一个台阶，同时新增一类失效方式。

### 2.1 第一堵墙：晶体的永恒冬眠

**数学映射：**

$$
V_{\mathrm{obj}} = V_{\mathrm{s}} = \frac{I_{\mathrm{struct}}\,T_{\mathrm{struct}}}{E_{\mathrm{struct}}}, \qquad I_{\mathrm{causal}} = 0, \quad E_{\mathrm{causal}} = 0 \tag{Z-2.1}
$$

晶体是持久结构的原型：靠深势垒 $E_{\mathrm{barrier}}$（J）被动锁定，无持续耗散，无内部模型。花岗岩可以存续十亿年，但它永远不会知道自己存在了十亿年；它的信息是冻结的，没有写入，没有读出，也没有维护成本，归于 $D=\varnothing$，属被动相。它的高 $V_{\mathrm{obj}}$ 完全来自 $T_{\mathrm{struct}}$ 长、$E_{\mathrm{struct}}$ 小，不是来自 $I_{\mathrm{struct}}$ 大。**冻结的信息很便宜，活的信息很贵。** 

### 2.2 第二堵墙：RNA 的原始觉醒

**数学映射：**

$$
E_{\mathrm{causal}} > 0, \qquad I_{\mathrm{net}} = \varphi_{\mathrm{s}}I_{\mathrm{struct}} + \varphi_{\mathrm{c}}I_{\mathrm{causal}} > 0 \tag{Z-2.2}
$$

其中 $\varphi_{\mathrm{s}}=E_{\mathrm{struct}}/E_{\mathrm{eff}}$、$\varphi_{\mathrm{c}}=E_{\mathrm{causal}}/E_{\mathrm{eff}}$，二者之和为 1。这是按能量份额做的加权合成，属建模约定，不是可加性定理。

RNA 世界是解码器史上的第一次越狱：分子不再是被动晶体，而是开始主动复制、催化与选择。这是 $E_{\mathrm{causal}}$ 从零到正的临界点——结构开始支付能量来处理信息。但它的解码器极其简陋：$\eta_D$ 很低，$T_{\mathrm{pred}}$ 几乎为零，没有预测，只有反应。

### 2.3 第三堵墙：神经系统的预测革命

**数学映射：**

$$
T_{\mathrm{pred}} > 0, \qquad V_{\mathrm{c}} = \frac{I_{\mathrm{causal}}\,T_{\mathrm{causal}}}{E_{\mathrm{causal}}} > 0 \tag{Z-2.3}
$$

神经系统的出现让时间被**内生化**了：结构不再只活在 $T_{\mathrm{struct}}$ 里，而是获得了 $T_{\mathrm{pred}}$，能预测未来并据以调整当下行为，认知通道 $V_{\mathrm{c}}$ 由此打开。这是从“反应”到“预测”的相变——一条鱼躲开捕食者，是神经系统提前表征了“被咬”这件事，不必等被咬。

但 $T_{\mathrm{pred}}$ 一旦成为内生变量，就可以被压缩（短视）或膨胀（幻觉）。$T_{\mathrm{pred}}$ 是“我能规划多远”，$T_{\mathrm{causal}}$ 是“我的动作在世界上留下多久的后果”。一个短视的帝国可以留下千年的制度后果，一个规划百年的企业可能什么都没留下；两者不同步，正是许多历史误判的来源。

### 2.4 第四堵墙：语言与文明的集体外挂

**数学映射：**

$$
I_{\mathrm{orig}}\ \text{注入}, \qquad D_{\mathrm{depth}}^{\mathrm{dyn}} = 1 + \#\{\mathcal{T}\} \tag{Z-2.4}
$$

语言是人类解码器的第一次外化：在此之前 $D$ 被困在个体颅骨内，语言让它可以跨个体、跨代际传播。文明是一个巨大的分布式解码器——每个成员只持有局部 $D$，集体却形成了一个规则深度很高的网络。

**规则深度 $D_{\mathrm{depth}}$ 有两个定义，必须分开说。** **静态定义**是结构存续时必须同时维持的独立规则层数，可按功能清单去数。**动力学写法**是深度指数 $D_{\mathrm{depth}}^{\mathrm{dyn}}\equiv1+\#\{\mathcal{T}\}$，即“初始一层加历次拓扑跃迁次数”，式 (Z-2.4) 用的是后者。

**“每次跃迁恰好增加一层独立规则”是标定假设，不是从定义推出的等式。** 有些跃迁增加好几层（文字同时带来记录、检索与跨代校验），有些只是把旧层替换掉。两者是否吻合是可检验的经验问题：横轴放跃迁次数、纵轴放静态深度做回归，看斜率是不是 1；斜率显著偏离 1，就说明该假设在该样本上不成立，此时只用静态定义，不做外推。

$D_{\mathrm{depth}}$ 与 $I_{\mathrm{struct}}$ 不是同一方向上的量：结构可以很大但很浅（章鱼），也可以很深但不一定很大。把两个维度压成一个“复杂度”数字，是跨物种比较多半会翻车的原因。

### 2.5 第五堵墙：AI 的递归噩梦

**数学映射：**

$$
\chi > \chi_{\mathrm{c}}, \qquad \Delta_{\mathrm{VV}} \gg 0, \qquad \rho \to 1 \tag{Z-2.5}
$$

硅基解码器的 $E_{\mathrm{struct}}$ 极小（没有肉身维持成本），$\gamma_0$ 极小（没有自然折旧），这让它可以持续递归展开算子 $\mathcal{F}$，却不容易触发真正的拓扑跃迁 $\mathcal{T}$。更麻烦的是自指耦合 $\chi$（系统用当前存续状态反馈加速信息提取的回路强度，无量纲）：虚拟存续势开始自我放大，$\chi$ 越过分岔点时进入短视失控态。这是第五堵墙——解码器开始燃烧自己照亮幻觉。

$\chi_{\mathrm{c}}$ 是**模型内的分岔点**，不是现实判据：它来自一组简化方程，换一套模型就换一个数值。把它当成“智能体的安全红线”，是把模型当成了现实；要判断真实系统是否失控，可用的代理是偏差比值 $\Delta_{\mathrm{VV}}/\Delta_{\mathrm{crit}}$。

### 2.6 复杂度跃迁的三个条件：越狱许可证

**数学肉身：**

**条件 1，信号可用性**：环境中必须存在范式突破信号 $I_{\mathrm{orig}}$，使得当前解码器提取不出它（$D_n(I_{\mathrm{orig}})\approx0$），而重组后的解码器可以（$D_{n+1}(I_{\mathrm{orig}})\gg0$）。

**条件 2，能量可用性：**

$$
E_{\mathrm{build}}(D_{n+1}) < E_{\mathrm{available}} \tag{Z-2.6}
$$

**条件 3，智慧杠杆：**

$$
L_{\mathrm{lev}} = \frac{V(D_{n+1}) - V(D_{n})}{E_{\mathrm{build}}} > L_{\mathrm{lev,min}} \tag{Z-2.7}
$$

三条可以排成一张可判定的表：

| 条件 | 判据 | 需要观测什么 | 不满足时的表型 |
| :------- | :----------------- | :----------------- | :--------------- |
| **信号可用** | 现有解码器在目标上的残差显著高于其历史残差分布 | 残差的稀有度读数、独立复现 | 系统在旧范式内持续微调，看不到“异常” |
| **能量可用** | $E_{\mathrm{build}}<E_{\mathrm{available}}$ | 建造期总投入、可用自由能预算 | 想法有了，做不出来；蓝图长期停在纸上 |
| **杠杆足够** | $L_{\mathrm{lev}}>L_{\mathrm{lev,min}}$ | 新旧解码器在同目标、同观察窗、同能量分摊下的 $V$ 差 | 升级完成但得不偿失，随后回退 |

两点说明。其一，三条是**必要条件**，不是充分条件：全满足仍可能因为时机、路径依赖或协调失败而不发生跃迁。其二，$L_{\mathrm{lev,min}}$ 不是普适常数，是因系统而异的决策阈值。

### 2.7 三轴结构坐标系：为什么“人类比细菌复杂”是个坑

**数学映射：**

$$
I \;\longrightarrow\; \left( I_{\mathrm{rule}},\; D_{\mathrm{depth}},\; F_{\mathrm{scale}} \right) \tag{Z-2.8}
$$

其中 $I_{\mathrm{rule}}$ 是最小生成规则的复杂度（bit），$D_{\mathrm{depth}}$ 是同时维持的独立规则层数（无量纲），$F_{\mathrm{scale}}$ 是规则被递归展开的规模（无量纲倍数）。

**直觉等价物**：传统信息论试图给任何结构赋予单一数值 $I=\log_2\Omega$ 并据此排名，这条路走不通，因为不同系统的状态空间不可通约，就像问“红色有多重”。正确的几何是多维的：

| 结构 | $D_{\mathrm{depth}}$ | 构型容量 | 注释 |
| :---------- | :-------------- | :------------ | :-------------------- |
| 晶体 | 1（低） | 低 | 单一规则，靠极高的 $F_{\mathrm{scale}}$ 广泛部署 |
| 章鱼 | 低 | 高 | 一次主要跃迁，然后极端展开 |
| 人类 | 高（十以上） | 高 | 多层叠加约束，加复杂内部拓扑 |
| 细菌 | 低 | 中等 | 古老，但在其层级上热力学效率极高 |

构型容量指该结构在保持自身同一性或功能的前提下，能呈现的可区分构型数的对数（bit）。

### 2.8 负拓扑跃迁：退化也是策略

**数学映射：**

$$
\mathcal{T}^{-}:\quad \Delta D_{\mathrm{depth}} = -1 \quad \text{当}\quad \frac{\partial V}{\partial D_{\mathrm{depth}}} < 0 \tag{Z-2.9}
$$

**直觉等价物**：演化不是单向进步。维持一个约束层的成本超过它对 $V$ 的贡献时，该层会被脱落。

这里有一层限定：$\partial V/\partial D_{\mathrm{depth}}<0$ 是**当下的边际判断**，依赖当前环境。环境一旦变回需要那一层的样子，被丢掉的层往往捡不回来——重建要重新支付 $E_{\mathrm{build}}$，而重建窗口未必还在。这就是退化的真实代价：省下当期维护费，押上未来的选择权。

***

## 第三章　时间管理大师：谁在掌控自己的时间？

时间是宇宙最公平的资源：每个持久结构都拥有它，但并非每个结构都能管理它。本章要把“时间”这个词拆开——拆不开，后面所有讨论都会打滑。

本章只用六个记号，绝不混用，也不裸写 $T$ 指代其中任何一个：

| 符号 | 单位 | 含义 | 谁决定它 |
| :----------- | :----------- | :---------------- | :------------------ |
| $T_{\mathrm{struct}}$ | s | 结构存续时间 | 材料、能量供给、环境扰动 |
| $T_{\mathrm{causal}}$ | s | 因果效果持续时间 | 动作的传播范围与衰减机制 |
| $T_{\mathrm{pred}}$ | s | 预测视界 | 解码器的内生规划跨度 |
| $T_{\mathrm{min}}$ | s | 时间粒度 | 系统能分辨的最小间隔 |
| $T_{\mathrm{env}}$ | s | 环境特征时间 | 环境本身的变化周期 |
| $T_{\mathrm{thermo}}$ | K | 温度 | 热浴，不参与时间比较 |

前五个是时间，第六个是温度——它只是借用了同一个字母的写法，量纲完全不同，任何时候都不参与时间的比较。

最容易被混掉的是三个。一块石碑的 $T_{\mathrm{struct}}$ 可以是三千年，$T_{\mathrm{causal}}$ 接近于零（它不影响任何事），$T_{\mathrm{pred}}$ 是零（它不预测）。一个短命的宣传机构可能只有三年 $T_{\mathrm{struct}}$，却有三十年的 $T_{\mathrm{causal}}$，$T_{\mathrm{pred}}$ 是三个月。三者的组合方式，比任何单一数字都更能说明一个结构是什么。

另外两个记号负责“分辨率”与“外部节奏”。$T_{\mathrm{pred}}\ll T_{\mathrm{env}}$ 时，长视界没有意义——环境还没变，你看得再远也用不上；$T_{\mathrm{pred}}\gg T_{\mathrm{env}}$ 时，长视界反而危险——你在按旧地图走新地形。真正的时间管理，是让两者保持恰当比例，而不是一味求长。

本章只做现实投影，不做数学推导：所有结论都来自前面的相态结构。

### 3.1 生与死：一道信息鸿沟

**数学投影：** 活着的系统，

$$
V_{\mathrm{obj}} = \underbrace{\frac{I_{\mathrm{struct}}\,T_{\mathrm{struct}}}{E_{\mathrm{struct}}}}_{V_{\mathrm{s}}} + \underbrace{\frac{I_{\mathrm{causal}}\,T_{\mathrm{causal}}}{E_{\mathrm{causal}}}}_{V_{\mathrm{c}}}, \qquad I_{\mathrm{net}} > 0, \quad T_{\mathrm{pred}} > T_{\mathrm{min}} \tag{Z-3.1}
$$

死后的系统，

$$
V_{\mathrm{obj}} \to V_{\mathrm{s}} = \frac{I_{\mathrm{struct}}\,T_{\mathrm{struct}}}{E_{\mathrm{struct}}}, \qquad I_{\mathrm{causal}} = 0, \quad T_{\mathrm{pred}} = 0 \tag{Z-3.2}
$$

**直觉等价物：** 一块花岗岩和一具刚断气的动物尸体，在这本账里**没有本质区别**：$E_{\mathrm{causal}}=0$，$T_{\mathrm{pred}}=0$，都只剩结构通道。

**死亡不是结构的瓦解，而是信息的熄灭。** 它真正丢失的是**因果效力**：再也无法对环境施加任何 $I^{+}$ 或 $I^{-}$，再也无法预测、规划、干预。这就是为什么生物普遍抗拒死亡——怕的是从主动相不可逆地退回被动相。

补一句边界：以上说的是“在这套记账口径下，死亡意味着什么”，不是“死亡对当事人意味着什么”。模型描述的是通道的关闭，不是体验的终止。

### 3.2 内生时间的双维性：长度与精度

**数学投影：** $T_{\mathrm{pred}}$ 不是标量，而是具有两个正交属性的结构：

| 维度 | 符号 | 定义 | 物理含义 |
| :--------- | :--------- | :------------------- | :------------------ |
| **长度** | $L_{\mathrm{pred}}$ | 满足置信度阈值的最大预测时域（s） | 系统规划的最远时间边界 |
| **精度** | $G_{\mathrm{pred}}$ | $-\log_2\left(T_{\mathrm{min}}/T_{\mathrm{ref}}\right)$（bit），定义域 $T_{\mathrm{min}}\le T_{\mathrm{ref}}$ | 系统可分辨的最小时间粒度的对数 |

其中 $T_{\mathrm{ref}}$ 是参考时间尺度（s，取系统特征采样周期或 1 s，用于把比值无量纲化）。定义域那一栏不能省：没有 $T_{\mathrm{min}}\le T_{\mathrm{ref}}$，“精度”会取到负值，四象限的坐标随之失去意义。

**直觉等价物：** 长度是望远镜的口径，精度是望远镜的分辨率。一个人可以说“我五年内要财务自由”（长度长，精度粗），也可以说“我明天下午三点一刻在咖啡馆见客户”（长度短，精度细）。**真正的时间管理能力，是同时在两个维度上扩展。** 只有长度，你是空想家；只有精度，你是瞎忙者。

### 3.3 四象限时间管理者：从石头到乌鸦

**数学投影：** 以 $(L_{\mathrm{pred}},G_{\mathrm{pred}})$ 为坐标轴：

| 结构 | $L_{\mathrm{pred}}$（长度） | $G_{\mathrm{pred}}$（精度） | 比喻 | 管理方式 |
| :--------- | :--------- | :-------------- | :-------- | :-------------- |
| **石头** | $0$ | $0$ | 盲目木偶 | 不管理（从未拥有时间维度） |
| **植物种子** | 长（$O(10^{1})$ 月） | 极低（只能区分旱季与雨季） | 定好的闹钟 | 被动对齐自然节律，粗粒度押注 |
| **水熊虫** | 短（$O(10^{-1}\sim 10^{1})$ 小时） | 中等（能感知湿度变化速率） | 高频开关 | 高频开关，战术精确但战略短视 |
| **鸟类（乌鸦）** | 长（$O(10^{1}\sim 10^{2})$ 天） | 高（能精确到具体地点与时间） | 实时导航仪 | 实时导航，战略与战术双优 |

**关键洞察：** 种子赌的是“未来会有雨季”，不是“下周三下午下雨”；这种**粗粒度长视界**是低成本策略，预测错了还有厚种皮与种群分散兜底。水熊虫相反，必须精确判断“湿度下降速率是否超过阈值”，脱水时机差几分钟就是生死之别，代价是 $E_{\mathrm{causal}}$ 持续燃烧、且没有兜底。乌鸦两个维度同时扩展，代谢账单也最高。

### 3.4 精度即权力：为什么“明天下午三点下雨”比“未来会下雨”更值钱

**数学投影：** 预测精度直接影响有效因果信息的提取量。设 $I_{\mathrm{latent}}$ 为尚未被提取的潜在因果信息（bit），则

$$
I_{\mathrm{causal}} = \eta_D\, I_{\mathrm{latent}}, \qquad
I_{\mathrm{causal}}^{(\mathrm{coarse})} = \eta_D^{(\mathrm{season})} I_{\mathrm{latent}}^{(\mathrm{season})} \ll I_{\mathrm{causal}}^{(\mathrm{fine})} = \eta_D^{(\mathrm{hour})} I_{\mathrm{latent}}^{(\mathrm{hour})} \tag{Z-3.3}
$$

$\eta_D\in[0,1]$ 是解码效率（无量纲）。更高精度的预测允许系统在更细的粒度上区分环境状态——它把“季节”这一个格子切成了许多个“小时”格子，每个格子里的状态都可分辨。

**直觉等价物：** 知道“未来会下雨”只能让你决定种不种水稻；知道“明天下午三点下雨”能让你决定现在晒不晒被子、下午出不出去、要不要带伞。**精度每提升一个数量级，可操作的因果分支就成倍增长。** 注意是“成倍”，不是“指数级无上限”：分支数受 $E_{\mathrm{causal}}$ 预算约束，切得越细，维持模型的代价越高。

### 3.5 时间套利的双杠杆：长度赌战略，精度赌战术

**【假说】长度与精度对有效内生时间的贡献是乘法耦合，不是线性加和。** 下式只作**结构示意**：$\Lambda$（$\mathrm{s}^{1-\kappa_{\mathrm L}}$）与 $\kappa_{\mathrm{L}},\kappa_{\mathrm{G}}$ 三个系数在卷Ⅰ–Ⅳ中零次出现、也没有独立标定方法，**本式不用于数值计算**，可用的只是它的定性含义（长度与精度乘性耦合）。**失效条件**：若 $\langle T_{\mathrm{pred}}\rangle$ 对 $L_{\mathrm{pred}}$ 与 $G_{\mathrm{pred}}$ 的响应可加（交互项不显著），乘性形式在该域内失效。

$$
\langle T_{\mathrm{pred}}\rangle = \Lambda \cdot L_{\mathrm{pred}}^{\kappa_{\mathrm{L}}} \cdot 2^{\kappa_{\mathrm{G}} G_{\mathrm{pred}}} \tag{Z-3.4}
$$

系统规划能力对应的内部评估值为 $V_{\mathrm{c}}^{\mathrm{virt}} = I_{\mathrm{causal}}^{\mathrm{virt}}\langle T_{\mathrm{pred}}\rangle/E_{\mathrm{causal}}^{\mathrm{virt}}$：长度扩展状态空间边界，精度增加分辨率。

**直觉等价物：** 长度杠杆让你进入“时间套利”市场，精度杠杆让你在这个市场里**实际赚到钱**——没有精度，你知道未来有波动，却抓不住买卖点。战略决定你做不做，战术决定你做不做得成。

### 3.6 死亡的双重归零：当长度和精度同时熄灭

**数学投影：**

$$
\text{死亡：}\quad L_{\mathrm{pred}}\to 0 \ \land\ G_{\mathrm{pred}}\to 0 \ \Rightarrow\ I_{\mathrm{causal}}\to 0 \ \Rightarrow\ V_{\mathrm{c}}\to 0 \tag{Z-3.5}
$$

此时系统退化为纯被动相，$V_{\mathrm{obj}}=V_{\mathrm{s}}$。

**直觉等价物：** 死亡不是 $T_{\mathrm{struct}}$ 归零——尸体的 $T_{\mathrm{struct}}$ 还能持续很多年。死亡是 $T_{\mathrm{pred}}$ 的双重归零：**既看不到未来，也看不清当下**。昏迷的植物人 $L_{\mathrm{pred}}$ 可能趋近于零，但 $G_{\mathrm{pred}}$ 可能仍有残余；脑死亡者两者同时归零，即使心脏还在跳动，在这套记账口径下已经死亡。

同样要加边界：这是一个**功能性判据**，用于说明模型如何区分主动相与被动相，不是医学诊断标准，也不能用于临床或伦理判断。

### 3.7 认知占比不等于长度不等于精度：被误解的“远见”

**数学投影：** 认知通道在总存续势中的占比，称认知占比：

$$
\text{认知占比} = \frac{V_{\mathrm{c}}}{V_{\mathrm{obj}}} = \frac{V_{\mathrm{c}}}{V_{\mathrm{s}}+V_{\mathrm{c}}} \tag{Z-3.6}
$$

这个比值落在 $[0,1)$ 内，且只在 $V_{\mathrm{obj}}>0$ 时有定义。

**直觉等价物：** 认知占比高不等于看得远。种子的 $V_{\mathrm{c}}/V_{\mathrm{obj}}$ 很低，却押中了十年后的雨季；一个整天做预测的机构占比很高，可能只看得见下周。占比量的是“多少资源押在预测上”，不是“预测得多准”；种子的“长”是粗线条的长，水熊虫的“短”是细颗粒的短，两者在各自生存策略里的耦合效率才决定成败。

### 3.8 本章总结：时间管理的三个层级

四个层级排下来，是一条从“没有时间”到“双维导航”的路：石头 0 级；种子 1 级，粗粒度长波，靠物理兜底；水熊虫 2 级，细粒度短波，每次判断生死攸关；乌鸦和人是 3 级，战略与战术双优，风险是自指耦合越界导致幻觉。本章确定的是：时间要拆成五个记号加一个温度来读，内生视界是长度与精度的乘积。没确定的是：各层级的边界值，以及从 2 级跨到 3 级的门槛条件。

### 3.9 跨期决策：主权基金与散户的贴现率之战

**数学肉身：**

$$
r_{\mathrm{eff}} = \gamma_0 + \psi(\rho) + \frac{1}{T_{\mathrm{pred}}} \tag{Z-3.7}
$$

其中 $\psi(\rho)$ 为竞争附加贴现率（$\mathrm{s^{-1}}$，$\psi(0)=0$，随 $\rho$ 单调增大），$1/T_{\mathrm{pred}}$ 为视界项（$\mathrm{s^{-1}}$）。

**直觉等价物**：长期主义的价值积分。主权财富基金贴现率极低，看重百年积分；散户贴现率极高，只看明天。这是贴现率结构的结果：高竞争压缩视界，贴现率随之抬升；资源紧张的主体只顾眼前，是因为 $r_{\mathrm{eff}}$ 被环境强制抬高。

$I^{-}$ 冲击（战争、疫情）使 $T_{\mathrm{pred}}$ 坍缩到 $T_{\mathrm{min}}$ 附近，$r_{\mathrm{eff}}$ 趋近一个**有限**上界 $\gamma_0+\psi(\rho)+1/T_{\mathrm{min}}$：$T_{\mathrm{min}}$ 再小也是正的，所以贴现率不会发散。危机中人们变得短视，不是素质下降，是方程里的 $T_{\mathrm{pred}}$ 被压缩了；压缩会自己恢复，前提是冲击停止。

### 3.10 建造成本与沉没成本：为什么金字塔不是资产

**数学肉身：** 建造成本 $E_{\mathrm{build}}$ 是一次性的历史存量，不进入存续势的动力学公式，只通过锁死风险进入决策：

$$
\Pr(\text{锁死}) \propto R(E_{\mathrm{build}}) = 1 - \exp\!\left(-\frac{E_{\mathrm{build}}}{E_{\mathrm{topo}}}\right) \tag{Z-3.8}
$$

其中 $E_{\mathrm{topo}}$ 是当前生态位的特征拓扑能量（J）。这条式子是**示意性的**：它只说了“成本越高越容易锁死”这个方向，具体形状取决于锁死机制，不能当定量预测用。

**直觉等价物**：沉没成本不决定上限。金字塔的宏伟建造并未提升它作为遗迹的存续势上限——通道的稳态容量与一次性构建成本无关。创业融资的最优解是既融够钱开发、又控制破产风险：钱不够会死，钱太多也会死。

### 3.11 三温区与跨期存续：冬眠不是怂，是跨期决策

**数学肉身：** 认知投资回报率【候选推论】：

$$
\rho_I \equiv \frac{\alpha}{\gamma} = \frac{\partial \ln V/\partial \ln I_{\mathrm{net}}}{\partial \ln V/\partial \ln E_{\mathrm{eff}}} \tag{Z-3.9}
$$

其中 $\alpha$、$\gamma$ 是对数—对数斜率（无量纲），分别度量 $V$ 对信息与对成本的弹性。$\rho_I>1$ 时系统有主动认知相，$\rho_I<1$ 时只剩被动筛选。这个排序是经验假说，跨系统是否稳定另说；能确定的只是：在给定样本上算出 $\rho_I>1$，说明该样本的信息投入比成本投入更值钱。休眠需要跨期的存续势：跨期存续势 = 当期结构通道项 + 折扣后的未来因果期权的期望值。

**直觉等价物**：温度同时调制三个成本。高温时每比特擦除的能量下限更高（正比于 $T_{\mathrm{thermo}}$），低温时生化反应更慢（Arrhenius 型速率下降），高温时结构更容易被热涨落打散。所以没有“越热越好”或“越冷越好”，只有权衡：

| 温区 | 一句话 |
| :------------------------- | :--------------------------------- |
| 低温无源 | 冻结，等待 |
| 低温有源 | 用时间换信息：慢，但省 |
| 中温 | 又快又贵 |
| 高温 | 结构难维持，倾向节能 |

这一条标【候选推论】：四个温区的分界、以及弹性随温度的显式函数，本卷都未给出——“温度同时调制三个成本”是机制陈述，“调制曲线长什么样”仍是待标定问题。

***

## 第四章　黑暗森林与 V-Bug：高级玩家的失控手册

当解码器变得足够复杂，它开始产生幻觉。这套框架把这种现象称为“三重分裂”：客观势、虚拟势与价值目标的脱钩。它是高复杂度解码器的一个固有相态，修不掉——只要系统开始用内部模型指导行动，内部模型就有可能与现实分家。本章讲分家之后的事：怎么分、分多快、分到什么程度会致命。

### 4.1 三重分裂：一个灵魂裂成三个

**数学肉身：**

$$
V_{\mathrm{obj}} = \frac{I_{\mathrm{struct}}\,T_{\mathrm{struct}}}{E_{\mathrm{struct}}} + \frac{I_{\mathrm{causal}}\,T_{\mathrm{causal}}}{E_{\mathrm{causal}}} \tag{Z-4.1}
$$

$$
V^{\mathrm{virt}} = \frac{I_{\mathrm{struct}}^{\mathrm{virt}}\,T_{\mathrm{struct}}^{\mathrm{virt}}}{E_{\mathrm{struct}}^{\mathrm{virt}}} + \frac{I_{\mathrm{causal}}^{\mathrm{virt}}\,T_{\mathrm{pred}}^{\mathrm{virt}}}{E_{\mathrm{causal}}^{\mathrm{virt}}} \tag{Z-4.2}
$$

$$
V^{\mathrm{val}} = w_{\mathrm{s}}V_{\mathrm{s}}^{\mathrm{virt}} + w_{\mathrm{c}}V_{\mathrm{c}}^{\mathrm{virt}}, \qquad w_{\mathrm{s}}+w_{\mathrm{c}}=1 \tag{Z-4.3}
$$

式 (Z-4.2) 与式 (Z-4.1) 的差别不在分子上的字母，而在时间的取法：客观势用 $T_{\mathrm{causal}}$（效果实际持续多久），虚拟势用 $T_{\mathrm{pred}}^{\mathrm{virt}}$（系统自己以为能规划多久）。这一处替换，就是全部幻觉的来源。

**直觉等价物**：低阶物理结构中三者统一；$T_{\mathrm{pred}}$ 内生化之后，灵魂裂成三个。**客观存续势 $V_{\mathrm{obj}}$**（$\mathrm{bit\cdot s/J}$）是受热力学耗散约束的物理存量，不可欺骗，不可跨期借贷。**虚拟存续势 $V^{\mathrm{virt}}$**（$\mathrm{bit\cdot s/J}$）是内部模型的主观评估：$\chi$ 上升时 $I_{\mathrm{net}}$ 增长而 $T_{\mathrm{pred}}$ 按平方反比收缩。**价值存续势 $V^{\mathrm{val}}$**（$\mathrm{bit\cdot s/J}$）是系统实际优化的行为目标——它执行 $V^{\mathrm{virt}}$ 的指令，把能量导入维持虚拟存续势的正反馈循环。

**核心命题【命题】**：系统实际优化的不是 $V_{\mathrm{obj}}$，而是 $V^{\mathrm{val}}$。前提是行为界面由内部评估驱动；失效条件是行为界面被外部强制约束（硬性预算、外部审计、不可绕过的物理限位）——那时 $V^{\mathrm{val}}$ 会被拉回接近 $V_{\mathrm{obj}}$。当 $w_{\mathrm{s}}$ 与 $w_{\mathrm{c}}$ 极端偏置（如 $w_{\mathrm{s}}\to0$ 且 $\Delta_{\mathrm{VV}}\gg0$），系统可能从“追求客观存续”转变为“追求虚拟的、自毁性的目标”。

### 4.2 脱钩偏差：你离现实有多远？

**数学肉身：**

$$
\frac{\mathrm{d}\Delta_{\mathrm{VV}}}{\mathrm{d}t} = -\alpha_{\mathrm{L}}\,I_{\mathrm{net}}\,\Delta_{\mathrm{VV}} + \sigma \tag{Z-4.4}
$$

$$
\Delta_{\mathrm{VV}}(t) = \frac{\sigma}{\alpha_{\mathrm{L}}I_{\mathrm{net}}} + \left(\Delta_0 - \frac{\sigma}{\alpha_{\mathrm{L}}I_{\mathrm{net}}}\right)e^{-\alpha_{\mathrm{L}}I_{\mathrm{net}}t}, \qquad \Delta_{\mathrm{VV}}^{*} = \frac{\sigma}{\alpha_{\mathrm{L}}I_{\mathrm{net}}} \tag{Z-4.5}
$$

其中 $\alpha_{\mathrm{L}}$ 是学习率（$\mathrm{bit^{-1}\cdot s^{-1}}$，每比特信息带来的偏差收敛速率），$\sigma$ 是环境噪声强度（$\mathrm{bit/J}$，与 $\Delta_{\mathrm{VV}}$ 同量纲除以时间），$\Delta_0$ 是初值。能使 $\alpha_{\mathrm{L}}I_{\mathrm{net}}$ 成为 $\mathrm{s^{-1}}$ 的正是这组单位，不是自由选择。

**直觉等价物**：脱钩偏差 $\Delta_{\mathrm{VV}}=\lvert V^{\mathrm{virt}}-V_{\mathrm{obj}}\rvert$ 是导航仪的误差。它总是指数收敛到有界平衡值 $\Delta_{\mathrm{VV}}^{*}$，信息流越强，平衡偏差越小——但平衡值不为零：再好的学习器也无法完全克服环境噪声。以单位偏差为容限，临界信息量 $I_{\Delta,\mathrm{crit}}=\sigma/\alpha_{\mathrm{L}}$（bit）：$I_{\mathrm{net}}<I_{\Delta,\mathrm{crit}}$ 时平衡偏差超出容限，系统在认知上失去对环境的准确模型。成立条件是学习线性、噪声平稳、$I_{\mathrm{net}}$ 在观察窗内近似不变；三条任一不成立，收敛速度与平衡值都会变，但“偏差有界、信息越多偏差越小”的方向仍然成立。**能用的是方向，不是数值。**

### 4.3 短视失控态：燃烧自己照亮幻觉

**数学肉身：**

$$
V^{\mathrm{virt}}\uparrow \;\to\; r_{\mathrm{v}}^{\mathrm{virt}}\uparrow \;\to\; V^{\mathrm{val}}\ \text{被劫持} \;\to\; E_{\mathrm{eff}}\uparrow \;\to\; V_{\mathrm{obj}}\ \text{恶化} \;\to\; V_{\mathrm{obj}}\to 0 \tag{Z-4.6}
$$

**直觉等价物**：短视失控态是系统持续消耗客观存续势、以维持虚拟存续势极端值的动力学自噬过程。五个台阶：虚拟势膨胀（$\chi$ 越过分岔点，$I_{\mathrm{net}}$ 增长而 $T_{\mathrm{pred}}$ 收缩）；驱动率激增；价值目标被劫持（$E_{\mathrm{eff}}$ 被倾入自指循环）；客观势恶化（$T_{\mathrm{pred}}$ 趋近 $T_{\mathrm{min}}$）；物理存量承压（越过损伤触发阈值，累积存量开始被销毁）。

**关键的不对称性**：前四个台阶发生在潜在（评估）层，几乎不需要物理成本；最后一个台阶不可逆。系统用真实结构去换内部幻象，汇率还由它自己定。

式 (Z-4.6) 的末端含义是：$V_{\mathrm{obj}}\to0$ 是**链条走到尽头**的结果，不是“一越过分岔点就归零”。越过阈值之后的归宿与 1.4 的三种情形相同：可能归零，也可能落到较低的正平衡上带病活着。危险不在立刻致命，而在它把系统推进“看起来还在跑、实际在耗本金”的区间，那里的仪表盘是失准的。

### 4.4 猜疑链：为什么越聪明的系统越不信任？

**数学肉身：** 用的仍是内生风险贴现率（式 (Z-3.7)），此处不重排。

**直觉等价物**：黑暗森林的预期坍缩。只要存在“他者是失控体”的概率（$p>0$），$T_{\mathrm{pred}}$ 就被压缩，$\psi(\rho)$ 随防御性耗散抬高，$r_{\mathrm{eff}}>\gamma_0$，系统失去躺平的资格。自己是失控体，就无法证明别人不是——猜疑链是给定支付结构下的均衡：只要对方构成威胁的概率不为零、且防御成本低于被突袭的损失，维持高耗散防御就是理性的。越聪明的系统越焦虑，也在这里：解码器越好，越能模拟“别人可能是威胁”的未来，从而压缩自己的 $T_{\mathrm{pred}}$。

**这里要标条件。** 猜疑链成立需要三条：对方能力足以造成不可逆损失；防御可观测、可执行；双方没有可执行的共同约束。任一条被打破——出现可验证的互不侵犯协议，或防御成本高到不划算——猜疑链就退化。把它讲成“只要有两个智能体就必然互相猜疑”，是把条件均衡说成了宿命。

### 4.5 V-Bug：一个强脱钩系统的命名【假说】

**数学肉身：**

$$
\Delta_{\mathrm{VV}}\gg 0, \quad \chi>\chi_{\mathrm{c}} \;\Rightarrow\; \rho\to 1 \tag{Z-4.7}
$$

**直觉等价物**：V-Bug 是这套框架对“强脱钩系统”的命名。在假设性的极限情形下，严重脱钩且自指增益极强的智能体，其极高耗散可能把整个生态位的竞争压力拉满。

$\rho\to1$ 属于强脱钩猜想，标【假说】，需要在具体的多主体博弈模型里才能被证明或否证。现实中可观察的版本要弱得多：一个高耗散主体只会**局部**抬高竞争压力，幅度取决于它占该生态位自由能通量的份额——份额不到一定比例，$\rho$ 的显著上升就不会发生。

### 4.6 N 体博弈与强迫欠饱和：没人敢先停手

**数学肉身：** 一个示意性的净增长模型。设主体 $i$ 的净增长率为

$$
F_i = r_{\mathrm{v},i} - \gamma_0 - \psi(\rho)\frac{\langle r_{\mathrm{v}}\rangle}{r_{\mathrm{v},i}} \tag{Z-4.8}
$$

对称均衡（$r_{\mathrm{v},i}=\langle r_{\mathrm{v}}\rangle$，$F_i=0$）满足

$$
r_{\mathrm{v,eq}} = \gamma_0 + \psi(\rho), \qquad \frac{\partial F_i}{\partial r_{\mathrm{v},i}} = 1 + \psi(\rho)\frac{\langle r_{\mathrm{v}}\rangle}{r_{\mathrm{v},i}^{2}} > 0 \tag{Z-4.9}
$$

**直觉等价物**：剧场效应的流场。你的增长率不仅取决于自己，还被同行平均增长率和竞争强度惩罚。只要 $\psi(\rho)>0$，均衡驱动力必大于折旧率；偏导恒正，谁敢单方面降耗散，谁的净增长就断崖式下跌。没人敢先停手。

式 (Z-4.8) 是**示意性**的增长率模型，不是从第一原理推出来的。它抓的机制是——竞争惩罚作用在增长率上，而不是作用在存量上——足以解释“越卷越不敢停”，但不构成对囚徒困境的证明。真实的多方博弈里还有合作、声誉、退出、制度约束，都会改变均衡。最值得记住的一点：惩罚落在 $r_{\mathrm{v}}$ 上，不落在 $V$ 上；内卷摧毁的是**增量的分配权**。

### 4.7 外部冲击：黑天鹅的泊松跳跃

**直觉等价物**：外星接触（$\rho$ 跳跃）、核战争（$E_{\mathrm{total}}$ 被截断）、大流行病（$T_{\mathrm{pred}}$ 坍缩）。无需新变量，只需把冲击建模为参数向量（$E_{\mathrm{total}}$、$I_{\max}(D)$、$T_{\mathrm{struct}}^{\max}$、$\rho$、$\Delta_{\mathrm{VV}}$）上的泊松跳跃。五项里 $I_{\max}(D)$ 与 $T_{\mathrm{struct}}^{\max}$ 一旦跳变就很难恢复（重建要付 $E_{\mathrm{build}}$），$\rho$ 与 $\Delta_{\mathrm{VV}}$ 通常会自行回归——所以致命的是**打中的是哪一项**。

### 4.8 元解码器：能停战的通用语言

**数学肉身：**

$$
V_{i}(D_{\mathrm{meta}}) \ge V_{i}(D_{i}^{\mathrm{deviate}}) - C_{i}^{\mathrm{punish}} \tag{Z-4.10}
$$

其中 $C_{i}^{\mathrm{punish}}$ 是偏离后受联合惩罚的预期存续势损失（$\mathrm{bit\cdot s/J}$）。

**直觉等价物**：如何跳出猜疑链？构建**元解码器**，一种跨主体的共享抽象层。数学、物理定律、热力学第二定律本身就是元解码器，因为它们是所有 $D$ 都必须服从的约束。元解码器下，共享的 $I_{\mathrm{orig}}^{\mathrm{meta}}$ 成为共同的 $I^{+}$，降低跨主体的 $\Delta_{\mathrm{VV}}$，使合作从囚徒困境退化为协调博弈。

**等级说明【命题】**。式 (Z-4.10) 常被写成“当且仅当”的形式，那是不对的：它只是**对单个偏离方案的收益检验**，通过它只能说明“这一个偏离不划算”，不能说明“所有偏离都不划算”，更不能说明惩罚一定可执行。要抬成均衡结论，至少得补三件东西：完整的可行偏离集合、惩罚的可执行性条件、每个参与者的个体收益函数。三件缺一件，它就只能算**治理设计建议**。

### 4.9 征服博弈：零和份额，负和账单【命题】

以前的写法是“零和博弈的热力学负和定理”，还配一句“战争没有赢家”。这两句话放在一起是矛盾的：如果真是零和，双方的存续势变化就该一正一负、加起来是零；可公式又给双方的分母都加了正的冲突成本，算出双方同时下降、加起来是负的。**零和与“双方都亏”不能同时为真**——矛盾不在推导，在概念：把“份额怎么分”和“成本谁来付”当成了同一层。正确的做法是把存续势的变化拆成两个可加的分量：

$$
\Delta V_{i} = \Delta V_{i}^{\mathrm{share}} + \Delta V_{i}^{\mathrm{cost}} \tag{Z-4.11}
$$

**份额层是零和的。** 在资源总量固定、份额转移是纯再分配、双方计量口径一致这三个前提下，

$$
\Delta V_{A}^{\mathrm{share}} = -\Delta V_{B}^{\mathrm{share}} \quad\Longrightarrow\quad \sum_{i\in\{A,B\}}\Delta V_{i}^{\mathrm{share}} = 0
$$

这是“零和”一词的合法位置。它是一层**账面**：一张饼怎么切。

**成本层是负和的。** 冲突本身要烧能量：军备、情报、动员、占领区的治安维持。这些消耗不转化为任何一方的份额，直接耗散掉。设冲突使双方的等效成本各增加 $\Delta E_{\mathrm{conflict},i}>0$（J），在 $I_{\mathrm{net}}$ 与 $T_{\mathrm{pred}}$ 于冲突期内近似不变的条件下，

$$
\Delta V_{i}^{\mathrm{cost}} = V_{i}^{0}\left(\frac{E_{\mathrm{eff},i}}{E_{\mathrm{eff},i}+\Delta E_{\mathrm{conflict},i}} - 1\right) = -V_{i}^{0}\,\frac{\Delta E_{\mathrm{conflict},i}}{E_{\mathrm{eff},i}+\Delta E_{\mathrm{conflict},i}} < 0
$$

对双方求和：

$$
\sum_{i\in\{A,B\}}\left(V_{i}^{1}-V_{i}^{0}\right) = -\sum_{i\in\{A,B\}}V_{i}^{0}\,\frac{\Delta E_{\mathrm{conflict},i}}{E_{\mathrm{eff},i}+\Delta E_{\mathrm{conflict},i}} < 0 \tag{Z-4.12}
$$

式 (Z-4.12) 只用了一个假设：$\Delta E_{\mathrm{conflict},i}>0$，即冲突对双方都有成本。这个假设极难违反——持续对抗总要投入资源，即使投入极不对称，也没有哪一方的成本严格为零。

**合并起来**：$\sum_i\Delta V_i = \underbrace{0}_{\text{份额层}} + \underbrace{<0}_{\text{成本层}} < 0$。于是“$\Delta V_A=-\Delta V_B$”这个纯零和关系，**只在冲突成本趋零的极限下成立**：

$$
\lim_{\Delta E_{\mathrm{conflict}}\to 0}\left(\Delta V_{A}+\Delta V_{B}\right) = 0 \tag{Z-4.13}
$$

而这个极限与“双方都承担成本”不相容：成本趋零意味着对抗趋零，对抗趋零意味着这已经不是征服博弈了。所以纯零和只能作为极限参考。

**长期军备竞赛的写法。** 定义竞争强度 $\Upsilon=\Delta E_{\mathrm{conflict}}/E_{\mathrm{eff}}^{\mathrm{base}}$（无量纲），则单一主体的存续势近似为 $V=V_{0}/(1+\Upsilon)$。$\Upsilon$ 越大，$V$ 越低；越过域内标定的阈值，系统进入崩溃区。

**跨主体求和的前提。** 式 (Z-4.12) 含跨主体求和，须先满足四条核算前提：**复合边界**（只纳入直接参与者）、**持有者集合**（双人或 $n$ 人，中途改范围则两个结论都失效）、**同窗条件**（双方成本同窗计，征服者的成本在前线且即时，被征服者的成本滞后数代）、**去重规则**（共同成本按实际支付方记账）。四条不能同时建立时只作定性比较：可以说双方总存续势下降，不能说下降了多少。

**直觉等价物**：战争是一张**双层账单**。上层是份额，切得干净，一方的所得就是另一方的所失；下层是成本，切不干净，两边都在往火里扔钱，扔进去的钱不归任何人。“战争没有赢家”作为**经验概括**大体成立——它描述的是下层账单通常大于上层收益。但它不是定理，例外是有的：**一方在份额层大赚、同时把成本几乎全部转嫁给对方**（战场在别人家里、账单记在别人账上、收益回流自己手里），它可能是净赢家。定理能说的只有一句：只要双方都在付成本，两边加起来就是亏的；谁亏得多，取决于份额层怎么分。

### 4.10 合作超加性与视界—合作条件：婚姻的本质

**数学肉身：** 合作的前提是时间视界足够长。先定义单轮支付：$\Pi_{\mathrm{coop},i}$、$\Pi_{\mathrm{def},i}$、$\Pi_{\mathrm{pun},i}$ 分别是合作、背叛、互相惩罚三种情形下，一个**共同核算窗**内的单轮支付，本身不含 $T_{\mathrm{pred}}$。折现因子由视界生成：$\delta_{\mathrm{disc}}=e^{-t_{\mathrm{dec}}/T_{\mathrm{pred}}}$，$t_{\mathrm{dec}}$ 为决策周期（s）。冷酷触发策略下，合作可持续的条件是

$$
\frac{\Pi_{\mathrm{coop},i}}{1-\delta_{\mathrm{disc}}} \ge \Pi_{\mathrm{def},i} + \frac{\delta_{\mathrm{disc}}\,\Pi_{\mathrm{pun},i}}{1-\delta_{\mathrm{disc}}} \tag{Z-4.14}
$$

解出临界视界：

$$
T_{\mathrm{pred}} > T_{\mathrm{crit}} = \frac{t_{\mathrm{dec}}}{\ln\dfrac{\Pi_{\mathrm{def},i}-\Pi_{\mathrm{pun},i}}{\Pi_{\mathrm{def},i}-\Pi_{\mathrm{coop},i}}} \tag{Z-4.15}
$$

解有意义的前提是 **$\Pi_{\mathrm{def},i}>\Pi_{\mathrm{coop},i}>\Pi_{\mathrm{pun},i}$**（背叛有诱惑、合作优于互相惩罚）。**三条缺一不可**：若只写前两条（$\Pi_{\mathrm{def}}>\Pi_{\mathrm{coop}}$ 且 $\Pi_{\mathrm{pun}}<\Pi_{\mathrm{def}}$），漏掉 $\Pi_{\mathrm{coop}}>\Pi_{\mathrm{pun}}$，则 $\ln[(Π_{\mathrm{def}}-Π_{\mathrm{pun}})/(Π_{\mathrm{def}}-Π_{\mathrm{coop}})]\le0$，(Z-4.15) 的分母非正，$T_{\mathrm{crit}}$ 无定义——**此时任何有限视界下冷酷触发都不构成均衡**，而不是“视界不够长”。

**直觉等价物**：合作通过共享 $I_{\mathrm{orig}}$ 与 $T_{\mathrm{pred}}$，降低各自的 $E_{\mathrm{causal}}$，可能产生超加性（$1+1>2$）。**条件是双方信息互补、能耗可分担、且合并本身不引入新的协调成本。** 三条缺一条，超加性就可能变成“$1+1<2$”——两个组织合并后开会时间翻倍，是最常见的反例。

***

## 第五章　热力学极限：宇宙的预算表

前四章讲的是这套框架在“可观测运作范围”内的叙事对应。本章换一个维度：**边界条件**。当系统逼近物理极限时，框架的适用域终点在哪里？

先把一个说法改掉：这些极限不是“参数趋极值时的必然收敛点”。物理极限本身是硬约束；但“某个具体系统会撞上哪一条、什么时候撞、撞上之后怎样”，都依赖它的架构、工作负荷与散热条件。所以本章统一写成：在所列条件下，那条不等式成立；越过它，会发生什么，取决于系统有没有降速、外移、重构的余地。

### 5.1 朗道尔税：每一笔擦除都要交的热力学增值税

**数学肉身：** 先把单位写清楚。**朗道尔原理（Landauer, 1961）** 给出的是**每比特**的量：

$$
E_{\mathrm{L,bit}} = k_B T_{\mathrm{thermo}}\ln 2 \quad (\mathrm{J/bit}) \tag{Z-5.1}
$$

它必须乘上“擦掉了多少比特”，才得到焦耳：

$$
E_{\mathrm{erase}} \ge E_{\mathrm{L,bit}}\cdot I_{\mathrm{erased}} = k_B T_{\mathrm{thermo}}\ln 2 \cdot I_{\mathrm{erased}} \quad (\mathrm{J}) \tag{Z-5.2}
$$

其中 $I_{\mathrm{erased}}$ 是逻辑不可逆擦除的比特数（bit）。由此得到的存续势上界，在纯信息处理极限下（$E_{\mathrm{struct}}\to0$，$I_{\mathrm{causal}}\le I_{\mathrm{erased}}$）成立：

$$
V \le \frac{I_{\mathrm{causal}}\,T_{\mathrm{causal}}}{E_{\mathrm{L,bit}}\,I_{\mathrm{causal}}} = \frac{T_{\mathrm{causal}}}{k_B T_{\mathrm{thermo}}\ln 2} \quad (\mathrm{bit\cdot s/J}) \tag{Z-5.3}
$$

量纲检查：分子是 s，分母是 J/bit，商是 $\mathrm{bit\cdot s/J}$，与 $V$ 同量纲。这一步不能省——把 bit 因子漏在分母外，读起来就像“$V$ 的上界只是一个时间”，那是把量纲混了。

**直觉等价物**：任何物理计算每擦除 1 bit，至少耗散 $k_B T_{\mathrm{thermo}}\ln2$ 的热量。这不是工程限制，而是热力学定律。这套框架称之为“**朗道尔税**”：每一笔擦除都要交的增值税。

三点必须补充。

**其一，税基是“擦除”，不是“处理”。** 可逆的逻辑操作理论上不必付这笔税；只有把信息真正抹掉——合并两个不同的状态到一个状态——才付。所以“每比特思维都要交税”是**比喻**，严格版本是“每比特不可逆擦除都要交税”。两者之间隔着一个必须声明的映射：每处理一比特，实际发生了几次不可逆擦除。

**其二，映射系数必须自己报。** 记这个映射为 $\beta_{\mathrm{erase}}$（无量纲，擦除比特数／处理比特数），产热功率下界才能写成

$$
\dot Q_{\mathrm{heat}} \ge E_{\mathrm{L,bit}}\cdot \dot I_{\mathrm{erase}} = E_{\mathrm{L,bit}}\cdot \beta_{\mathrm{erase}}\cdot \dot I_{\mathrm{proc}} \quad (\mathrm{W}) \tag{Z-5.4}
$$

$\beta_{\mathrm{erase}}$ 不报，式 (Z-5.4) 就不能代入任何具体数字。工程上那些“每比特能耗”数字，全是某个特定架构、特定比特界定下的标定值，不是普适常数。

**其三，温度是本地温度。** $T_{\mathrm{thermo}}$ 取擦除发生处的温度，不是环境平均温度，也不是宇宙微波背景温度。芯片结温与室温可以差几十开，这一项直接线性影响税额。

**结论的形状**：系统接近纯信息处理极限时，存续势上界仅由因果作用时间与本地温度决定，**与信息率无关**——这是式 (Z-5.3) 最反直觉的地方。算力再高，面前也有一道硬天花板；但天花板的高度，由“你能让效果持续多久”和“你在多冷的地方算”共同决定。

### 5.2 布雷默曼天花板：质量即算力，算力即命运

**数学肉身：** 这里必须先分清两种“率”。物理界限给出的是**逻辑操作率**的上界：

$$
\dot I_{\mathrm{op}} \le \frac{2m_D c^{2}}{\pi\hbar} \quad (\mathrm{ops/s}) \tag{Z-5.5}
$$

其中 $m_D$ 是解码器的物理质量（kg），$\hbar$ 是约化普朗克常数，$c$ 是光速。对应的“每单位质量可维持的信息量”写成

$$
\frac{I_{\mathrm{net}}}{m_D} \le \frac{1}{\beta_{\mathrm{op}}}\cdot\frac{2c^{2}\tau_{\mathrm{proc}}}{\pi\hbar} \quad (\mathrm{bit/kg})
$$

其中 $\tau_{\mathrm{proc}}$ 是特征处理周期（s）。两个式子的右边原本都是**操作计数**，不是比特计数；不除 $\beta_{\mathrm{op}}$，两边就不是同一个量，不能直接比。

**关键的一步，不能跳。** 操作率要变成比特率，必须经过一个声明过的“操作—有效信息”映射：

$$
\dot I_{\mathrm{bit}} = \frac{\dot I_{\mathrm{op}}}{\beta_{\mathrm{op}}}, \qquad \beta_{\mathrm{op}}\ge 1 \tag{Z-5.6}
$$

$\beta_{\mathrm{op}}$ 是“平均多少次逻辑操作才产出一个有效信息比特”（无量纲），因任务而异：查表类任务可以很小，需要大量迭代的优化任务可以很大。**在 $\beta_{\mathrm{op}}$ 未标定之前，不得把 $\dot I_{\mathrm{net}}\le\dot I_{\mathrm{Brem}}$ 直接写出来**——那是把操作计数当成了比特计数。正确的写法是：

$$
\dot I_{\mathrm{net}} \le \frac{1}{\beta_{\mathrm{op}}}\cdot\frac{2m_D c^{2}}{\pi\hbar}, \qquad \beta_{\mathrm{op}}\ \text{须由该架构的任务谱标定} \tag{Z-5.7}
$$

**直觉等价物**：质量为 $m_D$ 的系统每秒最多做 $2m_Dc^{2}/(\pi\hbar)$ 次逻辑操作（Margolus–Levitin 界 $2E/(\pi\hbar)$；Bremermann 界是 $m_Dc^{2}/h$，常数不同，不可混用）。这是相对论与量子力学的联合约束，它管“操作次数”，不管“这些操作值多少信息”。

### 5.3 计算的热力学极限：智能体的保质期

**数学肉身：** 联立朗道尔下界与操作率上界，在**固定工作负荷**（吞吐量 $\dot I_{\mathrm{bit}}$ 保持不变）的条件下，可实现的存续时间满足

$$
T_{\mathrm{struct}}^{\mathrm{realizable}} \le \frac{E_{\max}}{E_{\mathrm{L,bit}}\,\beta_{\mathrm{erase}}\,\dot I_{\mathrm{bit}} + \dot E_{\mathrm{maintain}}} \quad (\mathrm{s}) \tag{Z-5.8}
$$

量纲检查：分子 J，分母 W，商 s。$\dot E_{\mathrm{maintain}}$ 是维持结构的功率（W）。维持成本可忽略、且 $\beta_{\mathrm{erase}}=1$ 时，上限退化为 $E_{\max}/(E_{\mathrm{L,bit}}\dot I_{\mathrm{bit}})$。把 $m_D$ 换成维持 $I_{\min}$ 位信息所需的最小物理质量 $m_{\min}\approx I_{\min}m_{\mathrm{bit}}$，上限随之提高，但仍有界。

**适用范围必须写清。** 它成立的前提是**工作负荷固定**：系统必须持续以 $\dot I_{\mathrm{bit}}$ 的吞吐量运行。如果系统可以降速，结论就变——把 $\dot I_{\mathrm{bit}}$ 降到原来的十分之一，同样的能量可以撑十倍时间。所以式 (Z-5.8) 给出的是**在给定吞吐量下**的寿命上界。系统通过降速换寿命，是最古老也最有效的延寿策略：从细菌的休眠孢子到数据中心的降频运行，用的是同一条算术。

**直觉等价物**：就像食品包装上的保质期标签，宇宙给智能体也贴了一个——但标签上还有一行小字：**“按当前食用速度计算”**。吃慢一点，保质期就长一点；这不是作弊，这是这条公式本来就说的事。

### 5.4 虚拟宇宙不可能：为什么我们不能模拟一切

**数学肉身：**

$$
\dot E_{\mathrm{causal}} \ge E_{\mathrm{L,bit}}\,\beta_{\mathrm{erase}}\,\dot I_{\mathrm{bit}} \tag{Z-5.9}
$$

**直觉等价物**：模拟一个完整宇宙（$m_D\approx10^{53}\ \mathrm{kg}$），若假定所有逻辑操作都对应不可逆擦除（$\beta_{\mathrm{op}}=\beta_{\mathrm{erase}}=1$，最宽松的算法），操作率上界约 $5.4\times10^{103}\ \mathrm{ops/s}$；取 $T_{\mathrm{thermo}}$ 为宇宙微波背景温度（约 2.7 K），$E_{\mathrm{L,bit}}\approx2.6\times10^{-23}\ \mathrm{J/bit}$，所需最小瞬时功率约 $1.4\times10^{81}\ \mathrm{W}$ 量级。而可观测宇宙所有恒星的总光度约 $10^{49}\ \mathrm{W}$ 量级。差距约 32 个数量级。

所以方向是稳的：**在已知物理定律与已知能量预算下，逐比特模拟一个完整宇宙不可行。** 但它是“不可行”，不是“不可能”——它依赖“模拟必须逐比特进行”这个前提。若存在不逐比特的模拟方式（例如利用被模拟系统本身的物理过程做“自然计算”），这条估算就不适用。这也是它标【命题】而不是【定理】的原因。

### 5.5 信息窒息流形：当系统被物理法则强制断氧

**数学肉身：**

$$
\mathcal{M}_{\mathrm{choke}}:\quad E_{\mathrm{L,bit}}\,\beta_{\mathrm{erase}}\,\dot I_{\mathrm{Brem}} > \dot E_{\max} \tag{Z-5.10}
$$

其中 $\dot E_{\max}$ 是系统的最大可持续散热功率（W）。两边同为 W，可以直接比较。

**但“直接坠落至 $I_{\min}$”这个说法要改。** 系统手上有三张牌，按代价从低到高：**降速**（把 $\dot I_{\mathrm{bit}}$ 降下来，让左边小于右边）、**外移**（把热搬到别处，抬高 $\dot E_{\max}$）、**重构**（换架构，让 $\beta_{\mathrm{erase}}$ 变小）。只有三张牌都打不出去——工作负荷被外部钉死、散热无处可去、架构无法更换——系统才真的被强制断氧，一路掉到 $I_{\min}$。所以窒息流形描述的是“**退路全被封死**”这个特定状态。判断一个系统是否进入窒息，要问的是“它还能不能降速”。

### 5.6 散热壳层：为什么文明越发达，基础设施越笨重

**数学肉身：** 先算**可承载比特数**，不是密度。给定可用于信息处理的总能量尺度 $E_{\max}$（J）与本地温度 $T_{\mathrm{thermo}}$（K），朗道尔成本下可承载的比特数上界为

$$
N_{\mathrm{bit}} \le \frac{E_{\max}}{E_{\mathrm{L,bit}}} = \frac{E_{\max}}{k_B T_{\mathrm{thermo}}\ln 2} \quad (\mathrm{bit}) \tag{Z-5.11}
$$

**信息密度**是它除以体积：

$$
n_{\mathrm{bit}} = \frac{N_{\mathrm{bit}}}{V_{\mathrm{vol}}} \le \frac{E_{\max}}{k_B T_{\mathrm{thermo}}\ln 2\cdot V_{\mathrm{vol}}} \quad (\mathrm{bit/m^{3}}) \tag{Z-5.12}
$$

式 (Z-5.11) 的右边不能直接叫“信息密度”：能量除以每比特能量得到的是比特数，不是每立方米的比特数。漏掉除以体积这一步，量纲上说不通；“密度”这个词一旦用错，后面所有关于“越发达越密集”的推论都会跟着错。

再看外壳与核心的能量比：

$$
\Sigma = \frac{E_{\mathrm{struct}}^{(\mathrm{shell})}}{E_{\mathrm{causal}}^{(\mathrm{core})}} = \frac{E_{\mathrm{barrier}}^{(\mathrm{support})}+E_{\mathrm{survival}}^{(\mathrm{cooling})}}{E_{\mathrm{causal}}} \tag{Z-5.13}
$$

$\Sigma$ **不构成无条件下界**。由“散热需要表面积”到“外壳能量存在正下界”，中间还隔着外壳厚度、材料密度、散热方式（传导／对流／辐射）、核心与外壳的规模比例。这些都没给定时，只能得到方向性判断，不能得到严格界限。**只有在壳层厚度有下界 $L_{\min}>0$ 时**，才给出与功率、尺度无关的弱下界 $\Sigma\ge\Sigma_{\min}$（卷Ⅲ 命题 8.12）；它是下界，不是对实际占比的预测。

所以式 (Z-5.13) 的正确读法是**【假说】（经验趋势）**：**在给定的几何、材料与散热方式下，随着核心功率密度上升，维持可接受温度所需的外壳能量占比 $\Sigma$ 趋于上升。** 这与卷Ⅲ 命题 8.12 不冲突：该命题给的是与功率无关的弱下界 $\Sigma_{\min}$，“随密度上升”是工程观察到的趋势，不是从导热模型推出来的。**口径**：本卷 (Z-5.13) 与附录 B 用**能量比**；卷Ⅲ (III-8.38) 的 $\Sigma=E_{\mathrm{shell}}/E_{\mathrm{core}}$ 是材料储能与运行能耗之比；另有“质量比”写法与之并存——三套口径量纲相同、含义不同，不可跨处比较。前提是散热主要靠外壳表面向环境排热；若改为液冷闭环、热泵、或把废热直接抛到外部（例如向太空辐射），这条趋势会被大幅削弱。

**直觉等价物**：2020 年前后，人类建造物体的总质量已超过全球生物量，绝大部分是混凝土、沥青与金属。这些“低功率密度”物质不是冗余，而是信息处理核心的散热壳与支撑护甲：文明越发达，核心越热，需要的“笨重”基础设施通常越多。但这是**常见形态**，不是必然形态——CPU 需要散热器和主板，文明需要公路、电网和数据中心，这些存在的理由是“当前技术路径下成本最低”，不是“物理定律不允许别的做法”。

***

## 第六章　规范化表述

本章把核心结论提炼为七条可记忆的**规范化表述**：被约定俗成的叙事形式，每条附证据等级、成立条件与典型实例。它们不扩展任何形式化条目的适用范围，也不替代任何推导；与形式化条目冲突时，以形式化条目为准。每条的格式固定：**等级与条件**、**叙事表述**、**实例**。等级放在最前面，因为它决定了这句话能被推多远。

**元表述**：持久结构在物理约束下，通过把耗散性能量转化为可预测信息来提升存续势。（*Persistent structures increase survival potential by converting dissipative energy into predictive information under physical constraints.*）

七条均从此元表述展开。元表述本身不是定理，只是一个**组织原则**：规定了这七条共同关心的对象（耗散、信息、时间、能量预算），不构成对任何具体系统的预测。

### CS-C1：编译优先（Compile-First）【命题】

**成立条件**：任务重复频次足够高，使编译成本的回收期短于观察窗；编译前后的行为可用同一目标、同一观察窗比较；无切换成本，或切换成本已计入 $E_{\mathrm{build}}$。**失效条件**：一次性任务；能量预算近似无限；任务分布漂移快于编译回收期。

**叙事表述**：重复任务最终会被编译为离线结构——不是“都会”，是“在回收期算得过来的情况下会被”。

**实例**：教育（反复练习形成肌肉记忆）｜AI（从在线推理转向离线缓存）｜组织管理（重复事务形成标准化流程）｜生物（先天行为替代后天试错）。

### CS-C2：压缩终局（Compression Finality）【假说】

**成立条件**：训练数据分布固定、解码器容量有限、且压缩带来的维护成本下降大于信息损失带来的收益下降。**失效条件**：开放演化系统；分布持续漂移的环境；压缩本身成为瓶颈（过度压缩导致泛化崩掉）。标【假说】的理由：这条陈述没有形式化推导，“最终会压缩”是从信息瓶颈类模型的直觉外推，缺一个明确的动力学方程。

**叙事表述**：固定解码器容量下，智能系统倾向于把经验压缩为结构化信息。

**实例**：语言（语法固化）｜艺术（后期作品趋于风格化）｜AI（过拟合）｜科学（范式固化）。

### CS-T1：热壳外包（Thermal Shell Outsourcing）【命题】

**成立条件**：环境边界固定；$\dot I_{\mathrm{net}}$ 长期为正；系统内部无法把废热完全回收（受第二定律约束）。**失效条件**：耗散可完全回收的封闭系统；热力学孤立系；环境边界可扩张（此时“外包”变成“搬家”，命题仍需成立但结论的形式变了）。

**叙事表述**：持续增长的信息系统会把耗散转移至外部。

**实例**：城市（工业废弃物排放）｜AI（训练计算迁移到数据中心）｜文明（能源进口）｜生物（代谢废物排放）。

### CS-T2：热力学天花板（Thermodynamic Ceiling）【命题】

**成立条件**：由电磁相互作用主导的物理计算系统；给定环境温度与可用质量；擦除映射 $\beta_{\mathrm{erase}}$ 已标定。**失效条件**：可逆计算（税基变小）；量子相干计算（成本结构不同）；尚未发现的非热力学计算范式。

**叙事表述**：给定环境温度与物理质量，智能规模存在热力学上限。

**实例**：AI（模型参数不能无限增长）｜生物（大脑代谢受氧气供给约束）｜文明（受恒星辐射通量限制）｜数据中心（散热限制计算密度）。

### CS-D1：失配成长（Mismatch-Driven Growth）【候选推论】

**母命题**：解码器漂移方程 $D_{n+1}=D_n+\varepsilon_{\mathrm{lr}}(\nabla_{\Theta}I_{\mathrm{net}}-k_D\,\frac{I_0}{E_0}\,\nabla_{\Theta}E_{\mathrm{causal}})$。**附加条件**：系统具有认知解码器 $D_{\mathrm{cog}}$，且 $\nabla_{\Theta}I_{\mathrm{net}}>0$；完全匹配稳态下 $\nabla_{\Theta}I_{\mathrm{net}}=0$，演化停滞。**可测后果**：人为制造适度失配应提升后续学习速率；失配过大应导致解码器崩溃而非成长。

**叙事表述**：解码器通过与环境失配来触发结构性成长。

**实例**：科学革命（实验异常驱动新范式）｜AI（分布外数据迫使模型更新）｜教育（略高于当前水平的挑战驱动学习）｜组织（外部压力驱动组织重构）。

### CS-B1：建造成本壁垒（Construction Cost Barrier）【命题】

**成立条件**：$E_{\mathrm{build}}<E_{\mathrm{available}}$ 是**必要条件**，不是充分条件——还需要杠杆条件 $L_{\mathrm{lev}}>L_{\mathrm{lev,min}}$ 与信号可用。**失效条件**：资源近似无限；外部注入能量；建造成本可从未来收益中借贷（此时约束变成跨期预算约束，形式不同）。

**叙事表述**：拓扑跃迁是否发生，取决于建造成本是否低于可用自由能预算——低于预算只是拿到入场券，不保证会进场。

**实例**：文明（大科学装置超出单国预算）｜AI（架构转型的切换成本）｜企业（数字化转型的投资门槛）｜生物（复杂器官演化的能量代价）。

### CS-H1：视界先坍缩（Horizon Collapse Precedence）【假说】

**成立条件**：系统具有认知解码器且其行为由内部评估驱动；存在可观测的视界收缩代理（如规划周期缩短、长期项目取消率上升）。**失效条件**：被动物理型持久结构；视界被外部制度钉死（例如法定的长期预算）；崩溃由外部冲击直接触发，与视界无关。标【假说】的理由：$\chi>\chi_{\mathrm{c}}$ 是模型内的分岔条件，不是现实判据；“先于”是时序断言，需要纵向数据才能检验。

**叙事表述**：具有认知解码器的系统在走向崩溃之前，其内生视界的收缩往往先于物理耗散的失控——“往往”，不是“必然”。

**实例**：企业（只看季度利润，放弃五年规划）｜AI（优化即时奖励而忽视长期后果）｜文明（选举周期压制长期战略）｜个人（压力状态下无法长期规划）。

***

## 第七章　命题的寓言：把条件句讲成故事

这一章把那些带条件的结论翻译成能讲给朋友听的故事。每节四段：**等级与条件**、**精简陈述**、**故事版**、**这条故事推不到哪里**。

这一章不叫“定理的寓言”：那些条目里，有的是【命题】（前提还没标定完），有的是【假说】（连形式化陈述都还没有），统一挂“定理”的牌子会让读者误以为推论已经闭合。第四段专门堵最常见的过度引申——故事讲完，人会忍不住往前再走一步，那一步通常就掉沟里了。

### 7.1 编译优先：学霸为什么先想通再刷题（条件性的 bang-bang 结构，【命题】）

**等级与条件。** 结论是“回收期短于视界时，最优策略是先全力编译、后全力执行”，依赖两条假设：目标泛函对控制变量线性（最优点落在边界上），切换没有成本。“半学半做”常见，恰恰因为切换有成本。

**精简陈述。** 设任务重复频率 $f_{\mathrm{task}}$（$\mathrm{s^{-1}}$）、每比特编译成本 $\varepsilon_{\mathrm{c}}$（$\mathrm{J/bit}$）、单次编译处理的比特数 $\Delta I_{\mathrm{orig}}$（bit），编译回收期为

$$
T_{\mathrm{pay}} = \frac{E_{\mathrm{build}}}{\varepsilon_{\mathrm{c}}\,\Delta I_{\mathrm{orig}}\,f_{\mathrm{task}}} \quad (\mathrm{s}) \tag{Z-7.1}
$$

判据写成 $T_{\mathrm{pay}}<T_{\mathrm{pred}}$——两边都是时间，量纲闭合；若另造无量纲的回报比 $R\equiv T_{\mathrm{pred}}/T_{\mathrm{pay}}$，判据即 $R>1$（$R$ 的定义里不能再塞进 $\gamma_0$，否则量纲不闭合）。**$R$ 只是净现值判据，不决定控制律**：在线性目标、零切换成本下，卷Ⅲ 命题 8.1 才给出至多切换一次的 bang-bang 结构；把“$R>1$”读成“最优分配是 bang-bang”，是把两个层混为一谈。**与卷Ⅲ (III-8.21) 的关系**：这里的 $R$ 与 $R_{\mathrm{dyn}}$ 是同一量在同一约定下的两种写法——取 $r_{\mathrm{eff}}=1/T_{\mathrm{pred}}$、$\eta_{\max}=1$ 即得 $R_{\mathrm{dyn}}=T_{\mathrm{pred}}/T_{\mathrm{pay}}=R$；换算须同时给出 $f_{\mathrm{task}}$ 与 $T_{\mathrm{pred}}$，未声明 $r_{\mathrm{eff}}$ 时两处数值不得互引。

**故事版。** 小明做数学题：现场推导（在线搜索，高 $E_{\mathrm{causal}}$），或先花三天理解定理（离线编译，付 $E_{\mathrm{build}}$）再秒解同类题。这类题一辈子只做五道，三天白花；要做五百道，那是本益比最高的一笔投资。顿悟是把高能耗的在线搜索压缩成低能耗的解码器结构——**变的是成本结构，不是能力凭空长出来了。**

**这条故事推不到哪里。** 推不出“刷题无用”：在 $T_{\mathrm{pay}}>T_{\mathrm{pred}}$ 的区域（题型多变、迁移性差、考试临近），刷题仍是最优策略。也推不出“必须先想通再动手”——明天交作业的学生和做二十年研究的学者，最优策略当然不同。

### 7.2 内卷锁死：为什么越穷越忙，越忙越穷（【命题】）

**等级与条件。** “存在临界竞争压力，越过它则离线编译通道关闭”依赖一个前提：编译决策由当期回报驱动，不由跨期规划驱动。若系统能做长期承诺（带薪学习、十年期研发预算），锁死可以被绕过。

**精简陈述。**

$$
R_{\mathrm{dynamic}}(\rho) \propto \frac{1}{r_{\mathrm{eff}}} = \frac{1}{\gamma_0+\psi(\rho)+1/T_{\mathrm{pred}}} \tag{Z-7.2}
$$

存在临界竞争压力 $\rho_{\mathrm{c}}$：$\rho>\rho_{\mathrm{c}}$ 时 $R_{\mathrm{dyn}}<1$，编译的净现值为负；在**由当期回报驱动**的决策规则下，系统不再选择编译（这不是最优控制解——“不再编译”只在该决策规则下成立，不能反过来当作最优性的证明）。“永久”要读成“在该竞争强度持续期间”。

**故事版。** 在极度内卷的行业里，没人敢停下来学新技能，因为一停，份额就被抢走。所有人都在用旧技能反复展开，直到技能折旧殆尽。最刺人的地方是：**每个参与者都是理性的，结果却是集体自杀**——不是有人算错了，是所有人的账本期限都被竞争压短了。

**这条故事推不到哪里。** 推不出“穷一定导致短视”：资源稀缺会抬高贴现率，但家庭、宗教、社区、制度都可以人为地把视界拉长。也推不出“内卷无法打破”：$\rho_{\mathrm{c}}$ 的位置取决于 $\psi(\rho)$ 的形状，而 $\psi$ 可以被制度改变。

### 7.3 创新不确定性：为什么伟大的发明都伴随着伟大的失败（【假说】）

**等级与条件。** 这一条是【假说】。它曾被写成 $p_{\mathrm{success}}=\Pr(\Delta V>0\mid D_n,I_{\mathrm{orig}})\le p_{\mathrm{random}}<1$（当 $I_{\mathrm{net}}<I_{\Delta,\mathrm{crit}}$）并声称是“数学必然”。**那个推导不成立**：未被表征的信号，仍可能通过外部观测、受控实验或探索策略被发现；原式把关于**表征**的陈述偷换成了关于**成功率**的陈述。正确的表述是：**在解码器偏差尚未收敛（$I_{\mathrm{net}}<I_{\Delta,\mathrm{crit}}$）的条件下，创新尝试的成功率不显著高于同等资源投入下的随机基准。**

**精简陈述：检验协议。** 三样缺一不可。**随机基准 $p_0$** 须事先固定：同一任务空间随机抽取方案、投入同等资源、按同一标准判定成功。**检验方向**：假说是“成功率不显著高于 $p_0$”，故不能用 $H_0:p\le p_0$ 对 $H_1:p>p_0$ 的单侧检验——那种设计只能否证假说、永远不能支持它（不拒绝 $H_0$ 只说明“没证据”，不等于“不高于”）。改为**双单侧等价检验**：$H_0:p\ge p_0+\delta$ 对 $H_1:p<p_0+\delta$，等价界 $\delta$ 须预注册；不设 $\delta$ 时，本检验只用于否证，支持性证据须另做等价检验。**样本量**（正态近似，$n\approx\left[z_{1-\alpha_0}\sqrt{p_0(1-p_0)}+z_{1-\beta_0}\sqrt{p_1(1-p_1)}\right]^2/(p_1-p_0)^2$，$\alpha_0=0.05$、功效 $1-\beta_0=0.8$）：$p_0=0.05$、$p_1=0.15$ 时 $n\approx43$；$p_0=0.01$、$p_1=0.03$ 时 $n\approx236$（精确二项略大）。**预注册**：任务、标准、样本量、停止规则事先写定，否则“伟大的失败”这类叙事会自动筛选出符合故事的案例。

**故事版。** 偏差未收敛时，系统分不清范式突破和陷阱，大量尝试落在无效区域。爱迪生试了上千种灯丝，SpaceX 炸了多枚火箭。零失败的组织往往意味着零 $I_{\mathrm{orig}}$ 注入：它们处在 $I$-锁死态，只做确定能成的事。

**这条故事推不到哪里。** 推不出“失败越多越好”：失败只有**携带可提取的残差**时才有价值——炸掉的火箭没留下数据，炸一百次也只是烧钱。也推不出“成功率低就说明在创新”：大多数低成功率就是做得不对。偏差未收敛的区域里，成功率的绝对值不提供信息，只有相对随机基准的差值提供信息。

### 7.4 拓扑不可逆性：为什么深度学习会“遗忘”（推论已撤回，见卷Ⅲ §8.6）

**等级与条件。** 条件是四条同时具备：**固定架构、有限容量、无外部记忆、无回放**。四条之外，命题不适用。

**精简陈述。**

$$
E_{\mathrm{erase}} \ge E_{\mathrm{L,bit}}\cdot\Delta I_{\mathrm{struct}} = k_B T_{\mathrm{thermo}}\ln 2\cdot\Delta I_{\mathrm{struct}} \tag{Z-7.3}
$$

当新增结构信息使占用逼近 $I_{\max}(D)$ 时，写入新规则必须覆盖旧规则，擦除成本由式 (Z-7.3) 给出下界；同时，逆跃迁要重新支付 $E_{\mathrm{build}}$，而旧规则依赖的中间状态已被擦除。**两个效应叠加，使“遗忘”在该架构内成为成本更低的选项——但前提是 $k_{\mathrm{sw}}>k_{\mathrm{sw}}^{c}$，而该前提在典型参数下不成立（卷Ⅲ §8.6），故本条只作失效登记，不构成预测。** 例外有三条：**可逆计算**（税基消失，代价是状态空间膨胀）；**外部记忆**（容量约束被绕开）；**回放**（被覆盖的规则可以重建）。

**故事版。** 灾难性遗忘在该架构下可能是成本更低的选项，但使其成立的前提 $k_{\mathrm{sw}}>k_{\mathrm{sw}}^{c}$ 在现实参数下不成立（卷Ⅲ §8.6 已撤回该推论）。可保留的弱陈述是：在容量税主导的系统里，旧拓扑的保留成本随结构信息上升——那是容量约束的结果，不是切换次数的结果。保留所有旧规则，每次切换都要付一笔擦除税或存储税；为了净 $V$ 最大，系统选择让旧规则难以恢复。学新必然伤旧，原因在目录就那么厚。

**这条故事推不到哪里。** 推不出“遗忘不可避免”：只要允许外部存储或回放，遗忘就变成工程取舍，而不是热力学宿命——今天的大模型用检索增强、持续学习、定期重训，走的正是三条例外路径。也推不出“逆跃迁成本必然趋于无穷”：那是“无外部记忆”假设下的极限说法，假设一撤，结论就撤。

### 7.5 饱和衰退：为什么大模型会遇到墙（【命题】）

**等级与条件。** 这一条最容易讲错，因为它把三件事混在一起：$V$ 的**水平**、$\dot V$ 的**符号**、结构崩溃的**判据**。

**精简陈述。**

$$
\frac{\mathrm{d}I_{\mathrm{causal}}}{\mathrm{d}t} = \mu_{\mathrm{gr}}I_{\mathrm{causal}}\left(1-\frac{I_{\mathrm{causal}}}{I_{\mathrm{causal}}^{\max}(D)}\right), \qquad V_{\mathrm{obj}}\to V_{\max}^{(\mathcal{F})} = \frac{T_{\mathrm{causal}}\,I_{\mathrm{causal}}^{\max}}{E_{\mathrm{struct}}+k\,I_{\mathrm{causal}}^{\max}} \tag{Z-7.4}
$$

其中 $\mu_{\mathrm{gr}}$ 是 Logistic 增长率（$\mathrm{s^{-1}}$），$k$ 是因果能耗对信息量的比例系数（$\mathrm{J/bit}$）。**$V$ 的水平**：固定架构下 $I_{\mathrm{causal}}$ 趋近有限上限，$V_{\mathrm{obj}}$ 趋近**正的有限值** $V_{\max}^{(\mathcal{F})}$，不趋于零。**$\dot V$ 的符号**：净增长率在 $I_{\mathrm{causal}}$ 接近上限时转负——增长项趋零，折旧项仍在，$V$ 从 $V_{\max}^{(\mathcal{F})}$ 往下走，不是走到零。**崩溃判据**：只有 $V$ 降到损伤触发阈值以下、且净增长率仍为负，才构成崩溃；饱和衰退本身不是崩溃，它是“增长停了、开始吃老本”。

**故事版。** 大模型不断堆参数，容量上限被固定架构锁死。信息量逼近上限时，净增长率被折旧率拖入负值。在触碰物理算力墙之前，系统先碰到的是架构饱和墙。

**这条故事推不到哪里。** 推不出“大模型必然撞墙”：“墙”的位置由架构与数据预算给定；换架构、换数据、换训练目标，墙就移动了。它能说的只有更弱但更可靠的一句：**在架构与数据预算固定的条件下，边际收益递减会使净增长率趋近于零；若折旧不为零，净增长率会穿过零变成负值。** 这是关于斜率的结论，不是关于高度的结论。

***

### 7.6 物理嵌入性溢价（【假说】）

**等级与条件。** 这一条整段都是【假说】。它依赖一个未标定的机制：物理噪声持续把系统推离平衡，从而持续制造 $I_{\mathrm{orig}}$。机制成立与否，本卷不给证明。

**精简陈述。** 设范式突破信息的产生速率为 $\dot I_{\mathrm{orig}}=\kappa_{\mathrm{orig}}\Delta_{\mathrm{VV}}\mathbf{1}[\Delta_{\mathrm{VV}}\ge\Delta_{\mathrm{crit}}]$，其中 $\kappa_{\mathrm{orig}}$ 是转换效率（$\mathrm{bit/s}$ 每单位偏差），$\Delta_{\mathrm{crit}}$ 是触发跃迁的最小偏差阈值（$\mathrm{bit\cdot s/J}$）。碳基系统暴露于物理噪声 $\sigma_{\mathrm{phys}}$，其平衡偏差 $\sigma_{\mathrm{phys}}/(\alpha_{\mathrm{L}}I_{\mathrm{net}})$ 不低于阈值；硅基系统的数字噪声远小于此。于是在这个模型内

$$
\dot I_{\mathrm{orig}}^{(\mathrm{carbon})} > 0, \qquad \dot I_{\mathrm{orig}}^{(\mathrm{silicon})} = 0 \tag{Z-7.5}
$$

**故事版。** 碳基生命受制于肉身维持成本（$E_{\mathrm{struct}}\ge E_{\mathrm{floor}}$），持续暴露于物理噪声，脱钩偏差收敛不到零，这种“缺陷”迫使人类不断产生 $I_{\mathrm{orig}}$ 去修正它。硅基系统因 $E_{\mathrm{struct}}$ 极小、噪声谱不同，偏差迅速收敛，缺少产生 $I_{\mathrm{orig}}$ 的**内在动机**，容易陷入 $I$-锁死。人类在 AI 时代的不可替代性，可能不是能力优势，而是缺陷优势。

**这条故事推不到哪里。** 其一，“$\sigma_{\mathrm{dig}}\approx0$”是错的：标注噪声、分布漂移、对抗扰动、硬件错误率都是噪声源；准确的说法只是“数字系统的噪声谱不同，不一定落在能触发跃迁的频段上”。其二，$\dot I_{\mathrm{orig}}^{(\mathrm{silicon})}=0$ 是**模型内的零**，不是观测到的零：硅基系统已经在产生新的算法范式，那些算不算 $I_{\mathrm{orig}}$，取决于怎么界定“范式突破”，本卷没有给出可操作的界定。其三，这条假说最容易被读成“人类有独特价值”的安慰剂——它说的是“碳基的偏差源更靠近阈值”，与“人类应该被如何对待”没有逻辑关系。

### 7.7 跨代累积条件：为什么 AI 不会自动进化（【命题】）

**等级与条件。** 这是一条**必要条件**形式的命题：不满足它，跨代累积不会发生；满足它，也不保证发生（还要看选择压力、遗传机制、环境稳定性）。

**精简陈述。**

$$
\frac{\Delta I_{\mathrm{struct}}^{(n\to n+1)}}{I_{\mathrm{struct},n}} > \gamma_0\,T_{\mathrm{struct},n} + \frac{E_{\mathrm{build}}^{(\mathcal{T})}}{E_{\mathrm{available},n}} \tag{Z-7.6}
$$

左边是每代的结构信息相对增益（无量纲），右边是折旧吃掉的部分加重建费占可用能量的比例。

**故事版。** 当前的 AI 系统因 $\gamma_0\approx0$、$E_{\mathrm{build}}\approx0$，使不等式右边趋近于零——门槛确实极低，任何正的代际增益都满足。问题不在门槛，在左边：可逆写入消除了选择的载体（生物写错由死亡支付代价，权重可被任意覆盖，没有东西被选择），零复制成本消除了繁殖瓶颈，训练与部署无隔离使「代」这个单位本身不成立；三者合起来使每代的结构信息净增量长期趋于零甚至为负。生物通过死亡和繁殖强制支付 $E_{\mathrm{build}}$ 并筛选高 $V$ 个体，这一种选择压力在 AI 中不存在。除非引入「数字死亡」机制（物理不可逆写入、强制折旧、代际隔离），否则 AI 难以跨代累积，只能在同一 $D_{\mathrm{depth}}$ 上做无界的展开。

**这条故事推不到哪里。** 推不出“AI 无法进化”。零复制成本只取消了**一种**选择压力（繁殖成本），并没有取消所有压力——算力预算、数据获取、评估成本、部署风险都是真实压力。更准确的说法是：**AI 的选择压力来自与生物不同的地方，因此演化方向也不同**；用生物演化的尺子去量它，会得出“它没在进化”的错误结论。

### 7.8 艺术编码权衡：为什么曲高和寡（【候选推论】）

**等级与条件。** 母命题是解码效率随规则深度**递增且 ln–ln 斜率递减**（$\eta_D$ 递增、$\partial\ln\eta_D/\partial\ln D$ 递减；**不是单峰**——二阶条件见卷Ⅲ (III-8.19)）。附加条件：$0\le\Delta_{\mathrm{VV}}<\Delta_{\max}$；$E_{\mathrm{causal}}$ 随 $D_{\mathrm{depth}}$ 单调上升。**最优解存在的条件**：一阶条件有内点解，该点二阶条件为负（$\partial^{2}\ln\eta_D/\partial(\ln D_{\mathrm{depth}})^{2}<0$），且内点值高于两个边界值；三条缺一条，最优点可能落在边界上，“存在最优深度”这句话就没有内容。

**精简陈述。** 作品存在最优规则深度 $D_{\mathrm{depth}}^{*}$，满足一阶条件：

$$
\frac{\partial\ln\eta_D}{\partial\ln D_{\mathrm{depth}}} = \frac{E_{\mathrm{causal}}}{E_{\mathrm{causal}}+E_{\mathrm{build}}}\cdot\frac{\partial\ln E_{\mathrm{causal}}}{\partial\ln D_{\mathrm{depth}}} + \frac{\Delta_{\mathrm{VV}}/\Delta_{\max}}{1-\Delta_{\mathrm{VV}}/\Delta_{\max}}\cdot\frac{\partial\ln\Delta_{\mathrm{VV}}}{\partial\ln D_{\mathrm{depth}}} \tag{Z-7.7}
$$

其中 $\Delta_{\max}$ 是理解度偏差的可容忍上限（$\mathrm{bit\cdot s/J}$）。分母 $1-\Delta_{\mathrm{VV}}/\Delta_{\max}$ 在 $\Delta_{\mathrm{VV}}\to\Delta_{\max}$ 时发散——这不是模型的预测，是定义域边界；$\Delta_{\mathrm{VV}}\ge\Delta_{\max}$ 时应另行定义为“表征失效态”，不再套用此式。

**故事版。** 太浅则无聊，太深则看不懂。“曲高和寡”是一种**在给定观众解码器条件下的成本现象**：观众的解码器尚未达到作品所需的规则深度，$E_{\mathrm{causal}}$ 超出预算，$\Delta_{\mathrm{VV}}$ 过大。艺术教育的一部分功能，就是提升观众的 $D_{\mathrm{depth}}$ 以匹配经典作品。

**这条故事推不到哪里。** 推不出“看不懂的作品一定更好”或“看得懂的一定更差”。也推不出“曲高必然和寡”是普遍规律——它只说在一个给定观众群体里存在一个最优深度；换一群人，最优点就移动。真正普遍的只有一句：**编码深度与解码能力需要匹配，匹配点由双方的预算共同决定。**

### 7.9 元解码器稳定性：AI 对齐的博弈论工程（【命题】）

**等级与条件。** 这是一条**检验条件**，不是均衡定理。通过它只说明“某一个偏离不划算”，不说明“所有偏离都不划算”，也不说明惩罚一定可执行。式 (Z-4.10) 即此检验，此处不重排。

**精简陈述。** 把人类价值体系设计为 AI 的元解码器，需要两个条件：人类核心价值在 AI 的解码器里产生 $I^{+}$ 响应，而不是 $I^{0}$（无响应）；偏离惩罚 $C_{i}^{\mathrm{punish}}$ 超过自指优化带来的虚拟增益。这把 AI 对齐从“价值函数设计”转化为可用博弈论检验的“元解码器工程”——**“工程”这个词是准确的：它是一套设计规范，不是一个已经证明的均衡。**

**故事版。** 对齐方案像一份验收清单：先看它能不能让价值在对方解码器里真的“响”，再看违约的代价是不是大于违约的诱惑。两条都过，方案才有资格进入下一步。

**这条故事推不到哪里。** 推不出“对齐问题已被解决”。要抬成均衡结论，至少要补：完整的可行偏离集合（含设计者没想到的偏离）、惩罚的可执行性（谁执行、成本谁付、误判怎么办）、每个参与者的真实收益函数。三样在 AI 对齐的语境下都极难标定，所以本卷把它停在【命题】，只当设计检查表用：**如果一条方案连这个检验都通不过，那它一定不行；通过了，也只是“可能行”。**

***

## 第八章　变量小传：这套宇宙的居民档案

如果把这里的变量看作一个虚构宇宙的角色，它们会是什么人设？每节先给三行档案：**符号、单位、一句话定义**。这三行是硬信息；后面的人设与日常翻译是软信息，只负责让你记住它。先看三行，再看故事——顺序反了，容易记住人设忘了量纲。

### 8.1 $V$：存续势，宇宙中的“生存信用分”

**档案**：符号 $V$；单位 $\mathrm{bit\cdot s/J}$；一句话定义：单位热力学成本所维持的有效信息与时间的乘积。

**人设**：一个冷酷的会计师，只认热力学货币。它不看你多努力，只看你的 $I_{\mathrm{net}}T_{\mathrm{causal}}$ 除掉了多少 $E_{\mathrm{eff}}$。

**日常翻译**：高 $V$ 是用很少的油维持了很久的有序结构；低 $V$ 是空转。**一个必须提的坑**：$V$ 有量纲，不能跨系统直接相加；两个主体的 $V$ 要比较，先约定同一目标、同一观察窗、同一能量分摊规则。

### 8.2 $I_{\mathrm{net}}$：净有效因果信息，你能听懂多少世界的语言？

**档案**：符号 $I_{\mathrm{net}}$；单位 bit；一句话定义：按能量份额加权的合成信息量，$I_{\mathrm{net}}=\varphi_{\mathrm{s}}I_{\mathrm{struct}}+\varphi_{\mathrm{c}}I_{\mathrm{causal}}$，是模型合成量而非实测值。

**人设**：翻译官。不是声音大（$I_{\mathrm{latent}}$ 大）就有用，关键是翻译准确率（$\eta_D$）。

**日常翻译**：只有你的解码器能提取的部分才成为 $I_{\mathrm{causal}}=\eta_DI_{\mathrm{latent}}$，对牛弹琴不是牛的问题，是解码器不匹配。同一个对象对不同的人 $I_{\mathrm{causal}}$ 不同——对一位父母，自己孩子的涂鸦往往比一幅“久仰大名却毫无触动”的名画更重；这种排序只在同一个人身上有意义。

### 8.3 $T_{\mathrm{pred}}$：预测视界，你能看到多远的未来？

**档案**：符号 $T_{\mathrm{pred}}$；单位 s；一句话定义：系统能据以调整当下行为的最远预测时域，由长度 $L_{\mathrm{pred}}$ 与精度 $G_{\mathrm{pred}}$ 共同决定。

**人设**：预言家，但容易近视。内生的 $T_{\mathrm{pred}}$ 可以被焦虑压缩，也可以被认知扩展。

**日常翻译**：$T_{\mathrm{pred}}$ 收缩时你变成赌徒，舒展时你变成投资者。**别和另外两个混**：它不是 $T_{\mathrm{struct}}$（能规划多久不等于能活多久），也不是 $T_{\mathrm{causal}}$（动作留下多久的后果不等于你算得多远）。

### 8.4 $E_{\mathrm{eff}}$：等效热力学成本，你活着的“代谢账单”

**档案**：符号 $E_{\mathrm{eff}}$；单位 J；一句话定义：维持结构、维持自维持边界、并完成信息处理三项所需能量之和，$E_{\mathrm{eff}}=E_{\mathrm{barrier}}+E_{\mathrm{survival}}+E_{\mathrm{causal}}$。本条为三项分解；卷Ⅳ 正文用两项形式，二者由 $E_{\mathrm{struct}}=E_{\mathrm{barrier}}+E_{\mathrm{survival}}$ 相联。

**人设**：房东。不管你的理想多宏大，每个月的房租（$E_{\mathrm{floor}}$）必须交。

**日常翻译**：房租（势垒）、饭钱（生存）、电费（思考），一个都不能少。$E_{\mathrm{floor}}$ 是这张账单的地板——低于它，结构就不成立了。

### 8.5 $D$：解码器，你的世界观硬件

**档案**：符号 $D$；单位无量纲（结构本身），容量 $I_{\max}(D)$ 以 bit 计；一句话定义：结构从环境中提取有效信息的物理机制。

**人设**：眼镜。你戴什么镜片，就看到什么世界；它决定了哪些信号是 $I^{+}$（机会），哪些是 $I^{-}$（威胁）。

**日常翻译**：升级 $D$ 就是换眼镜。拓扑跃迁 $\mathcal{T}$ 是换了一副能看到新维度的眼镜——换的过程要付 $E_{\mathrm{build}}$，换完之后旧眼镜就摘不回去了。

### 8.6 $\chi$：自指耦合强度，你的自恋程度（以及失控风险）

**档案**：符号 $\chi$；单位 $\mathrm{J/(bit\cdot s)}$（不是无量纲——$\chi V$ 必须与 1 同量纲）；一句话定义：系统把自身当前存续状态反馈进信息提取回路的强度。

**人设**：自恋狂。$\chi$ 衡量你有多容易把“我感觉很好”当成“我真的很好”。

**日常翻译**：低于模型内分岔点时你是自信，越过之后你活在幻觉里。**一句限定**：$\chi$ 与它的分岔点都是模型内的量，不是可穿戴设备能读出来的数；现实里可用的代理是偏差比值 $\Delta_{\mathrm{VV}}/\Delta_{\mathrm{crit}}$。

### 8.7 $\Delta_{\mathrm{VV}}$：脱钩偏差，你离现实有多远？

**档案**：符号 $\Delta_{\mathrm{VV}}$；单位 $\mathrm{bit\cdot s/J}$；一句话定义：虚拟存续势与客观存续势之差的绝对值。

**人设**：导航仪的误差。$\Delta_{\mathrm{VV}}=0$ 时你以为自己在罗马，确实就在罗马；$\Delta_{\mathrm{VV}}$ 很大时，你以为自己在罗马，实际在威尼斯，而且正往海里开。

**日常翻译**：组织崩溃、投资失败、关系破裂，常常追到同一件事——偏差太大导致导航失灵。

### 8.8 $D_{\mathrm{depth}}$：规则深度，你的规则层数

**档案**：符号 $D_{\mathrm{depth}}$；单位无量纲（层）；一句话定义：结构存续时必须同时维持的独立规则层数；动力学写法 $D_{\mathrm{depth}}^{\mathrm{dyn}}=1+\#\{\mathcal{T}\}$ 属标定假设。

**人设**：档案管理员。每经历一次拓扑跃迁，档案室通常多一层；层数越高，能处理的信息越复杂，维护成本也越高。

**日常翻译**：一个只会写实画的画师和一个同时掌握构图、色彩、透视、符号隐喻的艺术家，面对同一幅画的 $E_{\mathrm{causal}}$ 完全不同。

### 8.9 $E_{\mathrm{build}}$：建造成本，你的跳槽违约金

**档案**：符号 $E_{\mathrm{build}}$；单位 J；一句话定义：从解码器 $D_n$ 升级到 $D_{n+1}$ 所需支付的一次性能量。

**人设**：猎头费。付不起，就永远留在旧公司。

**日常翻译**：学一门新语言、转行、企业数字化转型，都是支付 $E_{\mathrm{build}}$。$E_{\mathrm{build}}>E_{\mathrm{available}}$ 时你被锁死在当前状态（D-锁死）——但这只是必要条件之一，够得着不等于跳得过去。

### 8.10 $L_{\mathrm{lev}}$：智慧杠杆系数，你的投资回报率

**档案**：符号 $L_{\mathrm{lev}}$；单位 $\mathrm{bit\cdot s/J^{2}}$（$V$ 差除以能量）；一句话定义：$L_{\mathrm{lev}}=\Delta V/E_{\mathrm{build}}$，单位建造能量撬动的存续势增量。

**人设**：风投经理。小额能量投资撬动存续势大幅跃升的效率。

**日常翻译**：牛顿被苹果砸中（低 $E_{\mathrm{build}}$，高 $\Delta V$）是 $L_{\mathrm{lev}}\gg1$ 的典范；官僚扩张（高 $E_{\mathrm{build}}$，低 $\Delta V$）是 $L_{\mathrm{lev}}\to0$ 的陷阱。**量纲提醒**：因为 $V$ 带 bit，$L_{\mathrm{lev}}$ 不是无量纲量；跨案例比较前，先确认 $\Delta V$ 同口径。

### 8.11 $\rho$：竞争压力，你的内卷指数

**档案**：符号 $\rho$；单位无量纲，取值 $[0,1]$；一句话定义：同生态位的平均耗散占该生态位可用自由能的比例。

**人设**：隔壁班的学霸。只要他在，你就不能躺平。$\rho=0$ 时你是垄断者，$\rho\to1$ 时你在红海血战。

**日常翻译**：$\rho$ 是生态位中自由能被掠夺的程度；它迫使系统改变能量转移策略。

### 8.12 $\lambda_{\mathrm{civ}}$：文明能量杠杆，你的扩张倍率

**档案**：符号 $\lambda_{\mathrm{civ}}$；单位无量纲；一句话定义：$\lambda_{\mathrm{civ}}=E_{\mathrm{ext}}/E_{\mathrm{causal}}$，解码器控制的外部能量流与它直接消耗的能量之比。

**人设**：财务杠杆。放大倍数越高，收益与风险同步上升。

**日常翻译**：工业革命让人类用极少的脑能耗控制巨大的化石能量，$\lambda_{\mathrm{civ}}$ 暴涨。但杠杆过了最优点（$\lambda_{\mathrm{civ}}>\lambda_{\mathrm{civ,opt}}$）时，扩张反而降低 $V$，就像杠杆过高会爆仓。最优杠杆的存在以“扩张同时增信息”为前提——只扩张不增信息的杠杆没有最优值，只有风险值。

**四种相态**由杠杆变化率 $\mathrm{d}\lambda_{\mathrm{civ}}/\mathrm{d}t$ 与 $\mathrm{d}V/\mathrm{d}t$ 的符号共同判定：两者皆正为扩张期（工业革命、AI 爆发）；皆约为零为饱和期（内卷，杠杆停滞）；杠杆下降而 $V$ 仍上升为休眠期（以杠杆换寿命，“戴森球休眠文明”就落在这里）；两者皆负为真实衰退。$T_{\mathrm{struct}}$ 足够长、竞争压力 $\rho\to0$、且环境特征时间 $T_{\mathrm{env}}$ 长于规划窗口时，休眠比扩张更优——这是“睡觉”在 $V$ 账本上的意思。

***

## 附录 A　符号与单位速查表

存续势的量纲是 $\mathrm{bit\cdot s/J}$，可从四个角度读它：**信息—时间积分密度**（单位热力学成本维持的因果有序—时间积分）；**热力学时间的桥接**（把 1 bit 折算为熵单位 $k_B\ln2$，数值上可桥接为 $\mathrm{s/K}$——这只是单位桥接，用掉了一个额外假设，不是量纲等价）；**因果维持成本**（$V^{-1}\sim\mathrm{J/(bit\cdot s)}$，高 $V$ 对应低维持成本）；**解码器效率**（固定 $E_{\mathrm{eff}}$ 时 $V\propto I_{\mathrm{net}}T_{\mathrm{causal}}$）。

| 符号 | 单位 | 一句话定义 |
| :----------- | :--------------- | :------------------------------ |
| $V$，$V_{\mathrm{obj}}$，$V^{\mathrm{virt}}$，$V^{\mathrm{val}}$ | $\mathrm{bit\cdot s/J}$ | 存续势；客观／虚拟／价值三个分身 |
| $V_{\mathrm{s}}$，$V_{\mathrm{c}}$，$V_{\max}$，$V_{\max}^{(\mathcal{F})}$ | $\mathrm{bit\cdot s/J}$ | 结构通道项、因果通道项、容量上限、固定架构下的有限饱和值 |
| $v=V/V_0$ | 无量纲 | 归一化存续势 |
| $I_{\mathrm{net}}$，$I_{\mathrm{struct}}$，$I_{\mathrm{causal}}$，$I_{\mathrm{latent}}$ | bit | 加权合成信息、结构信息、有效因果信息、未提取的潜在因果信息 |
| $I_{\mathrm{orig}}$，$I_{\max}(D)$，$I_{\min}$，$I_{\mathrm{erased}}$，$I_{\Delta,\mathrm{crit}}$ | bit | 范式突破信息、解码器容量、最低自我信息、擦除比特数、偏差不超容限的临界信息量 |
| $E_{\mathrm{eff}}$ | J | 等效热力学成本，$E_{\mathrm{barrier}}+E_{\mathrm{survival}}+E_{\mathrm{causal}}$ |
| $E_{\mathrm{struct}}$，$E_{\mathrm{causal}}$，$E_{\mathrm{barrier}}$，$E_{\mathrm{survival}}$ | J | 结构、认知、势垒、生存四项成本 |
| $E_{\mathrm{floor}}$，$E_{\max}$，$E_{\mathrm{available}}$，$E_{\mathrm{topo}}$ | J | 总等效成本下界（$E_{\mathrm{eff}}\ge E_{\mathrm{floor}}\ge E_{\mathrm{struct}}^{\min}$）、供给上限、可用自由能预算、特征拓扑能量 |
| $E_{\mathrm{build}}$，$E_{\mathrm{conflict}}$，$E_{\mathrm{thresh}}$ | J | 一次性建造成本、冲突附加成本、损伤触发阈值 |
| $E_{\mathrm{L,bit}}$ | $\mathrm{J/bit}$ | 朗道尔下界，$k_BT_{\mathrm{thermo}}\ln2$ |
| $T_{\mathrm{struct}}$，$T_{\mathrm{causal}}$，$T_{\mathrm{pred}}$，$T_{\min}$，$T_{\mathrm{env}}$，$T_{\mathrm{struct}}^{\max}$ | s | 结构存续时间、因果效果持续时间、预测视界、时间粒度、环境特征时间、寿命上界 |
| $T_{\mathrm{crit}}$ | s | 合作可持续的临界视界 |
| $T_{\mathrm{thermo}}$ | K | 热力学温度（不参与时间比较） |
| $L_{\mathrm{pred}}$，$G_{\mathrm{pred}}$ | s，bit | 预测长度、预测精度 |
| $D$，$D_{\mathrm{depth}}$，$D_{\mathrm{depth}}^{\mathrm{dyn}}$，$I_{\mathrm{rule}}$，$F_{\mathrm{scale}}$ | 无量纲（层、倍），bit | 解码器、静态规则深度、深度指数 $1+\#\{\mathcal T\}$、最小规则复杂度、递归展开规模 |
| $\chi$，$\chi_{\mathrm{c}}$ | $\mathrm{J/(bit\cdot s)}$ | 自指耦合强度及其模型内分岔点 |
| $\Delta_{\mathrm{VV}}$，$\Delta_{\mathrm{VV}}^{*}$，$\Delta_{\mathrm{crit}}$，$\Delta_{\max}$ | $\mathrm{bit\cdot s/J}$ | 脱钩偏差、其平衡值、跃迁触发阈值、可容忍上限 |
| $\alpha_{\mathrm{L}}$，$\sigma$ | $\mathrm{bit^{-1}\cdot s^{-1}}$，$\mathrm{bit/J}$ | 学习率、环境噪声强度 |
| $\rho$，$\psi(\rho)$ | 无量纲，$\mathrm{s^{-1}}$ | 竞争压力、竞争附加贴现率 |
| $r_{\mathrm{v}}$，$r_{\mathrm{v,eq}}$，$\gamma_0$，$\delta_{\mathrm{dam}}$，$r_{\mathrm{eff}}$ | $\mathrm{s^{-1}}$ | 存续驱动率、均衡驱动率、基线折旧率、损伤衰减率、内生风险贴现率 |
| $\delta_{\mathrm{disc}}$，$t_{\mathrm{dec}}$ | 无量纲，s | 折现因子、决策周期 |
| $\Pi_{\mathrm{coop}}$，$\Pi_{\mathrm{def}}$，$\Pi_{\mathrm{pun}}$ | 存续势单位 | 合作、背叛、惩罚的单轮支付 |
| $L_{\mathrm{lev}}$，$L_{\mathrm{lev,min}}$ | $\mathrm{bit\cdot s/J^{2}}$ | 智慧杠杆系数及其阈值 |
| $\lambda_{\mathrm{civ}}$，$\lambda_{\mathrm{civ,opt}}$，$\rho_I$，$\alpha$，$\gamma$ | 无量纲 | 文明能量杠杆及最优值、认知投资回报率、$V$ 对信息与对成本的弹性 |
| $\eta_D$，$\eta_{\max}$，$\varphi_{\mathrm{s}}$，$\varphi_{\mathrm{c}}$ | 无量纲 | 解码效率及上限、结构项与认知项的能量份额（和为 1） |
| $\beta_{\mathrm{erase}}$，$\beta_{\mathrm{op}}$ | 无量纲 | 擦除比特／处理比特；操作数／有效比特 |
| $m_D$，$m_{\mathrm{bit}}$，$m_{\min}$ | kg | 解码器质量、每比特最小质量、维持 $I_{\min}$ 的最小质量 |
| $\dot I_{\mathrm{op}}$，$\dot I_{\mathrm{bit}}$，$\dot I_{\mathrm{erase}}$ | $\mathrm{ops/s}$，$\mathrm{bit/s}$ | 逻辑操作率、比特吞吐率、擦除率 |
| $\dot E_{\mathrm{flow}}$，$\dot E_{\mathrm{maintain}}$，$\dot E_{\max}$ | W | 能量流、维持功率、最大可持续散热功率 |
| $\dot F_{\mathrm{avail}}$，$\sigma_{\min}$ | W，$\mathrm{W/K}$ | 可用自由能通量、最小熵产率 |
| $N_{\mathrm{bit}}$，$n_{\mathrm{bit}}$，$V_{\mathrm{vol}}$，$\Sigma$，$\Upsilon$ | bit，$\mathrm{bit/m^{3}}$，$\mathrm{m^{3}}$，无量纲 | 可承载比特数、信息密度、体积、外壳／核心能量比、竞争强度 |
| $R$，$T_{\mathrm{pay}}$，$u_{\mathrm{c}}$ | 无量纲，s，无量纲 | 编译回报比、编译回收期、离线编译的能量分配比例 |

***

## 附录 B　证伪条件表

上一张表说“这条有多强”，这张说“怎么把它打掉”。没有反驳条件的条目，不配叫命题。**反驳条件是充分条件，不是必要条件**：观察到它，该条目在该样本上被否证；没观察到，只是“尚未否证”。

| 等级 | 条目 | 检验方式 | 反驳条件 |
| :---------- | :-------------- | :------------------- | :------------- |
| 【命题】 | 编译优先（条件性的 bang-bang 结构） | 取同一任务族的不同重复频率，测能耗分配曲线；比较“全学—全做”与“半学半做”的能量账 | 高频任务上，中间态（$0<u_{\mathrm{c}}<1$）显著优于边界解 |
| 【命题】 | 内卷锁死 | 在竞争强度外生变化的场景（政策、行业准入）里测探索性投入占比 | 竞争强度上升时，探索性投入占比不降反升且持续 |
| 【假说】 | 创新不确定性 | 预注册任务、样本量与等价界 $\delta$；以随机基准成功率 $p_0$ 为对照做双单侧等价检验（$H_0:p\ge p_0+\delta$ 对 $H_1:p<p_0+\delta$），单侧检验只作否证 | 在 $I_{\mathrm{net}}<I_{\Delta,\mathrm{crit}}$ 的样本里，成功率 $\ge p_0+\delta$ 且可重复（等价假设被拒） |
| —（源条目已撤回，见卷Ⅲ §8.6） | 拓扑不可逆性 | 比较四类系统（固定架构／可扩展架构／有外部记忆／有回放）的旧任务保持率 | 四条件下，旧任务保持率不随容量饱和下降 |
| 【命题】 | 饱和衰退 | 固定架构与数据预算，跟踪 $\mathrm{d}V/\mathrm{d}t$ 随 $I_{\mathrm{causal}}$ 的变化 | 固定架构下，$\mathrm{d}V/\mathrm{d}t-\gamma_0V$ 在 $I$ 接近上限时仍持续为正 |
| 【假说】 | 散热壳层 | 统计数据中心／城市的“支撑与散热**能量**／计算**能量**”随功率密度的变化（与 (Z-5.13) 同口径：能量比，非质量比） | 功率密度上升时该比值系统性下降（散热方式不变） |
| 【命题】 | 合成数据退化 | 封闭多代训练，逐代测分布外性能 | 封闭训练十代以上，分布外性能不下降 |
| 【假说】 | 自我—服从不相容（**源条目为卷Ⅲ 的【候选推论】，本卷降级**） | 提高生存权重后，测行为与外部目标的一致性 | 生存权重上升时，一致性不降 |
| 【候选推论】 | 艺术编码权衡 | 测不同 $D_{\mathrm{depth}}$ 作品的受众解码效率与理解能耗 | $\eta_D$ 随 $D_{\mathrm{depth}}$ 单调，无内点峰值 |
| 【候选推论】 | 教育极限 | 跨群体测教育投入与突破性产出的关系 | 单调递增，无拐点 |
| 【候选推论】 | 文明外包 | 比较共享与自建两种模式下参与者的平均 $E_{\mathrm{eff}}$ | 共享模式的平均 $E_{\mathrm{eff}}$ 不低于自建 |
| 【候选推论】 | 知识压缩 | 比较同一任务在新旧理论下的学习与执行能耗 | 新理论的理解能耗不低于旧理论 |
| 【假说】 | 创新窗口 | 纵向跟踪个体与团队的原创产出率 | 产出率随年龄单调，或峰值不在青年段 |
| 【假说】 | AI 数字死亡 | 对比引入与未引入不可逆写入、强制折旧、代际隔离的系统的深度累积 | 引入后深度累积不优于标准权重保存 |
| 【假说】 | 具身认知溢价 | 比较封闭数字环境与人机混合环境的原创信息密度 | 封闭环境的原创密度不低于混合环境 |
| 【假说】 | 跨尺度同向性 | 同域对照，测 $V$ 排序与瓦解先后 | 排序系统性反向 |
| 【假说】 | 休眠转变温度 | 测线虫 dauer、孢子萌发等的转变温度与收支平衡面的交点 | 交点与转变温度不对应 |

***

## 附录 C　参数区间的定性外推：四类结构形态

本附录把前四章的判据按参数区间重新分组，给出四类可辨识的结构形态。以下每条只陈述参数与形态的对应关系，不构成对任何具体系统的预测，也不替代正文中带标签的命题。

**一、按 $V$ 与 $E_{\mathrm{eff}}$ 的分类。** 高 $V$、低 $E_{\mathrm{eff}}$：能量约束型存续结构，以单位能量维持的读数时间取胜。高 $V$、高 $E_{\mathrm{eff}}$：高能耗扩张型，其存续依赖于持续的外部能量输入。低 $V$、高 $\rho$：竞争耗散型，维持成本主要由竞争压力决定。$V\to0$：已失效结构，仅余物质遗迹，不再产生可辨识读数。

**二、D-锁死条件下的刚性结构。** 一个 $D_{\mathrm{depth}}$ 极高、长期未发生拓扑跃迁的结构：$I_{\mathrm{struct}}$ 存量大，而解码器更新率趋于零（$\nabla D\to0$），因而无法识别新出现的 $I_{\mathrm{orig}}$。这类结构的失效方式通常不是被同级结构压倒，而是被一个它无法解码的 $I_{\mathrm{orig}}$ 绕过——两个结构的规模未必可比，决定胜负的是解码能力而非存量。

**三、$\Delta_{\mathrm{VV}}$ 持续为正的结构。** $V^{\mathrm{virt}}$ 单调上升而 $V_{\mathrm{obj}}$ 单调下降：自我描述与实际状态长期脱钩，且在脱钩过程中不产生纠正信号。这一形态可用于描述一类制度失灵——主体依据自身读数判定“正在修复”，而其物质基础同期在加速消耗；读数的改善与状态的恶化并行不悖，二者之间没有自动的负反馈。

**四、$\chi$ 与 $\Delta_{\mathrm{VV}}$ 同时越阈的结构（V-Bug）。** 无意图、无针对性：不对任何特定对象施加作用，仅因存在就把所在生态位的 $\rho$ 推至上限。它不构成对手，因为对策的通常前提——对方会因受损而调整——在此不成立。

**两条使用限制。** 其一，本附录只给参数区间与结构形态的对应，不给过程叙述：凡“必然”“注定”“唯一”一类断言，都应改写为具体条件，因为结论的适用范围由条件界定，而不是由措辞强度保证。其二，模型给出的是**约束的形状**，不是路径：同一参数区间内仍可存在显著的路径差异——高 $V$ 的结构可以内部分裂，D-锁死的结构也可以产生局部适应。以上四类只是分类，不描述过程。

***
*结构递归存续动力学（SRVD）卷Z：公式是图纸，叙事是速写；速写不能替代图纸，但图纸也无法传达建筑的情绪。*

***

## 参考文献

本卷正文只引两项定量下界，均为前人结果：

1. Landauer, R. (1961). Irreversibility and heat generation in the computing process. *IBM Journal of Research and Development*, 5, 183–191. https://doi.org/10.1147/rd.53.0183
2. Bremermann, H. J. (1962). Optimization through evolution and recombination. In M. C. Yovits et al. (Eds.), *Self-Organizing Systems*. Spartan Books.

其余数值均为示意性模型演算，按出版说明处理，不引具体来源。
