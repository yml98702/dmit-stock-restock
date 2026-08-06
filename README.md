# DMIT库存：香港日本美国三地补货套餐年付低至$36.9起，CN2 GIA/CMIN2/国际BGP三网线路全收录

说起 DMIT，第一反应大概是"又双叒缺货了"。

这个靠 CN2 GIA 起家的小众 VPS 商家，过去两年主打一个"蹲到就是赚到"。你打开官网，想入个香港 CN2 GIA，结果一刷新——售罄；再刷新——还是售罄；多刷几次，干脆弹个 403。好在 2026 这一年 DMIT 偶尔会低调补几波货，香港、日本、美国洛杉矶三个机房轮流上库存，热门款基本是上架即被秒，冷门款能撑个几天。这篇文章就专门聊聊 DMIT 库存这件事：补货规律、当前在售套餐、三网线路区别，以及怎么第一时间抢到。

## **一、DMIT 为什么常年缺货**

DMIT 的缺货不是营销噱头，是真没货。它走的是"精品路线"——香港 Equinix HK2、东京、洛杉矶三个机房，硬件用 AMD EPYC 7003 / 9004 / 9005 三代平台，线路从 CN2 GIA、9929+CMIN2 到纯国际 BGP 全覆盖，客单价高、利润薄、配额少。热门的 Pro（Premium）系列走三网 CN2 GIA 回程，电信去程也走 CN2 GIA，联通走 AS9929/10099，移动走 CMI，延迟基本压在 15ms 以内（香港到深圳），丢包率低于 0.1%——这种线路资源本身就贵，DMIT 又不愿意敞开卖，所以一补货就秒空，正常。

再加上 AMD EPYC 9005 这种新平台产能有限，AN5 系列的 Pro 套餐（LAX.AN5.Pro.MINI / MICRO / MEDIUM）从年初到现在几乎没怎么开放过现货。库存流转最快的反而是低配 T1（Tier 1）国际线路款和性价比的 WEE 限量款，这两类是日常补货的主力。

## **二、当前在售 / 近期补货套餐速览**

DMIT 三个机房的补货节奏完全不同，我把近期出现过现货的套餐按机房整理了一遍，方便你对照入手。

### **香港机房（HKG）**

香港是 DMIT 老牌节点，Equinix HK2 机房，提供 T1（国际 BGP）、Pro（CN2 GIA）、EB（CMI）三种线路。

- **HKG.AS3.T1.WEE**：1 核 / 1GB / 20GB SSD / 1TB@4Gbps，年付 **$36.9**。流量超出后限速 50Mbps 不断线，纯国际线路，适合海外业务、外贸应用，不适合建站或服务国内。测试 IP：154.12.176.28。
- **HKG.AS3.Pro.TINY**：1 核 / 1GB / 20GB / 500GB@1Gbps，月付 **$39.9**。三网回程 CN2 GIA，电信去程 CN2 GIA，联通走 4837 + AS10099，移动走 CMI。测试 IP：103.117.100.199。
- **HKG.AS3.EB.TINY**：1 核 / 1GB / 20GB / 1TB@1Gbps，月付 **$29.9**。回程三网走 CMI，移动用户体验最好，电信联通也够用，价格友好库存相对充足。

### **日本机房（TYO）**

日本机房主打 Premium 和 Tier 1 两条线，EB 系列已下架。Premium 走三网 CN2 GIA，T1 走国际线路（双程 NTT，移动走 CMI）。

- **TYO.AS3.T1.WEE**：1 核 / 1GB / 20GB / 1TB Max，年付 **$36.9**。超流量限速不断线，测试 IP：154.31.112.5。
- **TYO.AS3.Pro.TINY**：1 核 / 1GB / 20GB / 300GB@1Gbps，月付 **$21.9**。CN2 GIA / AS9929 / CMI 三网回程，东京 Premium 系列最低入门门槛，2026 年 4 月有过一次小规模补货。测试 IP：154.12.190.32。
- **TYO.AS3.Pro.STARTER**：1 核 / 2GB / 40GB / 500GB@1Gbps，月付 **$39.9**。

### **美国洛杉矶机房（LAX）**

洛杉矶是 DMIT 的"老巢"，硬件最新，套餐也最多。AN5 平台（AMD EPYC 9005 / Zen 5）是旗舰，AN4（Zen 4）次之，AS3（Zen 3）性价比之王。

- **LAX.AN5.T1.VOLUME**：AMD EPYC 9005 平台，10Gbps 国际带宽，月付 **$14.9** 起。2026 年 4 月补过货，定位大流量国际互联，不带中国优化。
- **LAX.AN5.T1.GENERAL**：同 AN5 平台，硬件规格更高，月付 **$16.9** 起。
- **LAX.AN4.Pro.WEE**：1 核 / 1GB / 20GB SSD / 500GB@500Mbps，年付 **$39.9**。三网回程 CN2 GIA，限量款无优惠码，圣诞促销时出现过。
- **LAX.AN4.EB.CORONA / WEE**：1 核 / 1GB / 20GB / 1TB@1Gbps，年付 **$39.9**。电信联通去程走 9929，移动走 CMIN2，三网回程全走 CMIN2，性价比很高，但库存几乎秒空。
- **LAX.AN4.Pro.TINY**：1 核 / 2GB / 20GB / 1TB@1Gbps，月付约 **$37.99**（含循环优惠）。AMD EPYC 9004 平台 + CN2 GIA。

## **三、三网线路到底怎么选**

DMIT 把线路拆成三条产品线，配置一样、价格差好几倍，区别全在线路上。新手最容易卡在这一步。

- **Premium（Pro）系列**：三网回程 CN2 GIA，电信去程也走 CN2 GIA。延迟最低、丢包最少，香港到深圳约 15ms、东京到上海约 20-50ms。**适合**：面向中国大陆访客的电商、企业站、直播点播、低延迟游戏服、跨境 SaaS。**价位**：月付 $21.9 起，年付少见。
- **Eyeball（EB）系列**：Tier 1 + CMI/CMIN2 尽力而为的中国路由。移动用户体验最好，电信联通够用但不如 Premium。**适合**：面向中国 / 全球混合受众的博客、API 后端、远程开发、镜像下载。**价位**：月付 $29.9 起，比 Pro 便宜一大截。
- **Tier 1（T1）系列**：纯国际 BGP，不针对中国优化，但亚太和美洲之间走 DMIT 自有骨干 + 7.6Tbps Tier 1 互联。**适合**：海外业务、外贸、备份归档、CI/CD、VPN 中继、成本敏感的通用计算。**价位**：年付 $36.9 起，月付 $6.9 起，是入门首选。

一句话总结：**国内访问要稳就上 Pro，预算紧又要兼顾国内就选 EB，纯海外业务直接 T1，便宜大碗。**

## **四、DMIT 主力补货套餐对比表**

下面这张表汇总了近期三地补货的主要套餐，方便横向比较配置、线路和价格。所有购买链接都挂在官方 AFF 渠道，点进去直接进购物车。

| 套餐 | 机房 | 平台 / CPU | 内存 | SSD | 流量 / 带宽 | 线路 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| HKG.AS3.T1.WEE | 香港 | EPYC 7003 / 1 核 | 1GB | 20GB | 1TB@4Gbps | 国际 BGP | $36.9/年 | [点击购买](https://bit.ly/DMIt) |
| HKG.AS3.Pro.TINY | 香港 | EPYC 7003 / 1 核 | 1GB | 20GB | 500GB@1Gbps | CN2 GIA | $39.9/月 | [点击购买](https://bit.ly/DMIt) |
| HKG.AS3.EB.TINY | 香港 | EPYC 7003 / 1 核 | 1GB | 20GB | 1TB@1Gbps | CMI | $29.9/月 | [点击购买](https://bit.ly/DMIt) |
| TYO.AS3.T1.WEE | 东京 | EPYC 7003 / 1 核 | 1GB | 20GB | 1TB Max | 国际 BGP | $36.9/年 | [点击购买](https://www.dmit.io/aff.php?aff=13832&cmd=cart&action=add&pid=163) |
| TYO.AS3.Pro.TINY | 东京 | EPYC 7003 / 1 核 | 1GB | 20GB | 300GB@1Gbps | CN2 GIA | $21.9/月 | [点击购买](https://www.dmit.io/aff.php?aff=13832&cmd=cart&action=add&pid=162) |
| LAX.AN5.T1.VOLUME | 洛杉矶 | EPYC 9005 / 2 核 | 2GB | 40GB | 1TB@10Gbps | Tier 1 | $14.9/月 | [点击购买](https://www.dmit.io/aff.php?aff=13832&cmd=cart&action=add&pid=183) |
| LAX.AN5.T1.GENERAL | 洛杉矶 | EPYC 9005 / 2 核 | 2GB | 40GB | 1TB@10Gbps | Tier 1 | $16.9/月 | [点击购买](https://www.dmit.io/aff.php?aff=13832&cmd=cart&action=add&pid=184) |
| LAX.AN4.Pro.WEE | 洛杉矶 | EPYC 9004 / 1 核 | 1GB | 20GB | 500GB@500Mbps | CN2 GIA | $39.9/年 | [点击购买](https://bit.ly/DMIt) |
| LAX.AN4.Pro.TINY | 洛杉矶 | EPYC 9004 / 1 核 | 2GB | 20GB | 1TB@1Gbps | CN2 GIA | ~$37.99/月 | [点击购买](https://www.dmit.io/aff.php?aff=13832&cmd=cart&action=add&pid=188) |
| LAX.AN4.EB.TINY | 洛杉矶 | EPYC 9004 / 1 核 | 2GB | 20GB | 1TB@1Gbps | 9929+CMIN2 | ~$37.99/月 | [点击购买](https://www.dmit.io/aff.php?aff=13832&cmd=cart&action=add&pid=189) |

> 表格里的价格为官方公开报价，限量款（WEE / CORONA）经常处于售罄状态，能否抢到要看实时库存。所有套餐默认 1 个 IPv4 + 1 个 IPv6 /64，支持支付宝、PayPal、信用卡付款。

## **五、怎么第一时间蹲到补货**

DMIT 没有公开的 RSS 或邮件订阅，但有几个公认的"蹲货姿势"：

1. **关注 DMIT 官方 Telegram**：账号 @dmitnews，补货、新套餐、促销码基本都在这里首发，是最快的信息源。
2. **盯 VPS 监控站**：有不少玩家自建了 DMIT 库存监控页，按套餐列出红绿状态，部分支持邮件 / Telegram 补货提醒，比手动刷官网高效得多。
3. **常刷 V2BOX、低配主机圈子和 55 主机测评、daniao 等渠道**：国内 VPS 圈的补货帖基本第一时间同步，附带配置和购买链接。
4. **优先蹲 T1 WEE 和 Pro.WEE 这类限量款**：这类年付 $36.9 / $39.9 的套餐补货频率最高，门槛最低，是入门 DMIT 的最便宜方式。
5. **关注年付折扣码**：DMIT 偶尔会放年付循环优惠码，比如 LAX T1 Annually 有过 20% Off、HKG T1 Annually 有过 45% Off、日本 Premium 年付有过 30% Off 的循环折扣。这些码通常在官方 Telegram 或促销专题页发布，不要轻信第三方未经验证的"通用码"。

如果你正在为某个具体业务挑线路，没思路的话——**国内访客为主就闭眼上 Pro，预算紧选 EB，纯海外就 T1**，这套选法基本不会翻车。

## **六、下单前几件事提醒一下**

- DMIT 不提供退款（除个别情况），下单前最好先用测试 IP 跑一下三网延迟和丢包，确认线路符合预期再付款。香港 Pro 测试 IP `103.117.100.199`，东京 Pro 测试 IP `154.12.190.32`，香港 T1 测试 IP `154.12.176.28`，东京 T1 测试 IP `154.31.112.5`。
- LAX.AS3 系列官方说明正在建设和优化中，期间可能出现磁盘性能下降、SLA 低于成熟平台的情况，介意的话优先选 AN4 / AN5。
- WEE、CORONA 这类限量款通常不可叠加优惠码，价格已经是最优。
- Pro / EB 套餐流量超出会停机，T1 套餐超量限速不断线（WEE 限速 50Mbps），按业务流量预估再选套餐，别只看价格。
- AS3 / AN4 / AN5 三代平台性能差距明显：Geekbench 6 单核参考分 AS3 约 1845、AN4 同价位更高、AN5（Zen 5）约 2770，对 CPU 敏感的业务直接上 AN5。

准备好了就 👉 [去 DMIT 看看当前库存](https://bit.ly/DMIt)，热门款靠手速，别犹豫。
