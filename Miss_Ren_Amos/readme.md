# 任姐Amos处理法
## 一、项目打包 Item Parceling
*这部分在SPSS软件完成*
### 1. Dimension(维度/尺度)
1. 有Dimension：如12items有4个dimensions，则每个dimension包含3个items
2. 无Dimension：依据数据大小顺序排列，最小与最大相、次小与次大相加……计算出各项的平均值（若为奇数items，排除最中间项）
### 2. 分析(A) → 维度缩减(D) → 因素(F)
1. 将需要缩减维度的变量全选入「变量(V)」内
2. 选项(O)功能下勾选「依据因素负荷排序(S)」
3. 根据输出资料的「Communalities」排序
4. 变项若为奇数，将中间项删除，变项若为偶数，直接分组，以3~4组为原则（本题共有13个变项，删除第7个）
5. 定义新变项（NCRE1, NCRE2, NCRE3）

|             | 第一次选 | 第二次选  |    结果     |
| :---------: | :--: | :---: | :-------: |
| 分组1 (NCRE1) | 1+2  | 13+12 | 1+2+12+13 |
| 分组2 (NCRE2) | 3+4  | 11+10 | 3+4+10+11 |
| 分组3 (NCRE3) | 5+6  |  9+8  |  5+6+8+9  |

### 3. 转换(T) → 计算变量(C)：
1. 目标变量(T)填入新的变项名称（NCRE1）
2. 数值表示式(E)填入维度缩减之选取结果之「平均值」
3. 分别将新的变项计算出来
### 4. 另存新檔
   
## 二、Amos绘图与模型判别
*接下来进入AMOS软件*
### 1. 绘图


|           | 步骤|
| --------- | ---- |
| ![](https://github.com/vcve/Manag-Sci./raw/master/Miss_Ren_Amos/pastedGraphic.png)|  1. 选取SPSS数据数据<br>2. 作业区内依据变项数目划出圆形<br>3. 依据变项在SPSS内包含的项目划出分支<br>将变量名称输入圆形内 <br>4. 将变量包含之项目拖曳至方框内<br>5. Plugins → Name Unobserved Variables将小圆形赋予名称<br>6. 将各变量（大圆形）两两相连<br>7. Save the current path diagram<br>8. Calculate estimates<br>9. Analysis properties |


<img src="https://github.com/vcve/Manag-Sci./raw/master/Miss_Ren_Amos/15179034426759.jpg" width="500">

<img src="https://github.com/vcve/Manag-Sci./raw/master/Miss_Ren_Amos/15179040228929.jpg" width="500">

备注：
Model 1（SE+IM-SEXP-NCRE）：删除两两相连之线条，仅保留SE和IM之相联；
单向箭头由SE指向SEXP、由IM指向SEXP、由SEXP指向NCRE
选择 ，凡是![](https://github.com/vcve/Manag-Sci./raw/master/Miss_Ren_Amos/15179032852673.jpg)「被单向箭头指入」的大圆，皆加入一个圆，并赋予新加入之圆 Object properties；

<img src="https://github.com/vcve/Manag-Sci./raw/master/Miss_Ren_Amos/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202018-02-06%2016.33.01.png" width="400">


### 2. 记录数据

|| ∆X<sup>2</sup>   | df| ∆R<sup>2</sup> | RMSEA | CFI| TLI  |
| ----| ---- | --- | --- | --- | --- | --- |
| Baseline (变项独立)  |
| Model1 (合并变项)   |
| Model2 (合并变项)    |
| ………           |

### 3. 模型判别原则
依据三原则找出最佳Model
* 绝对原则：CFI, TLI > 0.90且越大越好；RMSEA < 0.08且越小越好
* 相对原则：∆R<sup>2</sup>显著与否，显著表示有区别，越显著越好（先看df，差一个df的话，∆R<sup>2</sup>只要3.8就算显著）
* 就简原则：完全中介最佳，关联线越少越好

![](https://github.com/vcve/Manag-Sci./raw/master/Miss_Ren_Amos/15179035472877.jpg)<br>
*图中，模型三中，1个df代表了5.455的$∆X^2$,根据相对标准，模型三最好*

## 补充：构念题目数
![](https://github.com/vcve/Manag-Sci./raw/master/Miss_Ren_Amos/15179000053747.jpg)


