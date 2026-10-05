# 伦敦房产策略图谱（London Property Strategy Atlas）

> **👉 在线网页：https://icebbay.github.io/london-strategy-atlas/**
> （本仓库是源文件；点击上面的链接直接打开网页版地图和分析。）


一个独立的单页文件（`index.html`），汇总了对 Draft London Plan 2026（伦敦规划草案）、TfL 交通连接与客流需求、房价以及三种房产投资策略的研究。用任何现代浏览器打开 `index.html` 即可。仅地图库（来自 cdnjs 的 d3）和字体需要联网加载。

## 三大策略

| | 策略 1：非核心区捡漏、翻新、出售 | 策略 2：核心区捡漏、翻新、出售 | 策略 3：长期持有出租 |
|---|---|---|---|
| 范围 | 任何票价区，非核心地段 | 房价前 10%（中位价 ≥ £1.53m） | 仅限房屋（不含公寓），1–3 区 |
| 必须满足 | London Plan 未来增长评分 ≥ 0.3；翻新后退出价 ≤ 当地家庭收入的 10 倍；总成本利润率 15% | 总成本利润率 15%；挂牌价低于当地每平方英尺价格及成交中位价 | London Plan 未来增长评分 ≥ 0.3；全成本净收益率 ≥ 5%；再融资后现金流为正 |
| 市场装修成本 | £100/平方英尺 | £200/平方英尺 | £70/平方英尺 + £10k EPC |

## 页面内容

1. **三大策略**：规则、结论和市场成本假设。
2. **推荐交易（2026 年 10 月）**：在售房源，以及仍能满足各策略门槛的最高出价。
3. **交易筛选**：206 套 Rightmove 房源经成本模型测算（SDLT 按额外住宅税率、各项费用、融资、装修成本、退出价值）。
4. **按策略划分的目标区域**：社区短名单。
5. **修正说明**：研究过程中被修正的早期结论。
6. **研究地图**：行政区（borough）和社区图层。包括 London Plan 机会区（Opportunity Areas）、城镇中心升级、增长区位、CAZ 及其 3 公里环、工业用地及释放地块、考古优先区、保护区、受保护视廊、Superloop、TfL 车站客流与季节性、房价走势，以及扩建地块核查工具。
7. **实证**：过往交通项目、大型开发和城镇中心设施对房价的影响（1995–2025）、市场核查、交通项目、各板块优劣、机会区排名表。

## 数据工作簿（`data/`）

| 文件 | 内容 |
|---|---|
| `shortlist_market_costs.xlsx` | 交易筛选结果、接近达标的翻新转售标的、出租候选房源、假设 |
| `deal_profit_with_capex.xlsx` | 交易测算示例及敏感性分析 |
| `three_strategies.xlsx` | 各策略及方法下的社区短名单 |
| `near_station_houses.xlsx` | 目标车站 0.2 英里内的房屋：车站汇总（公开版本已删除单笔成交记录） |
| `prime_near_station_houses.xlsx` | 核心区车站的同类数据，另含核心区社区指标 |
| `TfL_station_monthly_entry_exit.xlsx` | 各车站每月进出站刷卡量，2019 年 1 月至 2026 年 9 月 |

## 数据来源

- **规划**：Draft London Plan 2026（GLA）；London Datastore（CAZ、城镇中心、SIL、LVMF）；planning.data.gov.uk（考古优先区、保护区、Article 4、列名建筑、洪水区）。
- **交通**：TfL 2026 Business Plan；Mayor's Transport Strategy 2025/26 年度实施报告；TfL Network Demand 开放数据；TfL StopPoint API；DfT NaPTAN。
- **价格与人口**：HM Land Registry Price Paid Data（2019 年至 2026 年 8 月）；ONS 小区域房价统计；ONS Price Index of Private Rents（2026 年 8 月）；ONS 小区域收入估算（FYE2023）；2021 年人口普查（Census 2021，Nomis）；ONS 小区域人口估算。
- **在售房源**：2026 年 10 月 5 日查阅的 Rightmove 房源。

Contains HM Land Registry data © Crown copyright and database right 2026. Contains OS data © Crown copyright 2026. Contains public sector information licensed under the Open Government Licence v3.0.

（以上为数据许可要求的英文版权声明：包含 HM Land Registry 数据 © Crown copyright and database right 2026；包含 OS 数据 © Crown copyright 2026；包含依据 Open Government Licence v3.0 授权的公共部门信息。）

## 局限性

- **地图精度**：机会区点位和交通线路为手工标注，仅为大致位置。
- **数据时效**：PTAL 为 2015 年数据，早于 Elizabeth line 开通。
- **样本较小**：部分区域的转售成交数量很少。
- **估算输入**：房源未标明面积时按卧室数估算。每平方英尺挂牌价取自当前在售房源，而非成交价。
- **假设**：成本、融资和租金假设为市场中档估算，并非报价。
- **非投资建议**：本工具仅用于筛选，不构成投资、税务或法律建议。SDLT 和持有架构会显著改变结果。
