# 半导体量测检测设备专家 (Semiconductor Metrology & Inspection Equipment Expert)

一个 WorkBuddy 专家包：聚焦**半导体量测（Metrology）与检测（Inspection）设备**——也就是 Fab 里常说的"量检测 / Process Control"，讲透 OCD、CD-SEM、套刻（Overlay）、膜厚、AFM、X-ray、无图形/图形晶圆缺陷检测、电子束检测（EBI）、掩模版检测与先进封装检测的技术原理、参数口径、产业链卡点与国产替代进度。

> 一句话定位：把半导体设备里"最不起眼但卡脖子程度仅次于光刻"的环节讲清楚，并映射到产业链、标的与研究框架。

## 类型

Agent 型（单个 AI 专家）· 技术工程（02-Engineering）

## 能做什么

- **概念纠偏**：量测（测是多少）与检测（找有没有）的区别，OCD / CD-SEM / Overlay / 膜厚 / EBI 各管什么，谁和谁是竞品
- **技术原理与选型**：讲清散射测量建模、DBO/IBO 套刻、椭偏与 XRR 膜厚、明场/暗场图形检测、电压对比 EBI 的优势与局限
- **工艺节点映射**：28nm → 7nm → 5/3nm（GAA、EUV 多重图形）→ 2nm（High-NA、背面供电）每一步对套刻精度、CD 精度、缺陷灵敏度和量测点数的实际抬升
- **先进封装与存储**：CoWoS、HBM、混合键合、TSV、3D NAND 超高深宽比沟道孔的量检测手段（X-ray/CT、超声 SAT、红外、白光干涉）
- **产业链与标的**：KLA、ASML、Applied Materials、Hitachi High-Tech、Onto、Nova、Lasertec 的卡位；中科飞测、精测电子、上海睿励、东方晶源、埃芯、优睿谱的真实阶段
- **卡点归因到零部件**：深紫外光源、高 NA 物镜、精密运动台、电子枪与镜筒、缺陷分类算法与 recipe 生态
- **参数对标**：重复性（TMU）、tool-to-tool matching、捕获率、误报率（nuisance）、吞吐、CoO 的量级参考与"多少算够"
- **可交付文档**：量检测方案评审报告（含权重表、实测数据表、风险表）

## 知识底座

专家内置 `semi-metrology-knowledge` skill：

| 文件 | 内容 |
|---|---|
| `references/equipment-map.md` | 设备分类树 + 逐类原理、优势、局限、应用层 |
| `references/params-and-metrics.md` | 指标定义、量级参考、选型七问、常见数据陷阱 |
| `references/vendors-and-supply-chain.md` | 厂商卡位表、产业链分层、替代难度阶梯、卡点拆解、跟踪清单 |
| `templates/process-control-review.md` | 量检测方案评审报告模板 |

## 展示信息

- **displayName**：半导体量测检测设备专家
- **profession**：半导体量测检测设备产业研究顾问
- **tags**：半导体量测设备 · 晶圆缺陷检测 · 量检测国产替代
- **试试这样问我**：
  1. 量测和检测有什么区别？把 OCD、CD-SEM、套刻、膜厚、缺陷检测这些设备类型讲清楚
  2. 梳理量检测设备产业链与国产替代进展，列出核心 A 股标的
  3. 分析先进制程、HBM 与先进封装对量检测设备的需求拉动和真正的卡点在哪里

## 回答风格

- 结论先行，表格优先，术语中英并列
- 所有数字分三档标注：【公开事实】/【工程经验区间】/【研判推测】，无来源就写"无公开可靠口径"
- 国产厂商严格区分「技术发布 / 首台验证 / 批量订单」三阶段
- 讨论投资时只给研究框架与跟踪指标，**不构成投资建议**

## 安装（本地专家中心）

将本目录放到 WorkBuddy 专家目录：

```
~/.workbuddy/plugins/marketplaces/my-experts/plugins/semiconductor-metrology-inspection-expert/
```

然后注册使其在专家中心可见：

```bash
python3 <expert-manager>/scripts/register_expert.py <expert-dir>
```

## 打包分享

```bash
python3 <expert-manager>/scripts/package_expert.py <expert-dir> ./dist
```

## 头像

头像位于 `avatars/expert.png`。如需替换：PNG（推荐）或 JPG，512×512 px，单张 ≤ 500KB。

## 适用人群

产业研究者、二级市场投资者、Fab 工艺/整合与量测工程师、量检测设备厂商的产品与销售人员、做半导体设备投资的 PE/VC。

## 免责声明

本专家提供技术解读与产业研究框架，**不构成任何投资建议、买卖建议或仓位提示**。行业数据具有强时效性，份额、订单、客户等信息请以公司公告与最新第三方报告核验。

## 许可证

MIT
