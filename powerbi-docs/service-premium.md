---
title: Power BI Premium 有哪些特权？
description: Power BI Premium 是适用于组织或团队的专用容量，提供了更可靠的性能和更大的数据卷，使你无需购买每用户许可证。
services: powerbi
documentationcenter: ''
author: mgblythe
manager: kfile
backup: ''
editor: ''
tags: ''
qualityfocus: no
qualitydate: ''
ms.service: powerbi
ms.devlang: NA
ms.topic: get-started-article
ms.tgt_pltfrm: NA
ms.workload: powerbi
ms.date: 02/05/2018
ms.author: mblythe
LocalizationGroup: Premium
ms.openlocfilehash: 617e56fd688016c8ee17184f726fb018a0128e05
ms.sourcegitcommit: 312390f18b99de1123bf7a7674c6dffa8088529f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2018
---
# <a name="power-bi-premium---what-is-it"></a>Power BI Premium 有哪些特权？
Power BI Premium 资源专用于为组织或团队运行 Power BI 服务，为你提供更可靠的性能和更大的数据卷。 Premium 还可以广泛发布内容，无需为查看者购买许可证。

可以将工作区分配到高级容量，从而充分利用 Power BI Premium。 “高级容量”是组织的专用资源。 未分配到高级容量的工作区，则属于共享容量。

“共享容量”是指在 Power BI 使用体验中，工作负荷在其他客户共享的计算资源上运行。 在共享容量中，为了确保所有用户的体验质量，每个用户会受到更多的限制。

[!INCLUDE [powerbi-premium-illustration](./includes/powerbi-premium-illustration.md)]

<iframe width="560" height="315" src="https://www.youtube.com/embed/lNQDkN0GXzU?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe>

## <a name="capacity-tiers"></a>容量层级
Power BI 中有两种类型的容量。 共享容量和 Power BI 高级容量。 下面我们来看它们之间的区别。

|  | 共享容量 | Power BI 高级容量 |
| --- | --- | --- |
| 刷新频率 |每天 8 次 |不受限制 |
| 专用硬件隔离 |![](media/service-premium/not-available.png "不可用") |![](media/service-premium/available.png "可用") |
| 面向所有用户的企业分发 | | |
| 应用 |![](media/service-premium/not-available.png "不可用") |![](media/service-premium/available.png "可用")<sup>1</sup> |
| 嵌入式 API 和控件 |![](media/service-premium/not-available.png "不可用") |![](media/service-premium/available.png "可用")<sup>2</sup> |
| 在本地发布 Power BI 报表 |![](media/service-premium/not-available.png "不可用") |![](media/service-premium/available.png "可用") |

*<sup>1</sup> 应用中用户可以免费使用的功能包括在 Web 和移动设备中查看内容、使用问答、Quick Insights、Cortana 以及导出到 CSV、Excel 和 PowerPoint。其他未列出的活动（如在共享数据集上创建报表和在 Excel 中分析）需要 Pro 许可证。详细了解 [Power BI 免费版与 Pro](service-free-vs-pro.md) 功能。*  
*<sup>2</sup> Power BI Premium 公开发布后推出的增强功能。*

### <a name="premium-capacity"></a>高级容量
需要将工作区分配给某个容量，方可开始使用 Power BI 高级容量。 有关如何将工作区分配给高级容量的详细信息，请参阅[管理 Power BI Premium](service-admin-premium-manage.md)。

工作区受高级容量支持时，可以享受 Power BI Premium 的权益。

* 预定刷新：使用导入的模型计划刷新时，用户以前的限制为每天 8 次。 对 Premium 工作区的数据集解除了此限制。 这不适用于 DirectQuery 的预定缓存刷新设置。 在高级容量和共享容量之间，这些设置保持相同。
* 专用硬件隔离 – 根据共享容量的性质，报表和仪表板的性能可能会该容量中受其他工作负荷的资源需求影响，尽管我们对此有所防护。 相反，Premium 通过隔离不相关的工作负荷，为你的工作负荷提供更一致、更可靠的性能。

如果应用受高级容量支持（即它是当前分配到高级容量的应用工作区发布的），则此后组织中的任何用户都可以使用发布的这个应用，而无需考虑分配给他们的许可证。 这意味着即使是 Power BI 免费用户也可以使用这些已发布的应用。

### <a name="shared-capacity"></a>共享容量
默认情况下，你的工作区属于共享容量。 这包括你个人的“我的工作区”以及应用工作区。 “共享容量”是指在 Power BI 使用体验中，工作负荷在其他客户共享的计算资源上运行。

<a name="premiumskus"/>

### <a name="premium-capacity-nodes"></a>高级容量节点
不同虚拟核心容量的节点配置中可使用 Power BI Premium。 有关特定 SKU 产品和成本的详细信息，请参阅 [Power BI 定价](https://powerbi.microsoft.com/pricing/)。 也可使用[成本计算器](https://powerbi.microsoft.com/calculator/)。 有关嵌入分析容量规划的信息，请参阅[“规划 Power BI Enterprise 部署”白皮书](https://aka.ms/pbienterprisedeploy)。

* P 节点可以用于嵌入式部署或服务部署
* EM 节点仅用于嵌入式部署
* EM1 和 EM2 

>[!NOTE]
>只有充当 Office 365 全局管理员的用户才能正常运行此表中的链接 - 其他人会收到 404 错误。 

| 容量节点 | 总虚拟核心<br/>（后端 + 前端） | 后端虚拟核心 | 前端虚拟核心 | DirectQuery/实时连接限制 | 高峰时间的最大显示页数 | 是否支持 |
| --- | --- | --- | --- | --- | --- | --- |
| [EM1（按月）](https://portal.office.com/SubscriptionDetails?OfferId=4004702D-749C-4F74-BF47-3048F1833780&adminportal=1) |1 个虚拟核心 |0.5 个虚拟核心，2.5 GB RAM |0.5 个虚拟核心 |每秒 3.75 |150-300 |可用 |
| [EM2（按月）](https://portal.office.com/SubscriptionDetails?OfferId=4004702D-749C-4F74-BF47-3048F1833780&adminportal=1) |2 个虚拟核心 |1 个虚拟核心，5 GB RAM |1 个虚拟核心 |每秒 7.5 |301-600 |可用 |
| [EM3（按月）](https://portal.office.com/SubscriptionDetails?OfferId=4004702D-749C-4F74-BF47-3048F1833780&adminportal=1) |4 个虚拟核心 |2 个虚拟核心，10 GB RAM |2 个虚拟核心 | |601-1,200 |可用 |
| [P1](https://portal.office.com/SubscriptionDetails?OfferId=b3ec5615-cc11-48de-967d-8d79f7cb0af1&adminportal=1) |8 个虚拟核心 |4 个虚拟核心，25 GB RAM |4 个虚拟核心 |每秒 30 个 |1,201-2,400 |可用（也可以[按月](https://portal.office.com/SubscriptionDetails?OfferId=E4C8EDD3-74A1-4D42-A738-C647972FBE81&adminportal=1)） |
| [P2](https://portal.office.com/SubscriptionDetails?OfferId=062F2AA7-B4BC-4B0E-980F-2072102D8605&adminportal=1) |16 个虚拟核心 |8 个虚拟核心，50 GB RAM |8 个虚拟核心 |每秒 60 个 |2,401-4,800 |可用 |
| [P3](https://portal.office.com/SubscriptionDetails?OfferId=40c7d673-375c-42a1-84ca-f993a524fed0&adminportal=1) |32 个虚拟核心 |16 个虚拟核心，100 GB RAM |16 个虚拟核心 |每秒 120 个 |4,801-9600 |可用 |

* 前端虚拟核心负责 Web 服务、仪表板和报表文档管理、访问 Rights Management、时间安排、API、上传和下载，并大体包括所有与用户体验相关的内容。
* 后端虚拟核心负责完成繁重的任务：查询处理、缓存管理、运行 R 服务器、数据刷新、自然语言处理、实时馈送和在服务器端绘制报表和图像。 后端虚拟核心也可保留一定的内存量。 处理大型数据模型或大量活动数据集时，内存充足尤为重要。

## <a name="power-bi-report-server"></a>Power BI 报表服务器
Power BI Premium 包含在本地运行 Power BI 报表服务器的权限。 更多详细信息，请参阅[开始使用 Power BI 报表服务器](report-server/get-started.md)。

## <a name="next-steps"></a>后续步骤
[Power BI Premium 常见问题解答](service-premium-faq.md)  
[Power BI Premium 发行说明](service-premium-release-notes.md)  
[如何购买 Power BI Premium](service-admin-premium-purchase.md)  
[管理 Power BI Premium](service-admin-premium-manage.md)  
[Microsoft Power BI Premium 白皮书](https://aka.ms/pbipremiumwhitepaper)  
[规划 Power BI Enterprise 部署白皮书](https://aka.ms/pbienterprisedeploy)  
[在组织中管理 Power BI](service-admin-administering-power-bi-in-your-organization.md)  

更多问题？ [尝试咨询 Power BI 社区](https://community.powerbi.com/)

