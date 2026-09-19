# 检索记录与覆盖边界

检索与核验于2026-09-19至2026-09-20完成本轮整理。目标30–50个独立数据来源，实际确认14个，直接相关A类9个；没有为数量补入远离工程缺陷的冰川、考古资料。不宣称穷尽公开数据。

## 执行记录

| 日期 | 平台／方式 | 实际关键词或范围 | 结果及限制 |
|---|---|---|---|
| 09-19 | Bing，追踪原站 | GPR void dataset Mendeley Zenodo；GPR tunnel lining void dataset Zenodo Mendeley | 追踪衬砌、复合衬砌、TunGPR等原始入口；搜索摘要不替代数据核验 |
| 09-19 | Bing | GPR road pavement void dataset URDD Mendeley | FDM-HHT-SR、TIGPR、URDD线索；URDD出版社页面机器人验证，未绕过 |
| 09-19 | Bing | GPR railway airport debonding dataset | 铁路含水／界面辅助数据及道面脱粘论文；没有确认独立机场脱空文件子集 |
| 09-19 | Bing | GPR concrete delamination debonding dataset Figshare Zenodo | 桥面板、混凝土与钢筋实验需分级；钢筋检测不升级为A |
| 09-19 | Bing | GPR cavity dataset Dryad Figshare IEEE DataPort | Figshare喀什页面标私有分享，保留线索；未确认新的Dryad来源；DataPort实际下载条件待查 |
| 09-19 | GitHub仓库检索 | GPR dataset、void、cavity、delamination、tunnel、railway、airport、debonding、URDD | 初始GPR dataset检索约50个仓库结果，后续场景检索；读取作者README和实际目录，排除仅方法、权重和重复来源 |
| 09-19 | Mendeley平台自身搜索 | GPR；ground penetrating radar | GPR显示67项；后者1650项但匹配很宽，查看前3页；发现腐蚀、采石场、表层岩溶等；不是1650个合格数据集 |
| 09-19 | Zenodo、UND、USBR RISE、Data.gov原页 | 逐条打开用户14条初始线索与关联入口 | 记录资源类型、文件列表、规模及许可；政府聚合与原始条目合并；14条初始线索全部有处理结论 |
| 09-20 | GitHub API及Google Drive作者链接 | Railway_GPR_Interface_Detectability；TunGPR；Optimizing_GPR_Acquisition_Geometry | 核验铁路递归树并完整读取一个TXT样本；TunGPR两个匿名归档入口可见，内部列表仅部分；现场铁路属性表仍留候选 |
| 09-20 | Bing中文查询尝试 | 探地雷达 脱空 数据集 开源 隧道 道路 | 导航超时，未取得结果；中文检索覆盖不足，不声称已完成系统中文检索 |

原始核验链接及逐条证据见[核验记录](verification_notes.md)和[候选线索](candidate_leads.md)。论文补充材料／Data Availability追踪仅在实际页面可读时使用；遇到登录、付费或验证障碍不越过，不从摘要猜下载许可。

## 主要排除与纠错

1. GPR缩写可能指高斯过程回归或地缘政治风险；与雷达无关项排除。
2. 仿真软件、处理脚本、模型权重和论文不是数据集；SDNET代码及其Zenodo存档不新增数量。
3. MCG为多个父来源的裁剪／掩膜汇编；公开不等于独立。版本、增强与格式转换同样归并。
4. Mendeley条目997pwzvhgj只有Impact-Echo数据，虽论文题目提GPR仍未收入GPR主目录。
5. aquifer、coastal等一般地球物理资料未因开放而加入；采石场／岩溶仅保留尚待标签核验的线索。
6. 缺失图片、README与实际目录矛盾、作者撤销公开访问、私有分享或只有论文入口均单列。

## 尚存覆盖缺口

直接相关A类只有9个，距目标下限30差21个；全部独立来源距30差16个。铁路直接脱空、独立机场道面和管线周围回填缺陷来源仍不足；Dryad／IEEE DataPort与中文文献数据声明覆盖有限。若进一步补充，应优先追踪已有A类候选的正式数据入口和标签，避免增加大量通用目标数据。
