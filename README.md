<div align="center">
    <a name="Top"></a>
 <h1>2024测绘程序设计比赛资料</h1>
</div>
<div align="center">
    <a name="Top"></a>
    <br/>
    <details>
        <summary><strong>2024赛前日程安排（点击展开）</strong></summary>
  <p>
            <img src="https://pic-bed-1316053657.cos.ap-nanjing.myqcloud.com/img/%E8%B5%9B%E5%89%8D%E6%97%A5%E7%A8%8B%E5%AE%89%E6%8E%92.png" alt="赛前日程安排" style="zoom:30%;" />
        </p>
    </details>
    <details>
        <summary><strong>2024年测绘程序设计比赛选题及说明（点击展开）</strong></summary>
  <p>
            <img src="https://pic-bed-1316053657.cos.ap-nanjing.myqcloud.com/img/2024%E5%B9%B4%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1%E6%AF%94%E8%B5%9B%E9%80%89%E9%A2%98%E5%8F%8A%E8%AF%B4%E6%98%8E.png" alt="2024年程序设计比赛选题及说明" style="zoom:30%;" />
        </p>
    </details>
</div>

## 相关资料

* [教育部高等学校测绘类专业教学指导委员会通知官网](https://smt.whu.edu.cn/sshd/dxscxcyznds.htm)：比赛通知、结果发布地址。
* [智绘未来B站账号](https://space.bilibili.com/1965733536)：赛前培训直播和录播。
* [测绘程序设计教材](https://pan.baidu.com/s/1zHryU_X0CNb2JY0wjCn9fA?pwd=aust)/[例程](https://github.com/ybli/bookcode)/[配套视频](https://www.bilibili.com/video/BV1Gh411e7ow)：测绘程序设计比赛的官方参考书、参考例程。
* [测绘程序设计比赛讲解-回放](https://www.bilibili.com/video/BV18s4y1y71P)：2023年李英冰老师做的赛题讲解。
* [luohongk 的仓库 CeHuiProgramDesign](https://github.com/luohongk/CeHuiProgramDesign)/[24赛题讲解视频](https://www.bilibili.com/video/BV1VM4m1R7xY)/[界面设计视频](https://www.bilibili.com/video/BV19x4y127MV)。
* [LiZhengXiao99 的 2022 年省赛的界面设计视频](https://pan.baidu.com/s/1XN0B3IF7GJFRDMTwnh73ew?pwd=aust)：可以和罗哥的界面设计视频结合着看。

---

## 国赛六个题

1. [**空间数据探索性分析**](01-空间数据探索性分析)：计算标准误差椭圆、空间权重矩阵、常用空间自相关指数。

    > **试题说明**：“常用空间自相关指数”指 Moran's I、Geary's C、Getis-Ord General G，试题从中选其一或其二。  
    > **参考例程**：暂无，具体算法参考 [ArcGIS 的文档](https://pro.arcgis.com/zh-cn/pro-app/latest/tool-reference/spatial-statistics/an-overview-of-the-spatial-statistics-toolbox.htm) 。

2. [**遥感图像空间前方交会计算**](02-遥感图像空间前方交会计算)：计算立体像对的投影系数、像空间辅助坐标系坐标及地面摄影测量坐标系坐标。

    > **试题说明**：输入：点坐标；输出：计算投影系数、像空间辅助坐标系坐标、地面摄影测量坐标系坐标。  
    > **参考例程**：书上的例程有错，可以参考 [luohongk 的 C# 程序](https://github.com/luohongk/CeHuiProgramDesign/tree/main/%E9%81%A5%E6%84%9F%E5%BD%B1%E5%83%8F%E7%9A%84%E7%A9%BA%E9%97%B4%E5%89%8D%E6%96%B9%E4%BA%A4%E4%BC%9A)。

3. [**GNSS空间大气改正计算**](03-GNSS空间大气改正计算)：常用电离层改正模型、对流层改正模型计算。

    > **试题说明**：未说明使用何种改正模型。  
    > **参考例程**：书上给的例程。
4. [**纵横断面计算**](04-纵横断面计算)：道路纵断面、横断面的相关点位计算，以及断面面积计算。

    > **试题说明**：输入：道路关键点和散点数据；输出：道路纵断面、横断面相关点位计算，以及断面面积计算。  
    > **参考例程**：2022 年国赛题，书上例程是 VB 的而且读文件的时候有 BUG（有个换行符写错了），可以参考 [luohongk 的 C# 程序](https://github.com/luohongk/CeHuiProgramDesign/tree/main/%E7%BA%B5%E6%A8%AA%E6%96%AD%E9%9D%A2%E8%AE%A1%E7%AE%97) 和 [LiZhengXiao99 的 2022 年国赛程序](2022国赛李贵程-李郑骁-纵横断面（国一）)。
5. [**大地线长度计算**](05-大地线长度计算)：根据地球椭球参数和椭球面上的大地经纬度坐标，计算两点之间的大地线长度。

    > **试题说明**：输入：地球椭球参数、大地经纬度两点坐标；输出：两点之间的大地线长度。  
    > **参考例程**：书上给的例程，也可以参考大地主题正反算例程，因为大地线长度计算是大地主题反算的一部分。
6. [**曲线拟合**](06-曲线拟合)：利用五点光滑法进行曲线拟合。

    > **试题说明**：曲线坐标向内/外插值。使用五点光滑法，试题中会适当扩展。  
    > **参考例程**：书上给的例程。

---

## 评分标准

### 程序正确性（60分）

* 每项结果的分值不同。
* 会给出一些参考答案，这些答案中有干扰项。

### 时间分（20分）

设第 $i$ 组时间设为 $T_i$ ，成绩为 $S_i$，其中 $T_1$ 是第一组“程序正确性成绩 ≥ 30 分”参赛队伍的比赛时间，$T_n$ 是在规定时间内最后一组参赛队伍的比赛时间。$S_0$ 代表基础分，为 30 分。

$$S_i = \left(1 - \frac{T_i - T_1}{T_n - T_1} \times 0.4\right) \times S_0$$

由该公式可知：

* 当 $T_i = T_1$ 时，$S_i = S_0 = 30$ 分，时间得分为 20 分。
* 当 $T_i = T_n$ 时，$S_i = 0.6 \times S_0 = 18$ 分，时间得分为 12 分。

特殊情况：

* 比赛用时超过比赛规定时间 15 分钟以内，$S_i = 7$ 分。
* 比赛用时超过比赛规定时间 15 分钟以上，取消比赛资格，$S_i = 0$ 分。
* 以考生客户端关闭时间为准。

### 专家评分（20分）

* 程序优化性（10分）：人机交互界面（4分），容错性、健壮性（3分），计算成果规范（3
分，如小数点位等）。
* 程序规范性（10分）：程序设计合理（3分），类结构、函数设计清晰（3分），注释规范（2
分），类、函数、变量命名规范（2分）。

### 扣分项

* 出现选手个人信息：-5分。
* 浏览历史项目：-20分。
* 缺少报告文档（.pdf 格式）：-10分。
* 缺少源码文件（.rar 格式）：-10分。
* 成果文件命名不规范：-2分。

### 其他要求

* 读/存文件：文本格式。

* 用户界面：菜单、工具条、表格显示、文本显示等。
