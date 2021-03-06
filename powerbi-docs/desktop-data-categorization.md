---
title: Power BI Desktop 中的数据分类
description: Power BI Desktop 中的数据分类
services: powerbi
documentationcenter: ''
author: davidiseminger
manager: kfile
backup: ''
editor: ''
tags: ''
qualityfocus: no
qualitydate: ''
ms.service: powerbi
ms.devlang: NA
ms.topic: article
ms.tgt_pltfrm: NA
ms.workload: powerbi
ms.date: 12/06/2017
ms.author: davidi
LocalizationGroup: Model your data
ms.openlocfilehash: cc66655e49860160b43afa5d1acb688c37468212
ms.sourcegitcommit: c80fbf5b12754ce217cb47a17cb5400b1036a8f2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2018
---
# <a name="data-categorization-in-power-bi-desktop"></a>Power BI Desktop 中的数据分类
在 **Power BI Desktop** 中，你可以为列指定数据类别，以便让 Power BI Desktop 知道如何在可视化效果中处理其值。

当 Power BI Desktop 导入数据时，它不仅会获取本身数据，还会获取表和列名称等信息（无论它是否为主关键字）。有了这些信息，Power BI Desktop 会进行某些假设，让你在创建可视化效果时可拥有较好的默认体验。 

下面的示例说明：当 Power BI Desktop 检测到某列有数字值时，你可能想以某种方式进行聚合，由此它将会被置于值区域。 或者，对于带日期时间值的列，它会假设你可能将其用作折线图上的时间层次结构轴。

但是，有些情况比较具有挑战性，如地理位置。 请思考下列来自 Excel 工作表的表：

![](media/desktop-data-categorization/datacategorizationtable.png)

Power BI Desktop 应该将 GeoCode 列中的代码视为国家/地区或美国州名的缩写吗？  由于此类代码可能表示这两种意思中的任何一个，因此并不清楚。  例如，AL 可以表示阿拉巴马或阿尔巴尼亚，AR 可以表示阿肯色或阿根廷，CA 可以表示加利福尼亚州或加拿大。 当我们在地图上绘制 GeoCode 字段时，需要加以区分。  Power BI Desktop 是突出显示了国家/地区的世界地图，还是突出显示了各州的美国地图呢？  你可以为此类型的数据指定数据类别。 数据分类进一步改进 Power BI Desktop 可用于提供最佳可视化效果的信息。  

**指定数据类别**

1. 在“报表视图”或“数据视图”中的**字段**列表中，选择你想要按不同的分类进行排序的字段。
2. 在功能区的“建模”选项卡上，单击“数据类别:”下拉列表。  这将显示你可以从列中选择的数据类别列表。  如果某些选项不适用于列的当前数据类型，它们可能会被禁用。  例如，如果列为二进制数据类型，Power BI Desktop 将不允许你选择地理数据类别。 

![](media/desktop-data-categorization/datacategorization.gif)

这样就大功告成了！  通常累算到视觉对象的任何行为将会自动进行。  

你可能还有兴趣了解[ Power BI 移动应用的地理筛选](desktop-mobile-geofiltering.md)。

