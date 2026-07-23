# 机场YYDS

**可核实的机场数据。** 不做「收录一百家」的清单，只保留能查到独立官网、能跑出实测数据的品牌。

主站 → **[www.jichangyyds.com](https://www.jichangyyds.com/)**

---

### 在做什么

维护一个机场（代理服务）品牌的**中央数据库**，并把其中可公开的部分开源出来。

市面上流传的机场清单动辄上百家，其中大量条目连独立官网都查不到。没有可核实的信息还要写评测，那是编。所以做了减法：

- **域名年限核实** —— 查注册日期，新注册域名单独标注
- **官网可达性探测** —— 打不开的直接剔除
- **工作日晚高峰实测** —— 21:00–22:00 采集，白天数据不算数
- **风险名单公开** —— 已跑路 / 有跑路前兆的品牌单独建档，不藏着

**列表长度不是质量，可核实性才是。**

---

### 开源数据仓库

| 仓库 | 内容 |
| --- | --- |
| [**jichang-tuijian**](https://github.com/jichangyyds/jichang-tuijian) | 精选 16 家机场，865 个节点晚高峰实测。含价格档位、线路类型、优惠码 |
| [**jichang-paolu-mingdan**](https://github.com/jichangyyds/jichang-paolu-mingdan) | 已确认停止运营的品牌存档，以及跑路前兆的识别方法 |

数据每次更新会同步回仓库，commit 记录即变更历史。

---

### 为什么只认晚高峰

白天带宽富余，任何机场都跑得好看。只有工作日 20:00–23:00 的表现才代表日常体验。

同理，选机场的顺序不要反：**先定预算档位 → 按用途挑线路 → 月付试一个晚高峰**。价格分层是带宽成本决定的，不存在「又便宜又是专线」这种事。别一上来就买年付。

| 档位 | 价格区间 | 典型线路 |
| --- | --- | --- |
| 低价走量 | ¥13 以内 | 公网直连 / 隧道中转 |
| 主流性价比 | ¥14 – 24 | 优质 BGP 中转、部分 CN2 |
| 专线高价 | ¥25 以上 | IPLC / IEPL 内网专线 |

---

### 常去的几页

[排行榜](https://www.jichangyyds.com/rank/) ·
[品牌库](https://www.jichangyyds.com/brands/) ·
[横向对比](https://www.jichangyyds.com/compare/) ·
[风险名单](https://www.jichangyyds.com/scam/) ·
[优惠码](https://www.jichangyyds.com/coupons/) ·
[上手教程](https://www.jichangyyds.com/guides/) ·
[报错排查](https://www.jichangyyds.com/troubleshoot/)

---

<sub>本仓库内容为公开信息整理与实测记录，仅供技术研究与选型参考。数据有时效性，以各服务商官网为准。</sub>
