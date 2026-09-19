# 待获取与待核验线索

以下 **19 条**是17条待获取／待核验线索与2条关联代码交叉引用，不是19个独立数据集。L13、L14为主目录已计来源的代码／存档交叉引用；其余17条尚未满足本轮主目录的“来源与文件入口均已核验”条件，或访问受限、证据不足、仅有论文／代码。全部不增加主目录独立数。线索状态描述的是当前核验结果，不推断未来能否获得。

原L01（TunGPR）已提升为GPR015，原L08已提升为GPR014；不再保留为待获取线索，原线索编号空缺有意保留。

L12在规定的开放状态枚举中归入“仅论文描述”桶，实际资源类型明确为软件；L13/L14的“公开下载”仅指关联代码，而非新增公开数据。搜索片段线索保留“待核验”，不擅自断言仅论文或申请访问。

## L02 — Open GPR Dataset for Bridge Deck

- 官方／候选入口：[https://github.com/InfraSmartLab/Open_GPR_Dataset_for_Bridge_Deck](https://github.com/InfraSmartLab/Open_GPR_Dataset_for_Bridge_Deck)
- 场景：桥梁及桥面板；相关性：C；开放状态：申请访问。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：作者 README：20000 simulated GPR scans，用 gprMax 生成钢筋双曲线，含增强，Labelme 框；通过表单验证后提供；仅学术研究、禁商用。不是脱层数据。
- 下一步：用户自行决定是否申请；本次不提交表单，不计公开数据。

## L03 — multi-view-3DGPR

- 官方／候选入口：[https://github.com/zhouchunpong/multi-view-3DGPR](https://github.com/zhouchunpong/multi-view-3DGPR)
- 场景：道路及路面；相关性：待核验；开放状态：链接失效。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：作者 README 首句明确：For security reasons, we remove the open access to the dataset。保留更早 2024 开放说明不代表当前仍开放。论文 https://arxiv.org/abs/2308.04779。
- 下一步：向作者确认合法获取方式、缺陷标签及与 TIGPR 的采集批次关系。这里“链接失效”指作者撤回公开入口，不是对服务器永久不可达的判断。

## L04 — Multimodal GPR-CHD Dataset

- 官方／候选入口：[https://github.com/BingxinYang/Multimodal-GPR-CHD-Dataset](https://github.com/BingxinYang/Multimodal-GPR-CHD-Dataset)
- 场景：道路及路面；相关性：A（描述中的 void；数据不完整）；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：README 声称50张640×640图片（19 crack、31 void）及文字标注；但实际根目录只有 annotations.jsonl、dataset_summary.json、checksums_sha256.txt、说明等，没有 README 声称的 B-scan-image 目录。原始数据受道路主管部门隐私协议限制。
- 下一步：核验缺失图片是否另行发布及许可。仅文字标注不能作为完整 GPR 图像数据；不计独立公开数据。

## L05 — GPR-rebar-signal-suppression-and-defect-recognition-dataset

- 官方／候选入口：[https://github.com/yyj2518/GPR-rebar-signal-suppression-and-defect-recognition-dataset](https://github.com/yyj2518/GPR-rebar-signal-suppression-and-defect-recognition-dataset)
- 场景：混凝土构件；相关性：待核验；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：GitHub 根目录可见 data_withrebar 和 label；README.md 返回404。尚未读文件、标签或采集描述，不能根据仓库名断言 void。
- 下一步：读取目录、样本及对应论文，确认来源、格式、标签与许可。

## L06 — EMIT-GPR

- 官方／候选入口：[https://github.com/fangzhengXJTU/EMIT-GPR](https://github.com/fangzhengXJTU/EMIT-GPR)
- 场景：待核验；相关性：待核验；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：根目录可见 EMIT-GPR-voc-10000.zip，25921983 bytes，与 LICENSE；README.md 返回404。10000只是文件名的一部分，未核实样本数量或目标。
- 下一步：核验原始论文、文件内容、标签、来源及 LICENSE；不凭命名列成一万个脱空样本。

## L07 — GPR-echo-amplitude-matrix

- 官方／候选入口：[https://github.com/Zhousr-code/GPR-echo-amplitude-matrix](https://github.com/Zhousr-code/GPR-echo-amplitude-matrix)
- 场景：隧道及地下衬砌；相关性：A（研究主题）；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：作者 README 说明 RMS、ROI、形态学及轻量分类的隧道脱空方法，称 field/simulation/physical-model validation；仅此说明未确认数据发布。
- 下一步：检查是否真正发布幅值矩阵、采样位置、数据许可；不能将方法描述计成数据集。

## L09 — Optimizing_GPR_Acquisition_Geometry

- 官方／候选入口：[https://github.com/Sepideh-Harajchi/Optimizing_GPR_Acquisition_Geometry](https://github.com/Sepideh-Harajchi/Optimizing_GPR_Acquisition_Geometry)
- 场景：铁路及路基；相关性：C（界面背景／属性研究候选）；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：README：荷兰 Delft–Schiedam 铁路约200 m，7组×3高度共21条纵向测线；GSSI SIR4000/400 MHz；提供提取属性 XLSX、图件及岩土验证，未明确发布原始逐道 GPR。2026-09-20已核验递归文件树：3个GPR属性XLSX（66167、23473、10699 bytes），2个CPT CSV、钻孔XLSX及图件；未见完整原始GPR矩阵。
- 下一步：核实原始波形是否存在、文件和许可；与 GPR014 同作者不等于同数据，需对比场地／采集批次；暂不独立计数。

## L10 — Raw GPR Experimental Data for the Kashgar Cavity in Xinjiang

- 官方／候选入口：[https://figshare.com/s/d56b2eb967ab5e18fa94](https://figshare.com/s/d56b2eb967ab5e18fa94)
- 场景：地下空洞及岩土；相关性：A（现场描述已核验）；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：已读 Figshare 页面：明确可直接观察的近地表 cavity、现场 GPR；9文件61.49 kB，GPS/KML/TXT/MAT等。但页面明确 This item is shared privately，下载地址带 private_link，未显示正式公开 DOI/作者。CC BY 4.0 标示。
- 下一步：取得正式公开落地页／作者确认后再计入；不把可在搜索中发现的私有分享当作稳定公开数据，不再公布带 private_link 的文件直链。

## L11 — URDD: An open dataset for urban roadway disease detection and classification（题名后半待全文核验）

- 官方／候选入口：[https://www.sciencedirect.com/science/article/pii/S2352340925002318](https://www.sciencedirect.com/science/article/pii/S2352340925002318)
- 场景：道路及路面；相关性：待核验；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：搜索结果指向该论文；作者衍生软件 README 引用 URDD 论文 DOI 10.1016/j.dib.2025.111499。ScienceDirect 打开后遇机器人验证，未读取正文、Data Availability 或原始数据入口。
- 下一步：恢复联网后通过官方仓库或论文数据声明找到原始 URDD；DURDD/CURDD 若同来源不能直接拆成两个独立数据集。

## L12 — Road cavity detection from GPR data using deep learning

- 官方／候选入口：[https://zenodo.org/records/18301084](https://zenodo.org/records/18301084)
- 场景：道路及路面；相关性：A（主题）；开放状态：仅论文描述。
- 已在主目录出现：否；parent_dataset：URDD（模型训练来源；不是已确认派生数据包）；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：已读 Zenodo：Resource type Software，201.8 MB归档；GitHub README 显示 YOLO 模型、GAN、仿真代码进度，并引用 URDD。不能将权重文件大小写成 GPR 数据规模。
- 下一步：当前作为软件／原始数据追踪线索；检查 https://github.com/ahmed-elseicy/GPR_Road_Cavity_Detection 。未确认另有可用数据，归入“仅论文描述”桶并明确实际资源类型为软件。

## L13 — Deep learning model for delamination detection from GPR data

- 官方／候选入口：[https://zenodo.org/records/14607117](https://zenodo.org/records/14607117)
- 场景：桥梁及桥面板；相关性：A（主题；非独立数据集）；开放状态：公开下载。
- 已在主目录出现：是：GPR001 的关联软件；parent_dataset：GPR001；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：已读取19.4 MB软件 ZIP 列表，内容为转换脚本和模型权重；原始数据明确指向 SDNET2021。对应 https://github.com/ahmed-elseicy/bridge-deck-delamination 。
- 下一步：无需另行计数；若使用转换输出，应保留 GPR001 与原始信号映射。

## L14 — LCSkhalid/GPR_Data

- 官方／候选入口：[https://github.com/LCSkhalid/GPR_Data](https://github.com/LCSkhalid/GPR_Data)
- 场景：地下空洞及岩土／管线周边；相关性：A；开放状态：公开下载。
- 已在主目录出现：是：GPR004 的关联代码；parent_dataset：GPR004；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：已读 README 和目录；下载链接指向 ww7fd9t325/1；仓库是说明、裁剪增强脚本和示意图。
- 下一步：与 GPR004 合并；后续核验原图—裁剪—增强映射。

## L15 — FKS-GPR / An Automated Method for Identifying Voids and Severe Loosening in …

- 官方／候选入口：[https://www.mdpi.com/2313-433X/11/8/255](https://www.mdpi.com/2313-433X/11/8/255)
- 场景：道路及路面；相关性：待核验；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：搜索片段出现 FKS-GPR 与道路 void/severe loosening；未读论文正文或数据声明，未确认正式数据名称、规模、访问方式。
- 下一步：核验正文与数据可用性声明；void 与 severe loosening 分开保留。

## L16 — A GPR Imagery-Based Real-Time Algorithm for Tunnel Lining Void …

- 官方／候选入口：[https://www.mdpi.com/2075-5309/15/18/3323](https://www.mdpi.com/2075-5309/15/18/3323)
- 场景：隧道及地下衬砌；相关性：待核验；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：搜索片段称运营重载铁路隧道624张图片；未读正文／数据声明，不把搜索片段数字计入已核验规模。
- 下一步：核验是否公开图片、原始波形与采集批次；铁路隧道仍分类为隧道衬砌，不等于铁路路基。

## L17 — Radar Database Collected over Artificial Debonding Pavement …

- 官方／候选入口：[https://link.springer.com/content/pdf/10.1007/978-3-030-55236-7_65.pdf](https://link.springer.com/content/pdf/10.1007/978-3-030-55236-7_65.pdf)
- 场景：道路及路面；相关性：待核验；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：检索片段显示 tack-free/geotextile/sand-based 人工脱粘；仅找到出版物入口，未读全文、未找到已验证数据下载。
- 下一步：追踪作者机构的原始雷达库及许可；不同人工界面不能当成同一物理标签。

## L18 — Highway GPR DATASETS

- 官方／候选入口：[https://data.mendeley.com/datasets/dc7g2pvn86/1](https://data.mendeley.com/datasets/dc7g2pvn86/1)
- 场景：道路及路面；相关性：C（初筛）；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：Mendeley 自身检索页给出作者 muwei ning、2020-07-09，描述仅为 highway layer-interface GPR profiles；尚未打开数据详情与文件列表。
- 下一步：核验文件、独立来源、标签及许可；当前无空洞证据，只能作为层界面背景候选。

## L19 — Ground Penetrating Radar measures from quarries

- 官方／候选入口：[https://data.mendeley.com/datasets/w26n6nftxs](https://data.mendeley.com/datasets/w26n6nftxs)
- 场景：地下空洞及岩土；相关性：B（初筛）；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：平台检索页描述意大利 Botticino 与罗马尼亚 Ruschita/Carpinis/Pietroasa 四采石场，双正交方向 GPR 与位置，用于裂隙和不连续面。未读详情与文件列表。
- 下一步：核验实际文件、采样头和许可；裂隙／不连续面不能直接称空洞。

## L20 — Data for: Evaluating the structure characteristics of epikarst at a typical peak cluster depression in Guizhou plateau area using ground penetrating radar attributes

- 官方／候选入口：[https://data.mendeley.com/datasets/9ch6ky5xf6](https://data.mendeley.com/datasets/9ch6ky5xf6)
- 场景：地下空洞及岩土；相关性：待核验；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：平台检索页列 Tao Peng、Qiangshan Gao、2021-04-27；称 ZIP 可由 Reflexw 读取。表层岩溶不等于已证实空洞标签。
- 下一步：核验详情、标签、文件、原始数值与场地位置；未确认前不计独立资源。

## L21 — highway gpr data

- 官方／候选入口：[https://ieee-dataport.org/documents/highway-gpr-data](https://ieee-dataport.org/documents/highway-gpr-data)
- 场景：道路及路面；相关性：待核验；开放状态：待核验。
- 已在主目录出现：否；parent_dataset：未披露；独立计数：不计入。
- 已核验及证据边界（2026-09-19；补核另注明）：Bing 命中 IEEE DataPort；片段提及 institutional subscribers，但该字样涉及 AI intelligence 功能，不能据此推定数据下载付费。未进入详情核验。
- 下一步：检查数据本身开放／注册／申请条件、具体目标、是否与 Mendeley Highway GPR 重叠，不绕过登录或付费。

