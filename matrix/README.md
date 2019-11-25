# 矩阵

### 定义
- 由m行n列的数构成的矩形点表称之为m*n的矩阵，简记为A=(a<sub>i</sub><sub>j</sub>)<sub>m</sub><sub>*</sub><sub>n</sub>

### 类型
- 0矩阵：元素全为0
- 行矩阵：1 * n的矩阵或行向量
- 列矩阵：m * 1的矩阵或列向量
- 方阵：矩阵的行列数相等
- 三角矩阵：对角线左下或者右上方的元素都为0的方阵称为上(下)三角矩阵
- 单位矩阵：对角线元素全为1
- 对称矩阵：矩阵为方阵，且a<sub>i</sub><sub>j</sub> = a<sub>j</sub><sub>i</sub>
- 同型矩阵：两个矩阵的行数和列数都相等
- 转置矩阵：将一个矩阵点行和列对换得到的矩阵
    - n阶方阵时对称矩阵时当且仅当A<sup>T</sup> = A
    - n阶方阵时反对称矩阵时当且仅当A<sup>T</sup> = -A
    - (AB)<sup>T</sup> = B<sup>T</sup>A<sup>T</sup>
- 初等矩阵：单位矩阵E经过一次初等变换后所得到的方阵

### 运算
- 加法：当矩阵同型时，矩阵的元素对应相加
- 数乘：数字a与矩阵A相乘等同于矩阵点每个元素乘以a
- 乘法：矩阵A，B相乘，A的列数必须等于B的行数，相乘时，A的行与B的列对应
- 幂：矩阵必须是方阵，A<sup>2</sup> = A<sup>1</sup>A<sup>1</sup>, ... , A<sup>k+1</sup> = A<sup>k</sup>A<sup>1</sup>，运算性质：
    - k，l均为非负整数
    - A<sup>k+l</sup> = A<sup>k</sup>A<sup>l</sup>
    - (A<sup>k</sup>)<sup>l</sup> = A<sup>kl</sup>
    - 当A和B可以交换时:
        - (AB)<sup>k</sup> = A<sup>k</sup>B<sup>k</sup>
        - 可以进行完全平方公式
        - 满足二项式定理求和运算

### 初等变换
- 对换变换：交换行或列
- 倍乘变换：将一行或列伸缩n倍
- 倍加变换：将一行或列伸缩n倍后加到另外一行或列
- 与初等矩阵的关系：
    - 用m阶初等矩阵P<sub>m</sub>(i, j)乘以矩阵A=[a<sub>i</sub><sub>j</sub>]<sub>m*n</sub>，相当于把矩阵A的第i行和第j行对调
    - 用m阶初等矩阵P<sub>m</sub>(j(k))乘以矩阵A=[a<sub>i</sub><sub>j</sub>]<sub>m*n</sub>，相当于把矩阵A的第j行进行k倍的伸缩
    - 用m阶初等矩阵P<sub>m</sub>(i, j(k))乘以矩阵A=[a<sub>i</sub><sub>j</sub>]<sub>m*n</sub>，相当于把矩阵A的第j行进行k倍的伸缩后加到第i行
    - P在左变换行，P在右变换列