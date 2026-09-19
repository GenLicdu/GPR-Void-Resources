# 优先数据资源与使用前核查

以下8个资源按研究需要推荐；是基于来源证据的选型判断，不是质量评分或已验证实验结论。名称链接指官方入口，完整参数和核验层级见[主目录JSON](../data/dataset_catalog.json)。除GPR014的小型TXT外，均未成功验证数据文件下载；不能把本表当作即取即用承诺。

| ID／资源 | 优先用途与依据 | 使用前必须解决 |
|---|---|---|
| GPR001 [SDNET2021](https://commons.und.edu/data/19/) | A类现场桥面板；信号级脱层类别、5座桥与位置／真值资源，对跨结构实验和A-scan表示学习最有价值 | 核实真实GPR格式、时间轴、信号与测点映射；不能把官方signals自动解释为精确原始A-scan数量；许可未明确 |
| GPR015 [TunGPR](https://github.com/LCA-Asset/TunGPR) | A类隧道仿真；明确空洞／脱层类别，作者声明原始OUT与几何、物性输入，道间距已说明；适合受控双关系实验 | 第一归档预览仅R，第二过大无法预览；先核齐实际缺陷文件、OUT采样头、补标注及许可；不要用缩放PNG恢复幅值 |
| GPR007 [MERL-GPR](https://zenodo.org/records/8145084) | A类空气圆柱仿真；400模型、H5／NPY频域数据及源系数，可研究受控逆散射／表征 | 有限50频点不等于完整原始时域A-scan；标签应来自模型；CC BY-SA4条款及模型／权重体积分别处理 |
| GPR006 [S&T Project21045 Void Detection Data](https://data.usbr.gov/catalog/8078/item/128829) | A类现场水工结构，多个试验位置与多模态资料，为交通场景外验证提供候选 | 先核对ZIP内部的GPR占比、波形、真值和测线；体积、许可与采样参数未披露 |
| GPR011 [TIGPR](https://data.mendeley.com/datasets/ckgvrft232/1) | A类实测交通多场景，含裂缝、界面脱粘、松散及空洞，适合先做图像缺陷迁移 | 不假定B/C图像能恢复原始3D波形；核实每类及场景样本量、标签、场地划分与相邻图重叠；CC BY4 |
| GPR004 [Intelligent recognition of subsurface utilities and voids](https://data.mendeley.com/datasets/ww7fd9t325/1) | A类现场地下空洞／设施，明确553空洞、786管线、900完好处理／增强图；可作图像级初始实验 | 2239图像不是2239独立测线；追溯原始profiles及增强父图；不用于未经确认的原始幅值建模；CC BY4 |
| GPR013 [Ground Penetrating Radar (GPR) Corrosion Data (Wong,2023)](https://data.mendeley.com/datasets/wbdr5pdxbd/1) | A类混合实验与现场，HKM_C1、NP_D明确含delamination；626KB表格便于先审读数值字段 | 腐蚀、裂缝、脱层共存要分开标签；下载尝试完成未确认；先判断XLSX保存完整波形还是指标、位置映射；CC BY4 |
| GPR014 [Railway_GPR_Interface_Detectability](https://github.com/Sepideh-Harajchi/Railway_GPR_Interface_Detectability) | B类铁路辅助；小型TXT已读取512行时间／幅值，20种含水／高度条件配套实验和仿真 | TXT为中心两道平均，不能重建完整空间图；实验与仿真分开评价；仿真几何依赖及MIT对数据适用范围待确认 |

如果首要目标必须是同一组完整实测A-scan的空间邻近图与响应相似图，应先核验SDNET2021，再考虑C类原始GPR DATASET或处理后GPR-SD作为辅助。后两者暂无确证空洞标签，不可用作有监督脱空性能的直接证据。GPR003复合衬砌虽然直接相关，但公开雷达主要在DOCX中，TLS点云不等于3D GPR，故不列为原始信号优先项。
