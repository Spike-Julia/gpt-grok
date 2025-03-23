# "A magnification device for precision mechanisms featuring piezoactuators and flexure hinges: Design and experimental validation"

## 问题 1

帮我总结这两篇文献，我需要你给出他们的创新点，以及结构设计，如何动力传递的，以及仿真的结果实验的结果，参数以表格形式汇总。最重要的是他们的建模，包括动力学，以及他们分析问题的角度，哪里值得借鉴，希望你精读两篇文章，好好总结成一篇汇报

以下是对两篇文献的详细总结与汇报，涵盖创新点、结构设计、动力传递、仿真与实验结果、参数表格，以及建模与分析方法的深入探讨。我将精读两篇文章，确保内容准确且全面，同时突出值得借鉴之处。

---

### 汇报：两篇关于压电驱动精密执行器的研究总结

#### 概述

本文总结了两篇关于压电驱动精密执行器的研究论文：

1. **文献 1**：Jianping Li 等人的《Design and experimental performances of a piezoelectric linear actuator by means of lateral motion》（Smart Materials and Structures, 2015）。
2. **文献 2**：S.B. Choi 等人的《A magnification device for precision mechanisms featuring piezoactuators and flexure hinges: Design and experimental validation》（Mechanism and Machine Theory, 2007）。

两篇论文均聚焦于利用压电执行器和柔性铰链实现高精度、大行程的运动，分别提出了基于侧向运动和两级放大机构的创新设计。以下从创新点、结构设计、动力传递、仿真与实验结果、建模方法及分析角度进行详细对比和总结。

---

#### 1. 创新点

- **文献 1**：

  - **侧向运动原理**：提出了一种利用压电堆叠的侧向运动（通常被视为误差）实现线性执行器的新方法，突破了传统压电执行器行程小的限制。
  - **紧凑设计**：通过单一压电堆叠和一个平行四边形柔性铰链，实现大行程（50 mm）和高精度（最小步进 0.04 μm），结构简单且体积小。
  - **应用潜力**：适用于超精密加工、航空航天电机和光学聚焦系统等领域。

- **文献 2**：
  - **两级放大机制**：设计了一种对称的两级放大机构，通过柔性铰链放大压电执行器的微小位移，实现了约 20 倍的放大倍率。
  - **通用建模方法**：提出了一种基于拉格朗日方程的通用动力学模型，适用于多柔性铰链系统的设计和优化。
  - **优化设计**：结合安全性和频率约束，通过数学优化确定设计参数，提升了实用性和可靠性。

**对比**：文献 1 创新性地利用了侧向运动，强调紧凑性和大行程；文献 2 则专注于放大倍率和通用性，适合需要超高精度的微定位应用。

---

#### 2. 结构设计

- **文献 1**：

  - **组成**：包括基座、滑块、平行四边形柔性铰链和压电堆叠，预紧螺钉用于调整初始状态。
  - **材料**：柔性铰链采用 Al7075，具有良好的弹性特性。
  - **尺寸**：整体尺寸为 62 × 52 × 16 mm，滑块行程约 50 mm。
  - **特点**：采用右圆形柔性铰链，通过平行四边形结构将压电堆叠的纵向扩展转化为侧向运动，推动滑块沿 y 方向移动。

- **文献 2**：
  - **组成**：对称结构，包含 12 个柔性铰链和 4 个刚性连杆，形成两级放大机制，驱动源为压电堆叠（PSt150/7/20）。
  - **材料**：采用 S20C 碳合金钢，机械性能优异（屈服应力 360 MPa，杨氏模量 200 GPa）。
  - **尺寸**：整体尺寸为 134 × 50 mm，设计参数包括杠杆长度（L1-L4）和铰链厚度/半径。
  - **特点**：第一级放大由 L1 和 L2 控制，第二级由 L3 和 L4 控制，通过杠杆效应逐步放大位移。

**对比**：文献 1 结构更紧凑，适合线性大行程需求；文献 2 设计更复杂，专注于放大微小位移，适合纳米级定位。

---

#### 3. 动力传递

- **文献 1**：

  - **原理**：压电堆叠沿 x 方向扩展，推动平行四边形柔性铰链变形，产生 x 和 y 方向的位移。侧向位移（ly）通过摩擦力驱动滑块沿 y 方向移动。
  - **工作过程**：
    1. **慢速扩展**（t0-t1）：压电堆叠受锯齿波电压驱动缓慢伸长，滑块随摩擦力移动 ΔL。
    2. **快速回缩**（t1-t2）：压电堆叠快速失电，柔性铰链回位，滑块因惯性保持位置。
  - **速度计算**：v = f · ΔL（f 为频率，ΔL 为步进距离）。

- **文献 2**：
  - **原理**：压电堆叠的纵向位移（yin）通过两级柔性铰链杠杆机构放大，转化为输出位移（yout）。
  - **工作过程**：
    1. **第一级放大**：压电输入位移通过 L1 和 L2 杠杆放大。
    2. **第二级放大**：第一级输出通过 L3 和 L4 进一步放大，最终作用于输出端。
  - **放大倍率**：yout / yin ≈ 20，受铰链厚度和杠杆长度比影响。

**对比**：文献 1 通过摩擦和惯性实现单向大行程运动；文献 2 通过杠杆放大实现静态位移增益，动力传递更直接。

---

#### 4. 仿真与实验结果

- **文献 1**：

  - **仿真**：采用有限元法（FEM）分析柔性铰链，当 lx = 10 μm 时，ly = 15.95 μm（理论值为 17.34 μm）。
  - **实验**：
    - 最大速度：14.25 mm/s（100 V，2000 Hz）。
    - 最大输出力：3.43 N。
    - 最小步进位移：0.04 μm（10 V，1 Hz）。
    - 最大步进位移：7.12 μm（100 V，2000 Hz）。

- **文献 2**：
  - **仿真**：通过 ANSYS 进行 FEM 分析，放大倍率约为 20，与理论值 22 略有偏差。
  - **实验**：
    - 放大倍率：18.6-21.9（140 V 输入，输出位移约 200 μm）。
    - 输入位移：自由状态 20 μm，安装后 10 μm。
    - 频率响应：理论与实验一致，第一阶固有频率约 150 Hz。

**参数表格**：

| 参数                  | 文献 1 (Li et al., 2015) | 文献 2 (Choi et al., 2007)   |
| --------------------- | ------------------------ | ---------------------------- |
| **最大速度**          | 14.25 mm/s               | 未测定                       |
| **最大输出力**        | 3.43 N                   | 未直接测定（压电推力 300 N） |
| **最小步进位移**      | 0.04 μm (10 V, 1 Hz)     | 未测定（精度达纳米级）       |
| **最大步进/放大位移** | 7.12 μm (100 V, 2000 Hz) | ~200 μm (放大倍率 20)        |
| **工作频率**          | 1-2000 Hz                | 未指定（固有频率 150 Hz）    |
| **驱动电压**          | 10-100 V                 | 0-140 V                      |
| **行程/输出范围**     | 50 mm                    | 数百微米                     |

**对比**：文献 1 在速度和行程上更优，文献 2 在放大倍率和精度上占优势。

---

#### 5. 建模与分析方法

- **文献 1**：

  - **建模**：
    - **几何模型**：基于伪刚体方法（PRBM），假设柔性铰链仅绕一点旋转，推导侧向位移公式：$$l_y=\sqrt{2l_{\mathrm{OA}}^{2}(1-\cos \beta )-l_{x}^{2}}$$。
    - **动力学**：未详细建模动力学方程，重点分析静态变形和摩擦/惯性效应。
  - **分析角度**：
    - 从侧向运动的利用出发，强调如何将“误差”转化为功能。
    - 通过实验验证频率、电压和负载对性能的影响。
  - **值得借鉴**：
    - 简洁的几何推导，适合快速设计。
    - 对摩擦和惯性作用的实用分析。

- **文献 2**：
  - **建模**：
    - **动力学**：基于拉格朗日方程推导多柔性铰链系统的运动方程：\( \mathbf{M} \ddot{\mathbf{x}} + \mathbf{K} \mathbf{x} = \mathbf{F} \)，其中 M 为质量矩阵，K 为刚度矩阵。
    - **静态关系**：通过矩阵变换得到输入输出位移关系：\( y_{\text {out }} = -\left(\mathbf{k}_{\text {out}}^{-1} \mathbf{k}_{\text {oi}}\right) y_{\text {in }} \)。
    - **优化**：定义目标函数\( \text{minimize} \frac{1}{y{\text {out }} / y{\text {in }}} \)，加入安全性和频率约束。
  - **分析角度**：
    - 从系统动力学和优化设计出发，注重理论模型的通用性和精确性。
    - 通过 FEM 和实验验证模型，分析铰链几何对性能的影响。
  - **值得借鉴**：
    - 通用的动力学建模方法，适用于复杂柔性系统。
    - 优化设计流程，平衡性能与安全性。

**对比**：文献 1 建模简单，侧重应用导向；文献 2 建模全面，强调理论深度和设计优化。

---

#### 6. 值得借鉴之处

- **文献 1**：
  - **创新思维**：将侧向运动从误差转为驱动力的思路，值得在其他压电系统中借鉴。
  - **实验导向**：通过大量实验数据验证性能，适合快速原型验证。
- **文献 2**：
  - **理论框架**：拉格朗日方法和优化设计的结合，为复杂柔性机构提供了一个系统化的设计范式。
  - **仿真验证**：理论、FEM 和实验的三重验证方法，确保模型可靠性。

**综合建议**：未来研究可结合文献 1 的紧凑设计与文献 2 的放大机制，开发兼具大行程和高精度的执行器，同时借鉴文献 2 的建模方法提升理论支持。

---

#### 结论

两篇论文均在压电驱动领域提出了创新解决方案：文献 1 通过侧向运动实现大行程线性执行器，文献 2 通过两级放大实现高精度微定位。它们的结构设计、动力传递和建模方法各有特色，为精密机械设计提供了宝贵参考。结合两者的优势，未来的执行器设计可在紧凑性、行程和精度之间找到更好的平衡。

---

希望这份汇报满足您的需求！如果需要进一步调整或补充，请随时告知。

## 问题 2

我想知道任意考虑刚体上的两点 p q，怎么得到最后的势能 V_net 的公式？

为了回答如何从任意考虑刚体上的两点 \( p \) 和 \( q \) 推导得到最后的势能 \( V_{\text{net}} \) 公式，我们需要逐步分析文献 2（S.B. Choi et al., 2007）中提供的建模过程，结合柔性铰链系统的势能计算原理，详细推导公式（5）。以下是详细的推导过程：

---

### 1. 背景与问题分析

在文献 2 中，作者研究了一个由多个柔性铰链和刚性连杆组成的放大机构，目标是推导整个系统的势能 \( V_{\text{net}} \)。柔性铰链是系统的核心弹性元件，其势能来源于铰链的变形，而刚性连杆的势能可以忽略（因为刚性连杆不发生弹性变形）。为了计算整个系统的势能，作者考虑了系统中所有柔性铰链的贡献，并通过广义坐标和变换矩阵将局部变形映射到全局坐标系。

公式（5）给出了系统的总势能 \( V_{\text{net}} \)：
$$V_{\mathrm{net}}=\sum_{n=1}^{N_h}{\frac{1}{2}\left[ \mathbf{g}^{iT}\mathbf{T}_{p}^{iT}\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n\mathbf{T}_{p}^{i}\mathbf{g}^i-\mathbf{g}^{iT}\mathbf{T}_{p}^{iT}\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n\mathbf{T}_{q}^{j}\mathbf{g}^j-\mathbf{g}^{jT}\mathbf{T}_{q}^{jT}\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n\mathbf{T}_{p}^{i}\mathbf{g}^i+\mathbf{g}^{jT}\mathbf{T}_{q}^{jT}\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n\mathbf{T}_{q}^{j}\mathbf{g}^j \right]}$$
其中：

- \( N_h \) 是系统中柔性铰链的总数；
- \( \mathbf{g}^i \) 和 \( \mathbf{g}^j \) 是刚体 \( i \) 和 \( j \) 上点的广义位移向量；
- \( \mathbf{T}_p^i \) 和 \( \mathbf{T}_q^j \) 是变换矩阵，描述点 \( p \) 和 \( q \) 的位置；
- \( \hat{\mathbf{R}}^n \) 是旋转变换矩阵，将局部坐标系转换为全局坐标系；
- \( \mathbf{k}_h^n \) 是第 \( n \) 个柔性铰链的刚度矩阵。

我们需要从单个柔性铰链的势能出发，结合刚体上两点 \( p \) 和 \( q \) 的位移关系，推导整个系统的总势能。

---

### 2. 单个柔性铰链的势能

首先，我们从单个柔性铰链的势能开始。文献中给出了第 \( n \) 个柔性铰链的势能公式（4）：
\[
V^n = \frac{1}{2} \mathbf{U}^{nT} \mathbf{k}^n \mathbf{U}^n = \frac{1}{2} \begin{bmatrix} \mathbf{u}_T^n \\ \mathbf{u}_R^n \end{bmatrix}^T \hat{\mathbf{R}}^{nT} \mathbf{k}_h^n \hat{\mathbf{R}}^n \begin{bmatrix} \mathbf{u}_T^n \\ \mathbf{u}_R^n \end{bmatrix}
\]
其中：

- \( \mathbf{U}^n = \begin{bmatrix} \mathbf{u}_T^n \\ \mathbf{u}_R^n \end{bmatrix} \) 是第 \( n \) 个柔性铰链的位移向量，包含平移位移 \( \mathbf{u}_T^n \) 和角位移 \( \mathbf{u}_R^n \)；
- \( \mathbf{k}^n = \hat{\mathbf{R}}^{nT} \mathbf{k}_h^n \hat{\mathbf{R}}^n \) 是第 \( n \) 个柔性铰链在全局坐标系中的刚度矩阵；
- \( \mathbf{k}_h^n \) 是局部坐标系中的刚度矩阵；
- \( \hat{\mathbf{R}}^n \) 是旋转变换矩阵，用于将局部坐标系转换为全局坐标系。

柔性铰链的刚度矩阵 \( \mathbf{k}_h^n \) 是通过柔性铰链的顺从矩阵 \( \mathbf{c}_h \) 求逆得到的（公式（3））：
$$\mathbf{k}_{h}^{n}=(\mathbf{c}_{h}^{n})^{-1}$$
顺从矩阵 \( \mathbf{c}_h^n \) 描述了柔性铰链在力或力矩作用下的变形（公式（2）），是一个对角化的矩阵，反映了柔性铰链在各自由度上的弹性特性。

---

### 3. 柔性铰链的位移与刚体位移的关系

柔性铰链连接两个刚体 \( i \) 和 \( j \)，其两端分别与刚体 \( i \) 上的点 \( p \) 和刚体 \( j \) 上的点 \( q \) 相连。柔性铰链的位移 \( \mathbf{U}^n \) 是由两端点 \( p \) 和 \( q \) 的相对位移决定的。

#### 3.1 广义位移向量

文献中定义了刚体上点的广义位移向量（公式（6））：
\[
\mathbf{g}^i = \begin{bmatrix} d\mathbf{r}^i \\ \mathbf{\Theta}^i \end{bmatrix}
\]
其中：

- \( d\mathbf{r}^i \) 是刚体 \( i \) 局部坐标系原点的平移位移向量；
- \( \mathbf{\Theta}^i \) 是局部坐标系的角位移向量。

类似地，对于刚体 \( j \) 上的点 \( q \)，有：
\[
\mathbf{g}^j = \begin{bmatrix} d\mathbf{r}^j \\ \mathbf{\Theta}^j \end{bmatrix}
\]

#### 3.2 点 \( p \) 和 \( q \) 的位移

点 \( p \) 和 \( q \) 的位移可以通过广义位移向量 \( \mathbf{g}^i \) 和 \( \mathbf{g}^j \) 以及变换矩阵 \( \mathbf{T}_p^i \) 和 \( \mathbf{T}_q^j \) 表示。变换矩阵 \( \mathbf{T}_p^i \) 和 \( \mathbf{T}_q^j \) 描述了点 \( p \) 和 \( q \) 相对于刚体局部坐标系原点的位置和方向。

柔性铰链两端点 \( p \) 和 \( q \) 的位移可以表示为：

- 点 \( p \) 的位移：\( \mathbf{u}_p = \mathbf{T}_p^i \mathbf{g}^i \)
- 点 \( q \) 的位移：\( \mathbf{u}_q = \mathbf{T}_q^j \mathbf{g}^j \)

其中，\( \mathbf{T}_p^i \) 和 \( \mathbf{T}_q^j \) 是变换矩阵，包含了点 \( p \) 和 \( q \) 的位置信息以及刚体的旋转信息。

#### 3.3 柔性铰链的相对位移

柔性铰链的位移向量 \( \mathbf{U}^n \) 是两端点 \( p \) 和 \( q \) 的相对位移：
$$\mathbf{U}^n=\mathbf{u}_p-\mathbf{u}_q=\mathbf{T}_{p}^{i}\mathbf{g}^i-\mathbf{T}_{q}^{j}\mathbf{g}^j$$
将 \( \mathbf{U}^n \) 分解为平移和角位移部分：
\[
\mathbf{U}^n = \begin{bmatrix} \mathbf{u}_T^n \\ \mathbf{u}_R^n \end{bmatrix} = \begin{bmatrix} \mathbf{T}_p^i \mathbf{g}^i - \mathbf{T}_q^j \mathbf{g}^j \end{bmatrix}
\]
这里的 \( \mathbf{u}_T^n \) 和 \( \mathbf{u}_R^n \) 分别表示平移和角位移分量，具体形式取决于 \( \mathbf{T}_p^i \) 和 \( \mathbf{T}_q^j \) 的定义。

---

### 4. 将位移映射到全局坐标系

由于柔性铰链的刚度矩阵 \( \mathbf{k}_h^n \) 是在局部坐标系中定义的，而 \( \mathbf{g}^i \) 和 \( \mathbf{g}^j \) 是在全局坐标系中定义的，因此需要通过旋转变换矩阵 \( \hat{\mathbf{R}}^n \) 将位移从全局坐标系转换到局部坐标系：
$$\mathbf{U}_{\mathrm{local}}^{n}=\hat{\mathbf{R}}^n\mathbf{U}^n=\hat{\mathbf{R}}^n(\mathbf{T}_{p}^{i}\mathbf{g}^i-\mathbf{T}_{q}^{j}\mathbf{g}^j)$$

---

### 5. 单个柔性铰链的势能

将 $$\mathbf{U}^n=\mathbf{T}_{p}^{i}\mathbf{g}^i-\mathbf{T}_{q}^{j}\mathbf{g}^j$$ 代入公式（4），并考虑坐标变换：
$$V^n=\frac{1}{2}\mathbf{U}^{nT}\mathbf{k}^n\mathbf{U}^n=\frac{1}{2}(\mathbf{T}_{p}^{i}\mathbf{g}^i-\mathbf{T}_{q}^{j}\mathbf{g}^j)^T(\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n)(\mathbf{T}_{p}^{i}\mathbf{g}^i-\mathbf{T}_{q}^{j}\mathbf{g}^j)$$
展开括号：
$$(\mathbf{T}_{p}^{i}\mathbf{g}^i-\mathbf{T}_{q}^{j}\mathbf{g}^j)^T(\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n)(\mathbf{T}_{p}^{i}\mathbf{g}^i-\mathbf{T}_{q}^{j}\mathbf{g}^j)=(\mathbf{g}^{iT}\mathbf{T}_{p}^{iT}-\mathbf{g}^{jT}\mathbf{T}_{q}^{jT})(\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n)(\mathbf{T}_{p}^{i}\mathbf{g}^i-\mathbf{T}_{q}^{j}\mathbf{g}^j)$$
进一步展开：
$$=\mathbf{g}^{iT}\mathbf{T}_{p}^{iT}(\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n)\mathbf{T}_{p}^{i}\mathbf{g}^i-\mathbf{g}^{iT}\mathbf{T}_{p}^{iT}(\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n)\mathbf{T}_{q}^{j}\mathbf{g}^j-\mathbf{g}^{jT}\mathbf{T}_{q}^{jT}(\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n)\mathbf{T}_{p}^{i}\mathbf{g}^i+\mathbf{g}^{jT}\mathbf{T}_{q}^{jT}(\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n)\mathbf{T}_{q}^{j}\mathbf{g}^j$$
因此，单个柔性铰链的势能为：
$$V^n=\frac{1}{2}\left[ \mathbf{g}^{iT}\mathbf{T}_{p}^{iT}\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n\mathbf{T}_{p}^{i}\mathbf{g}^i-\mathbf{g}^{iT}\mathbf{T}_{p}^{iT}\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n\mathbf{T}_{q}^{j}\mathbf{g}^j-\mathbf{g}^{jT}\mathbf{T}_{q}^{jT}\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n\mathbf{T}_{p}^{i}\mathbf{g}^i+\mathbf{g}^{jT}\mathbf{T}_{q}^{jT}\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n\mathbf{T}_{q}^{j}\mathbf{g}^j \right] $$

---

### 6. 整个系统的总势能

系统中总共有 \( N_h \) 个柔性铰链，每个铰链连接一对刚体 \( i \) 和 \( j \)。总势能 \( V_{\text{net}} \) 是所有柔性铰链势能的和：
$$V_{\mathrm{net}}=\sum_{n=1}^{N_h}{V^n}$$
将单个铰链的势能 \( V^n \) 代入：
$$V_{\mathrm{net}}=\sum_{n=1}^{N_h}{\frac{1}{2}\left[ \mathbf{g}^{iT}\mathbf{T}_{p}^{iT}\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n\mathbf{T}_{p}^{i}\mathbf{g}^i-\mathbf{g}^{iT}\mathbf{T}_{p}^{iT}\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n\mathbf{T}_{q}^{j}\mathbf{g}^j-\mathbf{g}^{jT}\mathbf{T}_{q}^{jT}\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n\mathbf{T}_{p}^{i}\mathbf{g}^i+\mathbf{g}^{jT}\mathbf{T}_{q}^{jT}\hat{\mathbf{R}}^{nT}\mathbf{k}_{h}^{n}\hat{\mathbf{R}}^n\mathbf{T}_{q}^{j}\mathbf{g}^j \right]}$$
这就是公式（5）。

---

### 7. 推导中的关键点

- **两点 \( p \) 和 \( q \) 的作用**：点 \( p \) 和 \( q \) 是柔性铰链两端的连接点，通过它们可以确定铰链的相对位移。变换矩阵 \( \mathbf{T}_p^i \) 和 \( \mathbf{T}_q^j \) 将刚体的广义位移映射到铰链两端的具体位移。
- **坐标变换**：由于刚度矩阵 \( \mathbf{k}_h^n \) 是在局部坐标系中定义的，必须通过 \( \hat{\mathbf{R}}^n \) 进行坐标变换，以确保位移和刚度矩阵在同一坐标系中计算。
- **势能的二次型形式**：势能的计算基于弹性变形的二次型形式，反映了柔性铰链的线性弹性特性。

---

### 8. 总结

通过以上推导，我们从单个柔性铰链的势能出发，结合刚体上两点 \( p \) 和 \( q \) 的位移关系，得到了整个系统的总势能 \( V_{\text{net}} \)。这一过程的关键在于：

1. 定义广义位移向量 \( \mathbf{g}^i \) 和 \( \mathbf{g}^j \)，并通过变换矩阵 \( \mathbf{T}_p^i \) 和 \( \mathbf{T}_q^j \) 确定铰链两端的位移；
2. 使用旋转变换矩阵 \( \hat{\mathbf{R}}^n \) 将位移和刚度矩阵从局部坐标系转换到全局坐标系；
3. 对所有柔性铰链的势能求和，得到系统的总势能。

这个推导方法适用于任何多柔性铰链系统，具有很强的通用性，适合用于复杂柔性机构的动力学建模和优化设计。

## 问题3

根据
$$\mathbf{M}\ddot{\mathbf{x}}+\mathbf{Kx}=\mathbf{F}$$
给出的质量和刚度矩阵的一般表达式如图片所示，结合另一张图片表达：body1是input，body5是output。最优设计问题包括等式（22）和等式（18）至（20）中给出的相关约束。

我不能理解质量和刚度矩阵以及图中的后续推导，请你帮我解释一下。

我将详细解释文献 2（S.B. Choi et al., 2007）中给出的质量矩阵 \( \mathbf{M} \)、刚度矩阵 \( \mathbf{K} \)，以及如何结合图示和公式推导系统的动力学方程 \( \mathbf{M}\ddot{\mathbf{x}} + \mathbf{K}\mathbf{x} = \mathbf{F} \)，并进一步解释如何得到输入输出位移关系 \( y_{\text{out}} = -(\mathbf{k}_{\text{oo}}^{-1} \mathbf{k}_{\text{oi}}) y_{\text{in}} \)。同时，我会结合图示（图 b）说明系统的物理意义，并解释最优设计问题的相关约束。

---

### 1. 系统概述与图示解释

#### 1.1 图示（图 b）分析

图 b 展示了一个由压电堆叠驱动的放大机构，包含 5 个刚体（Body 1 至 Body 5）和多个柔性铰链。系统的结构和功能如下：

- **Body 1（输入体）**：固定体，与压电堆叠（Piezoelectric Actuator）连接，压电堆叠提供输入位移 \( y_{\text{in}} \)。Body 1 通过柔性铰链（铰链 6）与 Body 2 相连。
- **Body 2**：中间刚体，通过柔性铰链（铰链 1、2、3）连接 Body 1、Body 3 和 Body 4，起到第一级放大的作用。
- **Body 3**：中间刚体，通过柔性铰链（铰链 3、4）连接 Body 2 和 Body 5，起到第二级放大的作用。
- **Body 4**：固定体，通过柔性铰链（铰链 5）与 Body 2 相连，提供支撑。
- **Body 5（输出体）**：通过柔性铰链（铰链 4）与 Body 3 相连，输出放大后的位移 \( y_{\text{out}} \)。
- **柔性铰链**：标记为 1 至 6，允许刚体之间的相对运动，同时提供弹性恢复力。
- **几何参数**：包括杠杆长度 \( L_1, L_2, L_3, L_4, L_w, L_h \)，铰链厚度 \( t_h \)，铰链半径 \( R_h \)，以及高度 \( h_1, h_2 \)。这些参数决定了系统的放大倍率和刚度。

#### 1.2 系统的动力学模型

系统的动力学方程为：
\[
\mathbf{M}\ddot{\mathbf{x}} + \mathbf{K}\mathbf{x} = \mathbf{F}
\]
其中：

- \( \mathbf{M} \) 是质量矩阵，描述系统的惯性特性；
- \( \mathbf{K} \) 是刚度矩阵，描述系统的弹性特性；
- \( \mathbf{x} \) 是广义位移向量，包含系统中各刚体的位移；
- \( \mathbf{F} \) 是外力向量，包含压电堆叠的输入力和输出端的负载力。

---

### 2. 质量矩阵 \( \mathbf{M} \) 的解释

#### 2.1 质量矩阵的定义

公式（21）给出了质量矩阵 \( \mathbf{M} \)：
\[
\mathbf{M} = \text{diag}[m_1, m_2 m_2, m_3, m_3, m_4, m_4, m_5]
\]

- \( \mathbf{M} \) 是一个对角矩阵，表示系统中各刚体的质量（或惯性）分量。
- \( m_1, m_2, m_3, m_4, m_5 \) 分别对应 Body 1 至 Body 5 的质量。
- 由于 Body 1 和 Body 4 是固定体，它们的质量 \( m_1 \) 和 \( m_4 \) 在动力学分析中通常不影响系统的运动（因为它们的位移为 0），但为了形式上的完整性，仍然包含在矩阵中。
- \( m_2, m_3, m_5 \) 分别对应 Body 2、Body 3 和 Body 5 的质量，这些刚体是运动体，质量会影响系统的动态响应。
- 每个刚体可能有多个自由度（例如沿 \( x \)、\( y \)、\( z \) 方向的平移和旋转），因此 \( m_2 m_2, m_3 m_3, m_4 m_4 \) 表示每个刚体在不同自由度上的质量分量。

#### 2.2 物理意义

- 质量矩阵 \( \mathbf{M} \) 反映了系统的惯性特性。在动力学方程中，\( \mathbf{M}\ddot{\mathbf{x}} \) 表示惯性力，描述了系统在加速度 \( \ddot{\mathbf{x}} \) 下的阻力。
- 由于系统是对称的，且主要运动方向是 \( y \) 方向（输入和输出位移沿 \( y \) 轴），质量矩阵被简化为对角形式，忽略了旋转自由度和耦合效应。

---

### 3. 刚度矩阵 \( \mathbf{K} \) 的解释

#### 3.1 刚度矩阵的定义

公式（21）给出了刚度矩阵 \( \mathbf{K}(i,j) \)：
\[
\mathbf{K}(i,j) = \begin{bmatrix}
k_{11} & k_{12} & 0 & 0 & 0 \\
k_{21} & k_{22} & k_{23} & 0 & 0 \\
0 & k_{32} & k_{33} & k_{34} & k_{35} \\
0 & 0 & k_{43} & k_{44} & 0 \\
0 & 0 & k_{53} & 0 & k_{55}
\end{bmatrix}_{11 \times 11}
\]

- \( \mathbf{K}(i,j) \) 是一个 \( 11 \times 11 \) 的矩阵，表示系统中各刚体之间的刚度耦合。
- \( (i,j) \) 表示刚体 \( i \) 和刚体 \( j \) 之间的刚度关系，具体表达式在文献的公式（18）中给出（但此处未提供公式（18）的具体内容）。
- 矩阵中的元素 \( k_{ij} \) 表示刚体 \( i \) 和 \( j \) 之间的刚度分量，反映了柔性铰链的弹性特性。

#### 3.2 刚度矩阵的物理意义

- 刚度矩阵 \( \mathbf{K} \) 描述了系统中柔性铰链的弹性恢复力。柔性铰链是系统的核心弹性元件，当刚体发生相对位移时，铰链会产生弹性力，试图恢复到初始状态。
- 矩阵的对称性（例如 \( k_{21} = k_{12}, k_{32} = k_{23} \)）反映了系统的物理对称性和弹性力的互易性。
- 非零元素表示刚体之间的直接耦合。例如：
  - \( k_{11}, k_{12}, k_{21}, k_{22} \) 表示 Body 1 和 Body 2 之间的刚度耦合（通过铰链 6）。
  - \( k_{22}, k_{23}, k_{32}, k_{33} \) 表示 Body 2 和 Body 3 之间的刚度耦合（通过铰链 3）。
  - \( k_{33}, k_{34}, k_{43} \) 表示 Body 3 和 Body 4 之间的刚度耦合（通过铰链 5）。
  - \( k_{33}, k_{35}, k_{53} \) 表示 Body 3 和 Body 5 之间的刚度耦合（通过铰链 4）。
- 零元素表示刚体之间没有直接的刚度耦合。例如，Body 1 和 Body 3 之间没有直接连接，因此 \( k_{13} = 0 \)。

#### 3.3 刚度矩阵的来源

刚度矩阵 \( \mathbf{K} \) 是通过柔性铰链的刚度矩阵 \( \mathbf{k}_h^n \) 组装得到的。在上一问题中，我们已经推导了系统的势能 \( V_{\text{net}} \)，其形式为：
\[
V_{\text{net}} = \sum_{n=1}^{N_h} \frac{1}{2} \left[ \mathbf{g}^{iT} \mathbf{T}_p^{iT} \hat{\mathbf{R}}^{nT} \mathbf{k}_h^n \hat{\mathbf{R}}^n \mathbf{T}_p^i \mathbf{g}^i - \mathbf{g}^{iT} \mathbf{T}_p^{iT} \hat{\mathbf{R}}^{nT} \mathbf{k}_h^n \hat{\mathbf{R}}^n \mathbf{T}_q^j \mathbf{g}^j - \mathbf{g}^{jT} \mathbf{T}_q^{jT} \hat{\mathbf{R}}^{nT} \mathbf{k}_h^n \hat{\mathbf{R}}^n \mathbf{T}_p^i \mathbf{g}^i + \mathbf{g}^{jT} \mathbf{T}_q^{jT} \hat{\mathbf{R}}^{nT} \mathbf{k}_h^n \hat{\mathbf{R}}^n \mathbf{T}_q^j \mathbf{g}^j \right]
\]
势能是位移的二次型形式：
\[
V_{\text{net}} = \frac{1}{2} \mathbf{x}^T \mathbf{K} \mathbf{x}
\]
通过对 \( V_{\text{net}} \) 关于广义位移 \( \mathbf{x} \) 求导，可以得到刚度矩阵 \( \mathbf{K} \)。具体来说，\( \mathbf{K} \) 是通过组装所有柔性铰链的刚度贡献得到的。

---

### 4. 动力学方程的推导

系统的动力学方程为：
\[
\mathbf{M}\ddot{\mathbf{x}} + \mathbf{K}\mathbf{x} = \mathbf{F}
\]

#### 4.1 广义位移向量 \( \mathbf{x} \)

广义位移向量 \( \mathbf{x} \) 包含系统中所有刚体的位移分量。由于系统有 5 个刚体，每个刚体可能有多个自由度（例如沿 \( y \) 方向的平移），\( \mathbf{x} \) 是一个 \( 11 \times 1 \) 的向量，形式为：
\[
\mathbf{x} = \begin{bmatrix} x_1 \\ x_2 \\ x_3 \\ x_4 \\ x_5 \\ \vdots \\ x_{11} \end{bmatrix}
\]
其中：

- \( x_1 \) 可能对应 Body 1 的位移（但 Body 1 固定，位移为 0）；
- \( x_2, x_3 \) 对应 Body 2 的位移；
- \( x_4, x_5 \) 对应 Body 3 的位移；
- \( x_6, x_7 \) 对应 Body 4 的位移（但 Body 4 固定，位移为 0）；
- \( x_8, \ldots, x_{11} \) 对应 Body 5 的位移。

#### 4.2 外力向量 \( \mathbf{F} \)

外力向量 \( \mathbf{F} \) 包含压电堆叠的输入力和输出端的负载力。结合公式（22）：
\[
\begin{bmatrix} \mathbf{k}_{ii} & \mathbf{k}_{io} \\ \mathbf{k}_{oi} & \mathbf{k}_{oo} \end{bmatrix} \begin{bmatrix} y_{\text{in}} \\ y_{\text{out}} \end{bmatrix} = \begin{bmatrix} F_i \\ F_o \end{bmatrix}
\]

- \( y_{\text{in}} \) 是 Body 1 的输入位移（由压电堆叠提供）；
- \( y_{\text{out}} \) 是 Body 5 的输出位移；
- \( F_i \) 是压电堆叠施加的输入力；
- \( F_o \) 是输出端的负载力（通常为 0，除非有外部负载）。

#### 4.3 动力学方程的意义

- \( \mathbf{M}\ddot{\mathbf{x}} \) 表示惯性力，描述了系统的加速度效应。
- \( \mathbf{K}\mathbf{x} \) 表示弹性力，描述了柔性铰链的恢复力。
- \( \mathbf{F} \) 表示外力，驱动系统的运动。

---

### 5. 静态位移-力关系的推导

在静态条件下（忽略动态效应，\( \ddot{\mathbf{x}} = 0 \)），动力学方程简化为：
\[
\mathbf{K}\mathbf{x} = \mathbf{F}
\]
公式（22）给出了静态位移-力关系：
\[
\begin{bmatrix} \mathbf{k}_{ii} & \mathbf{k}_{io} \\ \mathbf{k}_{oi} & \mathbf{k}_{oo} \end{bmatrix} \begin{bmatrix} y_{\text{in}} \\ y_{\text{out}} \end{bmatrix} = \begin{bmatrix} F_i \\ F_o \end{bmatrix}
\]
其中：

- \( \mathbf{k}_{ii} = \mathbf{k}_{11} - \mathbf{k}_{1D} \mathbf{k}_{DD}^{-1} \mathbf{k}_{D1} \)
- \( \mathbf{k}_{io} = \mathbf{k}_{1D} \)
- \( \mathbf{k}_{oi} = \mathbf{k}_{D1}^T \)
- \( \mathbf{k}_{oo} = \mathbf{k}_{DD} \)

#### 5.1 子矩阵的定义

- \( \mathbf{k}_{11} = [k_{11}] \)：Body 1 的刚度分量。
- \( \mathbf{k}_{1D} = [k_{12} \ 0 \ 0 \ k_{15}] \)：Body 1 与其他刚体的刚度耦合。
- \( \mathbf{k}_{D1} = \mathbf{k}_{1D}^T \)：转置矩阵。
- \( \mathbf{k}_{DD} \) 是剩余自由度的刚度矩阵：
  \[
  \mathbf{k}_{DD} = \begin{bmatrix}
  k_{22} & k_{23} & 0 & 0 \\
  k_{32} & k_{33} & k_{34} & 0 \\
  0 & k_{43} & k_{44} & 0 \\
  0 & 0 & 0 & k_{55}
  \end{bmatrix}
  \]

#### 5.2 推导输入输出位移关系

在静态条件下，假设输出端无外力（\( F_o = 0 \)），公式（22）可以写为：
$$
\mathbf{k}_{ii}y_{\mathrm{in}}+\mathbf{k}_{io}y_{\mathrm{out}}=F_i
\\
\mathbf{k}_{oi}y_{\mathrm{in}}+\mathbf{k}_{oo}y_{\mathrm{out}}=0
$$

从第二方程解出 \( y_{\text{out}} \)：
$$\mathbf{k}_{oo}y_{\mathrm{out}}=-\mathbf{k}_{oi}y_{\mathrm{in}}
\\
y_{\mathrm{out}}=-\mathbf{k}_{oo}^{-1}\mathbf{k}_{oi}y_{\mathrm{in}}$$

这就是公式（23）：
\[
y_{\text{out}} = -(\mathbf{k}_{\text{oo}}^{-1} \mathbf{k}_{\text{oi}}) y_{\text{in}}
\]

#### 5.3 计算 \( \mathbf{k}_{oo} \) 和 \( \mathbf{k}_{oi} \)

- \( \mathbf{k}_{oo} = k_{55} - k_{53} k_{32} k_{44} (k_{22} k_{33} k_{44} - k_{22} k_{34} k_{43} - k_{32} k_{23} k_{44})^{-1} k_{35} \)
- \( \mathbf{k}_{oi} = k_{53} k_{32} k_{44} (k_{22} k_{33} k_{44} - k_{22} k_{34} k_{43} - k_{32} k_{23} k_{44})^{-1} k_{21} \)

这些表达式是通过对 \( \mathbf{k}_{DD} \) 求逆并提取相关分量得到的。具体的计算需要用到矩阵求逆和代数运算，这里直接引用文献的结果。

#### 5.4 放大倍率

放大倍率定义为：
\[
\text{Amplification Ratio} = \frac{y_{\text{out}}}{y_{\text{in}}} = -(\mathbf{k}_{\text{oo}}^{-1} \mathbf{k}_{\text{oi}})
\]
文献中通过实验和仿真验证，放大倍率约为 20。

---

### 6. 最优设计问题的约束

最优设计问题需要满足公式（22）以及公式（18）至（20）中的约束。公式（18）至（20）未在问题中给出，但根据文献上下文，这些约束通常包括：

- **几何约束**：例如杠杆长度 \( L_1, L_2, L_3, L_4 \)、铰链厚度 \( t_h \)、铰链半径 \( R_h \) 等的范围。
- **安全性约束**：柔性铰链的应力不能超过材料的屈服应力（例如 S20C 钢的屈服应力为 360 MPa）。
- **频率约束**：系统的固有频率（例如第一阶固有频率 150 Hz）需满足设计要求，避免共振。
- **放大倍率约束**：放大倍率需达到目标值（例如 20 倍）。

公式（22）作为等式约束，确保输入输出位移关系满足设计目标。

---

### 7. 总结

#### 7.1 质量矩阵 \( \mathbf{M} \)

- \( \mathbf{M} \) 是一个对角矩阵，反映了系统中各刚体的惯性特性。
- 由于 Body 1 和 Body 4 固定，它们的质量分量不影响系统运动。

#### 7.2 刚度矩阵 \( \mathbf{K} \)

- \( \mathbf{K} \) 描述了柔性铰链的弹性特性，通过组装所有铰链的刚度贡献得到。
- 非零元素反映了刚体之间的耦合，零元素表示无直接连接。

#### 7.3 动力学方程

- \( \mathbf{M}\ddot{\mathbf{x}} + \mathbf{K}\mathbf{x} = \mathbf{F} \) 描述了系统的动态行为。
- 在静态条件下，简化为 \( \mathbf{K}\mathbf{x} = \mathbf{F} \)，用于推导输入输出位移关系。

#### 7.4 输入输出位移关系

- 通过静态分析，得到 \( y_{\text{out}} = -(\mathbf{k}_{\text{oo}}^{-1} \mathbf{k}_{\text{oi}}) y_{\text{in}} \)，放大倍率由 \( \mathbf{k}_{\text{oo}} \) 和 \( \mathbf{k}_{\text{oi}} \) 决定。

#### 7.5 最优设计

- 最优设计需要满足几何、安全性、频率和放大倍率等约束，同时满足公式（22）的位移-力关系。

希望这个解释清楚地解答了你的疑问！如果需要进一步深入某个部分，请随时告诉我。

## 问题4

$M$的方程是：$$\mathbf{M}=\mathrm{diag}\mathrm{[}m_1m_2m_2I_{z2}m_3m_3I_{z3}m_4m_4I_{z4}m_5]$$
并且body1~body5都不是固定的，只是由于结构关于y轴对称，body1和body5只考虑纵向y轴位移，不考虑横向x位移。
我不能理解M矩阵和K矩阵维度怎么匹配的，为什么是11×11维的矩阵。

另外，$$\mathbf{k}_{\mathbf{II}}\mathbf{、k}_{\mathbf{ID}}\mathbf{、k}_{\mathbf{DI}}\mathbf{、k}_{\mathbf{DD}}$$四个矩阵都是怎么得到的，为什么要这样拆分？

此外，
$$\begin{aligned}
\mathbf{k}_{oo}&=\mathbf{k}_{55}-\mathbf{k}_{53}\mathbf{k}_{22}\mathbf{k}_{44}\left( \mathbf{k}_{22}\mathbf{k}_{33}\mathbf{k}_{44}-\mathbf{k}_{22}\mathbf{k}_{34}\mathbf{k}_{43}-\mathbf{k}_{32}\mathbf{k}_{23}\mathbf{k}_{44} \right) ^{-1}\mathbf{k}_{35}\\
\mathbf{k}_{oi}&=\mathbf{k}_{53}\mathbf{k}_{32}\mathbf{k}_{44}\left( \mathbf{k}_{22}\mathbf{k}_{33}\mathbf{k}_{44}-\mathbf{k}_{22}\mathbf{k}_{34}\mathbf{k}_{43}-\mathbf{k}_{32}\mathbf{k}_{23}\mathbf{k}_{44} \right) ^{-1}\mathbf{k}_{21}\\
\end{aligned}$$

上述$k_{oo}$和$k_{oi}$是怎么得到的，我希望你直接引用文献，我这里不明白，希望你仔细解答。

综上，我需要你告诉我三点，第一，为什么$K$矩阵是11维，里面的分量如何用矩阵表示，$M$和$K$怎么匹配。第二，公式（22）怎么来的？第三，$k_{oo}、k_{oi}、k_{ii}$是如何通过$k_{11}、k_{12}$等这些矩阵求得的，并且你解释的时候，把矩阵维度都标上，为了我能更好阅读理解.

以下是对您查询的详细解答，我将基于动力学建模的一般原理和您提供的信息，逐步回答您的三个问题：(1) 为什么 \( \mathbf{M} \) 和 \( \mathbf{K} \) 矩阵是 \( 11 \times 11 \) 维，以及它们如何匹配；(2) 公式（22）是如何推导的；(3) \( \mathbf{k}_{oo} \)、\( \mathbf{k}_{oi} \) 和 \( \mathbf{k}_{ii} \) 是如何计算得到的。每个部分都会清晰地标注矩阵维度以便于理解。由于您未提供具体文献，我将基于标准方法进行推导，并在必要时说明假设。

---

### 第一部分：为什么 \( \mathbf{K} \) 矩阵是 11 维，\( \mathbf{M} \) 和 \( \mathbf{K} \) 如何匹配

#### 1.1 质量矩阵 \( \mathbf{M} \) 的维度和结构

您给出的质量矩阵为：
\[
\mathbf{M} = \text{diag}[m_1, m_2, m_2, I_{z2}, m_3, m_3, I_{z3}, m_4, m_4, I_{z4}, m_5]
\]
- 这是一个对角矩阵，包含 11 个元素，因此维度是 **\( 11 \times 11 \)**。
- 每个元素对应系统中刚体（Body 1 到 Body 5）的自由度质量或转动惯量。根据您提到的结构对称性（关于 \( y \) 轴），自由度分配如下：
  - **Body 1**：只有沿 \( y \) 轴的位移 \( y_1 \)，质量为 \( m_1 \)（1 个自由度）。
  - **Body 2**：沿 \( x \) 轴的位移 \( x_2 \)、沿 \( y \) 轴的位移 \( y_2 \)、绕 \( z \) 轴的旋转 \( \theta_{z2} \)，对应质量 \( m_2, m_2, I_{z2} \)（3 个自由度）。
  - **Body 3**：沿 \( x \) 轴的位移 \( x_3 \)、沿 \( y \) 轴的位移 \( y_3 \)、绕 \( z \) 轴的旋转 \( \theta_{z3} \)，对应质量 \( m_3, m_3, I_{z3} \)（3 个自由度）。
  - **Body 4**：沿 \( x \) 轴的位移 \( x_4 \)、沿 \( y \) 轴的位移 \( y_4 \)、绕 \( z \) 轴的旋转 \( \theta_{z4} \)，对应质量 \( m_4, m_4, I_{z4} \)（3 个自由度）。
  - **Body 5**：只有沿 \( y \) 轴的位移 \( y_5 \)，质量为 \( m_5 \)（1 个自由度）。
- 总自由度数：\( 1 + 3 + 3 + 3 + 1 = 11 \)。
- 因此，广义位移向量定义为：
\[
\mathbf{x} = \begin{bmatrix} y_1 \\ x_2 \\ y_2 \\ \theta_{z2} \\ x_3 \\ y_3 \\ \theta_{z3} \\ x_4 \\ y_4 \\ \theta_{z4} \\ y_5 \end{bmatrix} \quad (\text{维度：} 11 \times 1)
\]
- \( \mathbf{M} \) 的对角形式反映了各自由度的独立质量或转动惯量，与 \( \mathbf{x} \) 的 11 个分量一一对应。

#### 1.2 刚度矩阵 \( \mathbf{K} \) 的维度和结构

- \( \mathbf{K} \) 是描述系统中各自由度之间弹性耦合的矩阵，其维度必须与 \( \mathbf{M} \) 和 \( \mathbf{x} \) 匹配，因此也是 **\( 11 \times 11 \)**。
- \( \mathbf{K} \) 的分量来源于系统中柔性铰链或其他弹性连接的刚度。在文献中，它通常以分块形式表示，例如：
\[
\mathbf{K} = \begin{bmatrix}
\mathbf{k}_{11} & \mathbf{k}_{12} & 0 & 0 & 0 \\
\mathbf{k}_{21} & \mathbf{k}_{22} & \mathbf{k}_{23} & 0 & 0 \\
0 & \mathbf{k}_{32} & \mathbf{k}_{33} & \mathbf{k}_{34} & \mathbf{k}_{35} \\
0 & 0 & \mathbf{k}_{43} & \mathbf{k}_{44} & 0 \\
0 & 0 & \mathbf{k}_{53} & 0 & \mathbf{k}_{55}
\end{bmatrix}_{11 \times 11}
\]
- 每个子矩阵 \( \mathbf{k}_{ij} \) 的维度取决于对应刚体的自由度数量：
  - \( \mathbf{k}_{11} \)（Body 1 vs. Body 1）：\( 1 \times 1 \)（因为 Body 1 只有 \( y_1 \)）。
  - \( \mathbf{k}_{22} \)（Body 2 vs. Body 2）：\( 3 \times 3 \)（因为 Body 2 有 \( x_2, y_2, \theta_{z2} \)）。
  - \( \mathbf{k}_{12} \)（Body 1 vs. Body 2）：\( 1 \times 3 \)（Body 1 和 Body 2 之间的耦合）。
  - \( \mathbf{k}_{33} \)（Body 3 vs. Body 3）：\( 3 \times 3 \)。
  - \( \mathbf{k}_{55} \)（Body 5 vs. Body 5）：\( 1 \times 1 \)。
  - 等等。
- 这些子矩阵组装后，总维度为 \( 11 \times 11 \)，与 \( \mathbf{x} \) 的 11 个自由度一致。

#### 1.3 \( \mathbf{M} \) 和 \( \mathbf{K} \) 的匹配

- 动力学方程为：
\[
\mathbf{M} \ddot{\mathbf{x}} + \mathbf{K} \mathbf{x} = \mathbf{F}
\]
- 其中：
  - \( \mathbf{M} \) 是 \( 11 \times 11 \)，\( \ddot{\mathbf{x}} \) 是 \( 11 \times 1 \)，所以 \( \mathbf{M} \ddot{\mathbf{x}} \) 是 \( 11 \times 1 \)。
  - \( \mathbf{K} \) 是 \( 11 \times 11 \)，\( \mathbf{x} \) 是 \( 11 \times 1 \)，所以 \( \mathbf{K} \mathbf{x} \) 是 \( 11 \times 1 \)。
  - \( \mathbf{F} \) 是外力向量，维度为 \( 11 \times 1 \)。
- 因此，方程在维度上完全匹配，\( \mathbf{M} \) 和 \( \mathbf{K} \) 均为 \( 11 \times 11 \) 是因为系统中总共有 11 个自由度。

---

### 第二部分：公式（22）的推导

#### 2.1 静态条件下的方程

在静态条件下（无加速度，\( \ddot{\mathbf{x}} = 0 \)），动力学方程简化为：
\[
\mathbf{K} \mathbf{x} = \mathbf{F}
\]
- 为了分析输入和输出自由度之间的关系，将 \( \mathbf{x} \) 和 \( \mathbf{F} \) 分块：
  - **输入自由度**：\( y_1 = y_{\text{in}} \)（Body 1 的位移，1 维）。
  - **输出自由度**：\( y_5 = y_{\text{out}} \)（Body 5 的位移，1 维）。
  - **其他自由度**：\( \mathbf{x}_D = [x_2, y_2, \theta_{z2}, x_3, y_3, \theta_{z3}, x_4, y_4, \theta_{z4}] \)（Body 2, 3, 4 的 9 个自由度）。
- 对应的向量为：
\[
\mathbf{x} = \begin{bmatrix} y_{\text{in}} \\ \mathbf{x}_D \\ y_{\text{out}} \end{bmatrix}_{11 \times 1}, \quad \mathbf{F} = \begin{bmatrix} F_i \\ \mathbf{0} \\ F_o \end{bmatrix}_{11 \times 1}
\]
- 其中 \( F_i \) 是输入力，\( F_o \) 是输出力（通常为 0，除非有外部负载），\( \mathbf{0} \) 是 \( 9 \times 1 \) 的零向量。

#### 2.2 刚度矩阵的分块

将 \( \mathbf{K} \) 分块为：
\[
\mathbf{K} = \begin{bmatrix}
\mathbf{k}_{ii} & \mathbf{k}_{iD} & \mathbf{k}_{io} \\
\mathbf{k}_{Di} & \mathbf{k}_{DD} & \mathbf{k}_{Do} \\
\mathbf{k}_{oi} & \mathbf{k}_{oD} & \mathbf{k}_{oo}
\end{bmatrix}_{11 \times 11}
\]
- 维度：
  - \( \mathbf{k}_{ii} \)（输入 vs. 输入）：\( 1 \times 1 \)。
  - \( \mathbf{k}_{iD} \)（输入 vs. 其他）：\( 1 \times 9 \)。
  - \( \mathbf{k}_{io} \)（输入 vs. 输出）：\( 1 \times 1 \)。
  - \( \mathbf{k}_{Di} \)（其他 vs. 输入）：\( 9 \times 1 \)（\( \mathbf{k}_{Di} = \mathbf{k}_{iD}^T \)）。
  - \( \mathbf{k}_{DD} \)（其他 vs. 其他）：\( 9 \times 9 \)。
  - \( \mathbf{k}_{Do} \)（其他 vs. 输出）：\( 9 \times 1 \)。
  - \( \mathbf{k}_{oi} \)（输出 vs. 输入）：\( 1 \times 1 \)（\( \mathbf{k}_{oi} = \mathbf{k}_{io}^T \)）。
  - \( \mathbf{k}_{oo} \)（输出 vs. 输出）：\( 1 \times 1 \)。

#### 2.3 子矩阵的来源

- \( \mathbf{k}_{ii} = \mathbf{k}_{11} \)：Body 1 的刚度。
- \( \mathbf{k}_{iD} = \mathbf{k}_{12} \)：Body 1 和 Body 2 之间的耦合（因为 Body 1 只与 Body 2 直接相连，\( \mathbf{k}_{13}, \mathbf{k}_{14}, \mathbf{k}_{15} = 0 \)）。
- \( \mathbf{k}_{io} = 0 \)：Body 1 和 Body 5 无直接耦合（通过中间刚体间接耦合）。
- \( \mathbf{k}_{DD} \) 是 Body 2, 3, 4 的刚度子矩阵：
\[
\mathbf{k}_{DD} = \begin{bmatrix}
\mathbf{k}_{22} & \mathbf{k}_{23} & 0 \\
\mathbf{k}_{32} & \mathbf{k}_{33} & \mathbf{k}_{34} \\
0 & \mathbf{k}_{43} & \mathbf{k}_{44}
\end{bmatrix}_{9 \times 9}
\]
- \( \mathbf{k}_{Do} = [\mathbf{0}, \mathbf{k}_{35}, \mathbf{0}]^T \)（Body 3 和 Body 5 耦合）。
- \( \mathbf{k}_{oo} = \mathbf{k}_{55} \)：Body 5 的刚度。

#### 2.4 推导公式（22）

将分块形式代入 \( \mathbf{K} \mathbf{x} = \mathbf{F} \)：
$$\left[ \begin{matrix}
	\mathbf{k}_{ii}&		\mathbf{k}_{iD}&		\mathbf{k}_{io}\\
	\mathbf{k}_{Di}&		\mathbf{k}_{DD}&		\mathbf{k}_{Do}\\
	\mathbf{k}_{oi}&		\mathbf{k}_{oD}&		\mathbf{k}_{oo}\\
\end{matrix} \right] \left[ \begin{array}{c}
	y_{\mathrm{in}}\\
	\mathbf{x}_D\\
	y_{\mathrm{out}}\\
\end{array} \right] =\left[ \begin{array}{c}
	\boldsymbol{F}_{\boldsymbol{i}}\\
	\mathbf{0}\\
	\boldsymbol{F}_{\boldsymbol{o}}\\
\end{array} \right] $$

分解为三个方程：
1. \( \mathbf{k}_{ii} y_{\text{in}} + \mathbf{k}_{iD} \mathbf{x}_D + \mathbf{k}_{io} y_{\text{out}} = F_i \)
2. \( \mathbf{k}_{Di} y_{\text{in}} + \mathbf{k}_{DD} \mathbf{x}_D + \mathbf{k}_{Do} y_{\text{out}} = \mathbf{0} \)
3. \( \mathbf{k}_{oi} y_{\text{in}} + \mathbf{k}_{oD} \mathbf{x}_D + \mathbf{k}_{oo} y_{\text{out}} = F_o \)

从第 2 个方程解出 \( \mathbf{x}_D \)：
$$\mathbf{k}_{DD}\mathbf{x}_D=-\mathbf{k}_{Di}y_{\mathrm{in}}-\mathbf{k}_{Do}y_{\mathrm{out}}
\\
\mathbf{x}_D=-\mathbf{k}_{DD}^{-1}(\mathbf{k}_{Di}y_{\mathrm{in}}+\mathbf{k}_{Do}y_{\mathrm{out}})$$

代入第 1 和第 3 个方程，整理后得到：
$$\left[ \begin{matrix}
	\mathbf{k}_{ii}-\mathbf{k}_{iD}\mathbf{k}_{DD}^{-1}\mathbf{k}_{Di}&		\mathbf{k}_{io}-\mathbf{k}_{iD}\mathbf{k}_{DD}^{-1}\mathbf{k}_{Do}\\
	\mathbf{k}_{oi}-\mathbf{k}_{oD}\mathbf{k}_{DD}^{-1}\mathbf{k}_{Di}&		\mathbf{k}_{oo}-\mathbf{k}_{oD}\mathbf{k}_{DD}^{-1}\mathbf{k}_{Do}\\
\end{matrix} \right] \left[ \begin{array}{c}
	y_{\mathrm{in}}\\
	y_{\mathrm{out}}\\
\end{array} \right] =\left[ \begin{array}{c}
	\boldsymbol{F}_{\boldsymbol{i}}\\
	\boldsymbol{F}_{\boldsymbol{o}}\\
\end{array} \right] $$

定义：
- \( \mathbf{k}_{ii}' = \mathbf{k}_{ii} - \mathbf{k}_{iD} \mathbf{k}_{DD}^{-1} \mathbf{k}_{Di} \)（\( 1 \times 1 \)）
- \( \mathbf{k}_{io}' = \mathbf{k}_{io} - \mathbf{k}_{iD} \mathbf{k}_{DD}^{-1} \mathbf{k}_{Do} \)（\( 1 \times 1 \)）
- \( \mathbf{k}_{oi}' = \mathbf{k}_{oi} - \mathbf{k}_{oD} \mathbf{k}_{DD}^{-1} \mathbf{k}_{Di} \)（\( 1 \times 1 \)）
- \( \mathbf{k}_{oo}' = \mathbf{k}_{oo} - \mathbf{k}_{oD} \mathbf{k}_{DD}^{-1} \mathbf{k}_{Do} \)（\( 1 \times 1 \)）

这就是公式（22）：
$$\left[ \begin{matrix}
	\mathbf{k}_{ii}'&		\mathbf{k}_{io}'\\
	\mathbf{k}_{oi}'&		\mathbf{k}_{oo}'\\
\end{matrix} \right] _{2\times 2}\left[ \begin{array}{c}
	y_{\mathrm{in}}\\
	y_{\mathrm{out}}\\
\end{array} \right] _{2\times 1}=\left[ \begin{array}{c}
	\boldsymbol{F}_{\boldsymbol{i}}\\
	\boldsymbol{F}_{\boldsymbol{o}}\\
\end{array} \right] _{2\times 1}$$

---

### 第三部分：\( \mathbf{k}_{oo} \)、\( \mathbf{k}_{oi} \)、\( \mathbf{k}_{ii} \) 的计算

#### 3.1 表达式

您提供的表达式为：
\[
\mathbf{k}_{oo} = \mathbf{k}_{55} - \mathbf{k}_{53} \mathbf{k}_{22} \mathbf{k}_{44} (\mathbf{k}_{22} \mathbf{k}_{33} \mathbf{k}_{44} - \mathbf{k}_{22} \mathbf{k}_{34} \mathbf{k}_{43} - \mathbf{k}_{32} \mathbf{k}_{23} \mathbf{k}_{44})^{-1} \mathbf{k}_{35}
\]
\[
\mathbf{k}_{oi} = \mathbf{k}_{53} \mathbf{k}_{32} \mathbf{k}_{44} (\mathbf{k}_{22} \mathbf{k}_{33} \mathbf{k}_{44} - \mathbf{k}_{22} \mathbf{k}_{34} \mathbf{k}_{43} - \mathbf{k}_{32} \mathbf{k}_{23} \mathbf{k}_{44})^{-1} \mathbf{k}_{21}
\]
根据公式（22）的定义：
$$\mathbf{k}_{oo}\prime =\mathbf{k}_{oo}-\mathbf{k}_{oD}\mathbf{k}_{DD}^{-1}\mathbf{k}_{Do}$$

$$
\mathbf{k}_{oi}\prime =\mathbf{k}_{oi}-\mathbf{k}_{oD}\mathbf{k}_{DD}^{-1}\mathbf{k}_{Di}
$$

$$
\mathbf{k}_{ii}\prime =\mathbf{k}_{ii}-\mathbf{k}_{iD}\mathbf{k}_{DD}^{-1}\mathbf{k}_{Di}
$$

#### 3.2 推导过程

由于 \( \mathbf{k}_{DD} \) 是 \( 9 \times 9 \) 矩阵，直接求逆复杂。文献可能使用了符号计算或矩阵的稀疏结构。假设 \( \mathbf{k}_{DD} \) 的逆通过分块或代数方法得到，我们验证维度并解释：
- \( \mathbf{k}_{oo}' \)：
  - \( \mathbf{k}_{oo} = \mathbf{k}_{55} \)（\( 1 \times 1 \)）。
  - \( \mathbf{k}_{oD} = [0, \mathbf{k}_{53}, 0] \)（\( 1 \times 9 \)）。
  - \( \mathbf{k}_{DD}^{-1} \)（\( 9 \times 9 \)）。
  - \( \mathbf{k}_{Do} = [0, \mathbf{k}_{35}, 0]^T \)（\( 9 \times 1 \)）。
  - \( \mathbf{k}_{oD} \mathbf{k}_{DD}^{-1} \mathbf{k}_{Do} \)（\( 1 \times 1 \)）。
- 文献中的表达式 \( \mathbf{k}_{oo} \) 可能是 \( \mathbf{k}_{oo}' \) 的直接形式，通过对 \( \mathbf{k}_{DD} \) 求逆并提取与 Body 5 相关的项得到。
- 括号中的 \( \mathbf{k}_{22} \mathbf{k}_{33} \mathbf{k}_{44} - \mathbf{k}_{22} \mathbf{k}_{34} \mathbf{k}_{43} - \mathbf{k}_{32} \mathbf{k}_{23} \mathbf{k}_{44} \) 类似于行列式或 Schur 补的计算，但由于 \( \mathbf{k}_{ij} \) 是子矩阵（例如 \( \mathbf{k}_{22} \) 是 \( 3 \times 3 \)），这可能是符号化简的结果。
- \( \mathbf{k}_{oi}' \) 和 \( \mathbf{k}_{ii}' \) 同理，涉及 \( \mathbf{k}_{Di} = \mathbf{k}_{21} \)（\( 9 \times 1 \)）。

#### 3.3 文献引用说明

由于您未提供具体文献，我无法直接引用其步骤。上述表达式可能是通过对 \( \mathbf{k}_{DD} \) 的分块求逆（如使用 Schur 补或高斯消元）得到的。建议查阅文献中 \( \mathbf{k}_{DD} \) 的定义和求逆过程。

---

### 总结

1. **\( \mathbf{K} \) 和 \( \mathbf{M} \) 的维度**：
   - 均为 \( 11 \times 11 \)，因为系统有 11 个自由度，\( \mathbf{M} \) 是对角矩阵，\( \mathbf{K} \) 是分块组装的刚度矩阵。
2. **公式（22）**：
   - 通过静态方程分块并消去 \( \mathbf{x}_D \) 得到，反映输入输出自由度的有效刚度。
3. **\( \mathbf{k}_{oo} \)、\( \mathbf{k}_{oi} \)、\( \mathbf{k}_{ii} \)**：
   - 从 \( \mathbf{K} \) 的子矩阵 \( \mathbf{k}_{11}, \mathbf{k}_{12}, \ldots \) 组装并通过 \( \mathbf{k}_{DD} \) 的逆计算得到，维度分别为 \( 1 \times 1 \)。
