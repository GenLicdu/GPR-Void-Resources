# 核验记录

一手页面和 GitHub API 读取日期：2026-09-19至2026-09-20。逐条保留实际日期。

## 验证层级与计数口径

1. 页面：实际读到官方正文，不以搜索片段替代。
2. 文件列表：实际读到文件名、大小或官方资源下载项。能预览 ZIP 目录时单独说明；只见一个 ZIP 不表示核实了 ZIP 内部。
3. 下载：必须有成功文件传输和可读取结果才能记成功。按钮存在、HEAD、跳转或已调用下载工具都不能代替验证。本轮1个独立来源成功读取数据样本：GPR014的512行时间—幅值TXT；GPR013曾发起下载但完成待核验。
4. 内容：尚未系统解包或验证标签／波形／测线。GPR014只核验一个平均A-scan样本及一个仿真输入，不能外推全库。

主目录“公开下载”指官方公开文件入口，14个独立来源可追溯；若要求“至少一个数据样本成功读取”的严格数量，当前为 **1**。GPR015两个归档仅部分文件列表已核验，文件完整性待核验。原始数据和压缩文件都不提交。

## 初始14条线索的处理

| 初始项 | 归并或结论 |
|---|---|
| commons.und.edu/data/19 | GPR001；5座桥面板，不是桥梁衬砌 |
| ahmed-elseicy/bridge-deck-delamination | L13；SDNET2021转换／模型代码，不另计 |
| Zenodo 14607117 | L13；同一软件归档，19.4 MB不是新数据规模 |
| Zenodo 14637589 | GPR002；缺陷用途不证明空洞标签，保守 C |
| Mendeley c9mmbmkwcj/2 | GPR003；雷达图 DOCX 与 TLS 点云分开，V1/V2不重复 |
| LCSkhalid/GPR_Data | L14；指向 GPR004 的同一来源 |
| Mendeley ww7fd9t325/1 | GPR004；增强图片与原始 profiles分开 |
| Zenodo 18301084 | L12；软件／权重，指向 URDD，未证实独立信号数据 |
| Mendeley rfb2jv34mz/1 | GPR005；实测／仿真未披露，不猜 |
| Data.gov ST Project 21045 | GPR006；RISE原始条目与政府聚合页合并 |
| Zenodo 8145084 | GPR007；含空气圆柱的仿真频域数据 |
| Zenodo 10962520 | GPR008；钢筋实验，C类，不是脱层 |
| Zenodo 14270869 | GPR009；四来源裁剪派生，零新增独立数 |
| Zenodo 18769571 | GPR010；原始波形与GNSS，但未证实空洞标签，C类 |

## 逐条证据

### GPR001 — SDNET2021: Annotated NDE Dataset for Structural Defects

- 分类：桥梁及桥面板；A；现场实测。依据：机构数据页明确给出桥面板脱层真值与 GPR 标注。
- 页面：已核验：已读取官方正文。
- 文件：已核验：官方文件列表；未验证文件传输。
- 抽样下载：未执行。
- 体积口径：1941395 kB；官方 4. GPR DATA.zip 文件显示值；不包含真值、测点、IE、IRT 和旧版本。
- 独立性：计入：一手发布的独立来源；未见来源声明的派生关系；未做跨库文件哈希或采集批次比对。
- 一手依据（2026-09-19）：[https://commons.und.edu/data/19/](https://commons.und.edu/data/19/) — 正文：over 663,102 annotated GPR signals；five in-service bridge decks；Class 1/2/3。文件列表：4. GPR DATA.zip (1941395 kB)。2021 旧版被 2022 修订版取代。
- 一手依据（2026-09-19）：[https://github.com/ahmed-elseicy/bridge-deck-delamination/blob/master/README.md](https://github.com/ahmed-elseicy/bridge-deck-delamination/blob/master/README.md) — 作者处理代码明确引用 SDNET2021；格式转换与模型权重不形成新数据来源。
- 一手依据（2026-09-19）：[https://zenodo.org/records/14607117](https://zenodo.org/records/14607117) — Resource type: Software；Requires 10.31356/data019。19.4 MB 是软件归档，不是新的 GPR 数据集。
- 待确认：文件格式列表来自整个多模态发布，不能将每种格式都断言为 GPR 原始格式。；天线、时间采样、信号总数的文件级复核未完成。；旧版本、转换代码和 Zenodo 软件存档均不另计。

### GPR002 — GPR DATASET

- 分类：多场景；隧道及地下衬砌；管线周边；混凝土构件；C；现场实测。依据：页面将 cavities/defects 列为潜在用途及关联论文主题，但没有确认发布包中的空洞样本与真值；保守列为 C，不能据论文主题升为 A。
- 页面：已核验：已读取官方正文。
- 文件：已核验：官方文件列表；未验证文件传输。
- 抽样下载：未执行。
- 体积口径：3.8 GB；Data Set.zip 官方文件列表，未解压统计。
- 独立性：计入：一手发布的独立来源；未见来源声明的派生关系；未做跨库文件哈希或采集批次比对。
- 一手依据（2026-09-19）：[https://zenodo.org/records/14637589](https://zenodo.org/records/14637589) — 广州大学团队实测原始 .dt 数据；3 座具名隧道、广州大学城管线及佛山钢筋；压缩包 3.8 GB。
- 待确认：多场景仅计一次。；关联空洞论文不证明发布包含可定位的空洞标签。；原始幅值标定、滤波历史、采样头和全部文件尚未验证。

### GPR003 — Data on point cloud scanning and ground radar of composite lining in jointly constructed tunnel

- 分类：隧道及地下衬砌；A；现场实测。依据：正文明确支持 Numerical evaluation of segmental tunnel lining with voids in outside backfill，并说明 GPR 检测管片外回填质量。
- 页面：已核验：已读取官方正文。
- 文件：已核验：官方文件列表；未验证文件传输。
- 抽样下载：未执行。
- 体积口径：Radagrams.docx: 50.9 MB；Point cloud.zip: 865 MB；Central axis.xlsx: 10 KB；Download All: 916 MB；页面显示值；总包包含大量非 GPR 点云，不能写成 916 MB 原始雷达数据。
- 独立性：计入：一手发布的独立来源；V1 与 V2 同一来源；仅记录 V2。。
- 一手依据（2026-09-19）：[https://data.mendeley.com/datasets/c9mmbmkwcj/2](https://data.mendeley.com/datasets/c9mmbmkwcj/2) — 回填脱空相关隧道资料：Radagrams.docx 50.9 MB，另有点云 ZIP 865 MB、轴线 XLSX 10 KB；页面总包 916 MB。
- 待确认：未打开 50.9 MB 文档，不确认内部图数、缺陷标注或是否附有数值表。；采集地、频率与时间采样未披露。

### GPR004 — Intelligent recognition of subsurface utilities and voids: A Ground Penetrating Radar dataset for Deep Learning applications

- 分类：地下空洞及岩土；管线周边；A；现场实测。依据：官方页面与作者项目明确包含 voids/cavities；管线类别并不等价于管周脱空。
- 页面：已核验：已读取官方正文。
- 文件：已核验：官方文件列表；未验证文件传输。
- 抽样下载：未执行。
- 体积口径：GPR_data.rar: 48.1 MB；Download All: 47.3 MB；平台不同下载口径显示值；未用两者相加或推算解压体积。
- 独立性：计入：一手发布的独立来源；LCSkhalid/GPR_Data 是同一数据的说明和处理代码；裁剪和增强均属于本来源，不另计。。
- 一手依据（2026-09-19）：[https://data.mendeley.com/datasets/ww7fd9t325/1](https://data.mendeley.com/datasets/ww7fd9t325/1) — 官方描述、RAR 文件列表和 CC BY 4.0 已读取。
- 一手依据（2026-09-19）：[https://github.com/LCSkhalid/GPR_Data/blob/main/README.md](https://github.com/LCSkhalid/GPR_Data/blob/main/README.md) — 明确列出 79/131/75 original profiles、553/786/900 augmented images；224×224 裁剪及增强流程；512 samples/scan、50/150 ns。
- 待确认：README 对原始与增强文件夹的措辞存在混杂；以上计数保留作者口径，未解包逐项计数。；论文 URL 由搜索命中，全文及论文 DOI 未核验；不能将数据 DOI 误标为论文 DOI。

### GPR005 — FDM-HHT-SR-dataset

- 分类：道路及路面；A；未披露。依据：作者原文：Data before and after full-data migration for the detection of subsurface cavities beneath roadways (with and without water filling)。
- 页面：已核验：已读取官方正文。
- 文件：已核验：官方文件列表；未验证文件传输。
- 抽样下载：未执行。
- 体积口径：6.68 MB；Download All 6.65 MB；ZIP 文件显示值与平台打包显示值，非解压体积。
- 独立性：计入：一手发布的独立来源；未见来源声明的派生关系；未做跨库文件哈希或采集批次比对。
- 一手依据（2026-09-19）：[https://data.mendeley.com/datasets/rfb2jv34mz/1](https://data.mendeley.com/datasets/rfb2jv34mz/1) — 道路下含水与不含水空洞的全数据偏移处理前后数据；单个 ZIP 6.68 MB，内部样本数未披露。
- 待确认：不能从标题和文件大小推断实测／仿真、样本量或标签质量。

### GPR006 — S&T Project 21045 Data: Void Detection Data

- 分类：其他；A；现场实测。依据：Bureau of Reclamation 官方目录明确为 void detection portion，包含 ground penetrating radar。
- 页面：已核验：已读取官方正文。
- 文件：已核验：机构数据项有 Download File，Data.gov 列出 ZIP 资源；ZIP 内部文件列表未核验。
- 抽样下载：未执行。
- 体积口径：未披露；未披露。
- 独立性：计入：一手发布的独立来源；未见来源声明的派生关系；未做跨库文件哈希或采集批次比对。
- 一手依据（2026-09-19）：[https://data.usbr.gov/catalog/8078/item/128829](https://data.usbr.gov/catalog/8078/item/128829) — 机构正文和 Download File 按钮可见；列明三处实验、多种 NDE 模态及报告编号。
- 一手依据（2026-09-19）：[https://catalog.data.gov/dataset/st-project-21045-data-void-detection-data](https://catalog.data.gov/dataset/st-project-21045-data-void-detection-data) — 美国政府聚合目录列出同一 RISE 项与 ZIP 地址；不与机构页面重复计数。
- 待确认：实测属性依据在具名地点开展的实验；现场试验结构与室内控制部分是否混合仍需报告核实。；项目标题涵盖多种结构，不代表每一种都在 GPR 文件中实际存在。；公开政府目录不自动等于许可明确。

### GPR007 — MERL Ground Penetrating Radar Dataset (MERL-GPR)

- 分类：地下空洞及岩土；A；数值仿真。依据：一手描述明确给出地下介质中的 air cylinder（介电常数 1）；是理想化空洞模拟，不是现场空洞验证。
- 页面：已核验：已读取官方正文。
- 文件：已核验：ZIP 名称、大小、MD5 及在线内部目录；data_frequency.h5、data_frequency_freespace.h5、normalize_complex_coeff.npy 可见。
- 抽样下载：未执行。
- 体积口径：ZIP 1.6 GB；描述称解压约 1.72 GB；包含波场、模型权重等；不能视为纯原始 GPR 信号体积。
- 独立性：计入：一手发布的独立来源；未见来源声明的派生关系；未做跨库文件哈希或采集批次比对。
- 一手依据（2026-09-19）：[https://zenodo.org/records/8145084](https://zenodo.org/records/8145084) — 400 个二维地下介质模型，每个包含一个空气圆柱和另一个介质圆柱；发布 50 个频点的复数波场；ZIP 1.6 GB。
- 待确认：仿真中的空气圆柱只代表理想化空洞，不能替代工程脱空泛化证据。；未下载 HDF5 并读取维度；标签字段布局待核验。

### GPR008 — GPR dataset: pulsed radar and SFCW data for rebar detection (experimental data)

- 分类：混凝土构件；C；实验室实测。依据：只证实钢筋目标，未证实脱层或空洞；可作为钢筋干扰／迁移候选，属于研究判断。
- 页面：已核验：已读取官方正文。
- 文件：已核验：两个 ZIP 文件及脉冲包在线目录；三个试件各可见 RAD/RD3。
- 抽样下载：未执行。
- 体积口径：3.7 MB：Pulsed radar.zip 1.2 MB，SFCW.zip 2.5 MB；官方压缩文件显示值。
- 独立性：计入：一手发布的独立来源；未见来源声明的派生关系；未做跨库文件哈希或采集批次比对。
- 一手依据（2026-09-19）：[https://zenodo.org/records/10962520](https://zenodo.org/records/10962520) — 3 个实验试件，用于脉冲与步进频率雷达钢筋探测对比；两包共 3.7 MB。
- 待确认：不把无缺陷说明等同于经过真值验证的阴性样本。；SFCW 与脉冲采样体系不同，需分别读取和比较。

### GPR009 — MCG GPR dataset

- 分类：其他；C；未披露。依据：标签为前景／背景，不是空洞语义；其水文／海岸母来源与工程脱空距离较远，仅为初始线索纠错保留。
- 页面：已核验：已读取官方正文。
- 文件：已核验：官方文件列表；未验证文件传输。
- 抽样下载：未执行。
- 体积口径：1.4 GB；MCG_GPR_dataset.zip；样本张数未披露。
- 独立性：不计入：已确认派生数据；作者明确由以上四个公开来源裁剪；不能与母数据跨训练／测试。母数据本次未全部独立核验。。
- 一手依据（2026-09-19）：[https://zenodo.org/records/14270869](https://zenodo.org/records/14270869) — 公开数据的随机裁剪与人工修订分割集合；340×720 PNG 图像和二值掩膜；ZIP 1.4 GB；派生条目不计独立数。
- 待确认：未披露图片张数；未逐母来源确认实测／仿真属性，因此来源类型保留未披露。；不将二值前景掩膜映射为 void 掩膜。

### GPR010 — Low-Frequency Ground Penetrating Radar (GPR) Dataset Acquired via Ground-Based and UAV Platforms

- 分类：地下空洞及岩土；C；现场实测。依据：正文未说明空洞或结构缺陷真值；仅可作为信号、定位与采集域迁移的辅助候选。
- 页面：已核验：已读取官方正文。
- 文件：已核验：官方文件列表；未验证文件传输。
- 抽样下载：未执行。
- 体积口径：27.9 MB（含示意图）；Site_1/2/3.zip 分别 12.4/3.6/5.2 MB；官方顶层文件列表显示值。
- 独立性：计入：一手发布的独立来源；未见来源声明的派生关系；未做跨库文件哈希或采集批次比对。
- 一手依据（2026-09-19）：[https://zenodo.org/records/18769571](https://zenodo.org/records/18769571) — 3 个场地，地面推车与 UAV 同测线低频 GPR；原始 SEG-Y／GeoTable，三个站点 ZIP 及示意图片共 27.9 MB。
- 待确认：应在完整场地层面划分，不能把同场地空中／地面信号未经检查分入训练与测试。；subsoil risk assessment 项目用途不能证明数据实际含空洞。

### GPR011 — TIGPR: A Multi-View Ground Penetrating Radar Detection Data for Damage Assessment of Transportation Infrastructure

- 分类：多场景；道路及路面；桥梁及桥面板；隧道及地下衬砌；机场道面；A；现场实测。依据：官方数据页明确列出 voids 和 interlayer debonding；不将裂缝和松散区等同于空洞。
- 页面：已核验：已读取官方正文。
- 文件：已核验：官方文件列表；未验证文件传输。
- 抽样下载：未执行。
- 体积口径：TIGPR.rar 283 MB；Download All 278 MB；官方文件及打包显示值；不推算图片数。
- 独立性：计入：一手发布的独立来源；未见来源声明的派生关系；未做跨库文件哈希或采集批次比对。
- 一手依据（2026-09-19）：[https://data.mendeley.com/datasets/ckgvrft232/1](https://data.mendeley.com/datasets/ckgvrft232/1) — 交通基础设施多视图缺陷图片；2D B-scan 200×200，3D 派生 B/C-scan 320×320；RAR 283 MB；张数未披露。
- 待确认：论文 URL 由检索命中，正文未核验。；机场被作者纳入数据范围，但描述的实际采集清单未单独列机场；不可声称机场子集规模已验证。；多场景只计一个独立来源；未确认与其他 3D-GPR 项目的采集批次重叠情况。

### GPR012 — GPR Subsurface Diagnosis (GPR-SD)

- 分类：道路及路面；C；现场实测。依据：README 仅明确 subsurface targets 和粗位置标记；未明确空洞或介质异常类别，保守列 C，不能根据名称 diagnosis 自动升为 A/B。
- 页面：已核验：已读取官方正文。
- 文件：已核验：GitHub Contents API 给出 33 个分卷的文件名与字节数、Mark.xlsx、Introduce.txt、README.md；未解压。
- 抽样下载：未执行。
- 体积口径：680128689 bytes；GitHub Contents API：32 个 20971520 bytes 分卷加末卷 9040049 bytes；不含说明与 Mark.xlsx。
- 独立性：计入：一手发布的独立来源；未见来源声明的派生关系；未做跨库文件哈希或采集批次比对。
- 一手依据（2026-09-19）：[https://github.com/ubriustc/GPR_data/blob/main/README.md](https://github.com/ubriustc/GPR_data/blob/main/README.md) — 明确 3 cm、380 点、97 ns、MATGPR 去地表回波与增益，以及 coarse locations。
- 一手依据（2026-09-19）：[https://api.github.com/repos/ubriustc/GPR_data/contents/](https://api.github.com/repos/ubriustc/GPR_data/contents/) — 33 个分卷已核验文件级大小；未下载压缩数据。
- 待确认：未读取 Mark.xlsx 标签内容；不声称有明确空洞标签。；处理后幅值会影响响应相似边，需要保留处理版本并检查增益一致性。

### GPR013 — Ground Penetrating Radar (GPR) Corrosion Data (Wong, 2023)

- 分类：混凝土构件；A；混合。依据：作者逐组描述中 HKM_C1 与 NP_D 明确为 field marine structure, delamination。混合指现场与实验室实测混合，不含已证实仿真。
- 页面：已核验：已读取官方正文。
- 文件：已核验：官方文件列表；未验证文件传输。
- 抽样下载：已发起小型 XLSX 下载；中断前工具未返回保存路径或可读文件结果，完成状态待核验；不计成功下载。
- 体积口径：626 KB；Download All 609 KB；单 XLSX 与平台打包显示值。
- 独立性：计入：一手发布的独立来源；未见来源声明的派生关系；未做跨库文件哈希或采集批次比对。
- 一手依据（2026-09-19）：[https://data.mendeley.com/datasets/wbdr5pdxbd/1](https://data.mendeley.com/datasets/wbdr5pdxbd/1) — 实验试件与现场海工混凝土状态数据；含 HKM_C1、NP_D 脱层，其他裂缝／腐蚀／渗水／完好条件；XLSX 626 KB。
- 待确认：Phase 3 不是纯脱层类，必须按原始条件筛选，不把所有腐蚀样本映射为 void。；未核验行数、样本量与逐道空间关系。

### GPR014 — Railway_GPR_Interface_Detectability

- 分类：铁路及路基；B；混合。依据：作者明确研究含水率、衰减与界面可检测性；没有空洞标签，可作为介质响应辅助研究。
- 页面：已核验：已读取官方正文。
- 文件：已核验：递归GitHub文件树 truncated=false；20 TXT、20 OUT、20 IN及配套文件。。
- 抽样下载：已验证：通过GitHub连接器完整读取1个14102-byte实验TXT并检查512行时间—幅值数据；另读取717-byte IN及LICENSE。未下载OUT或全部数据。。
- 体积口径：抽样 TXT 14102 bytes；单个 OUT 52060 bytes；GitHub 文件树逐项值，非全库体积。
- 独立性：计入：一手发布的独立来源；未见来源声明的派生关系；未做跨库文件哈希或采集批次比对。
- 一手依据（2026-09-20）：[https://github.com/Sepideh-Harajchi/Railway_GPR_Interface_Detectability](https://github.com/Sepideh-Harajchi/Railway_GPR_Interface_Detectability) — README明确laboratory与gprMax；递归树核实实验及数值文件。
- 一手依据（2026-09-20）：[https://github.com/Sepideh-Harajchi/Railway_GPR_Interface_Detectability/blob/main/03_experimental_results/Dry/TESTTUDELFT__011_Ascan.txt](https://github.com/Sepideh-Harajchi/Railway_GPR_Interface_Detectability/blob/main/03_experimental_results/Dry/TESTTUDELFT__011_Ascan.txt) — 全文读取：512行time_ns amplitude；头部明确average of central traces, indices49 and50。文件blob SHA ae721a921693d670771837653396a01e2724b88c。
- 一手依据（2026-09-20）：[https://github.com/Sepideh-Harajchi/Railway_GPR_Interface_Detectability/blob/main/LICENSE](https://github.com/Sepideh-Harajchi/Railway_GPR_Interface_Detectability/blob/main/LICENSE) — MIT License，Copyright(c)2026 Sepideh Harajchi。
- 待确认：不含空洞真值，不作为A类。；抽样IN引用作者本机几何文件路径；完整几何依赖可用性未验证，不保证可直接复现。；同作者现场铁路项目另列候选，实验室与现场场景不同；未做跨库哈希检查。

### GPR015 — TunGPR

- 分类：隧道及地下衬砌；A；数值仿真。依据：作者数据说明明确列出D/Vd/Vs/Cd/Cs物理缺陷类别；下载归档已公开显示，内部缺陷文件尚未完整核验。
- 页面：已核验：已读取官方正文。
- 文件：部分核验：两个作者Google Drive入口匿名显示Tunnel lining.zip、Hyperbolic feature.zip与下载按钮；前者预览仅见R目录，后者因文件过大无法预览；R标注补包未打开。。
- 抽样下载：未执行。
- 体积口径：未披露；未披露。
- 独立性：计入：一手发布的独立来源；Part I/II与537图像子集、R标注补包合为同一数据来源；内部模型重叠尚未哈希检查。。
- 一手依据（2026-09-20）：[https://github.com/LCA-Asset/TunGPR](https://github.com/LCA-Asset/TunGPR) — README全文：synthetic data、六类缺陷、模型与原始OUT、采样参数和两个数据部分；图像经过resize。
- 一手依据（2026-09-20）：[https://drive.google.com/file/d/1OojzmbI5tDJrUtShyAYzcVTZc-lHmTLN/view](https://drive.google.com/file/d/1OojzmbI5tDJrUtShyAYzcVTZc-lHmTLN/view) — 匿名查看归档Tunnel lining.zip，预览仅1个R文件夹，未证实其它缺陷文件是否齐全。
- 一手依据（2026-09-20）：[https://drive.google.com/file/d/10Y3EEOUUtwHZY1K41uZUN3NDbQn4_uXe/view](https://drive.google.com/file/d/10Y3EEOUUtwHZY1K41uZUN3NDbQn4_uXe/view) — 匿名查看Hyperbolic feature.zip及下载按钮；too large to preview，未下载。
- 待确认：A类依据作者正式数据说明，不能据此声称所有缺陷文件均已验证。；Part I预览范围与README六类范围不一致，需解包核对；Part II不支持在线预览。；许可证未明确；R标注补包及全部原始输出仍待检查。

## 文档一致性与远程状态

目录由同一结构化记录生成 CSV、JSON 和 README 表格；已进行字段顺序、CSV/JSON无损一致、ID唯一、来源统计、派生排除、README条目覆盖、相对链接存在和待提交文件范围检查。自动检查不等于对未下载原始数据进行了内容验证。

目标为公开仓库 [GenLicdu/GPR-Void-Resources](https://github.com/GenLicdu/GPR-Void-Resources)。仓库已创建；提交采用GitHub授权连接器的标准Git树、提交及非强制分支更新。发布是否完成以远程main及实际文件为准；核验说明不将本地文件生成视为上传成功。
