---
title: 设置服务间隔
description: 服务间隔指示在您创建服务订单时为服务协议行创建服务订单行所采用的频率。
author: ShylaThompson
manager: AnnBe
ms.date: 02/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SMAAgreementinterval
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: ShylaThompson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 2a80b0a604bf2550b6d0f6d94f8baabb070f6d3c
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55368"
---
# <a name="set-up-service-intervals"></a><span data-ttu-id="71bc4-103">设置服务间隔</span><span class="sxs-lookup"><span data-stu-id="71bc4-103">Set up service intervals</span></span>  

[!include [banner](../includes/banner.md)]

<span data-ttu-id="71bc4-104">服务间隔指示在您创建服务订单时为服务协议行创建服务订单行所采用的频率。</span><span class="sxs-lookup"><span data-stu-id="71bc4-104">Service interval indicates the frequency with which service order lines are created for service agreement lines when you create service orders.</span></span>

1. <span data-ttu-id="71bc4-105">单击**服务管理** \> **设置** \> **服务协议** \> **服务间隔**。</span><span class="sxs-lookup"><span data-stu-id="71bc4-105">Click **Service management** \> **Setup** \> **Service agreements** \> **Service intervals**.</span></span>
2. <span data-ttu-id="71bc4-106">创建新的服务间隔。</span><span class="sxs-lookup"><span data-stu-id="71bc4-106">Create a new service interval.</span></span>
3. <span data-ttu-id="71bc4-107">输入 ID 和服务间隔的描述。</span><span class="sxs-lookup"><span data-stu-id="71bc4-107">Enter the ID and description of the service interval.</span></span>
4. <span data-ttu-id="71bc4-108">在**范围**字段中，选择范围。</span><span class="sxs-lookup"><span data-stu-id="71bc4-108">In the **Range** field, select the range.</span></span>
5. <span data-ttu-id="71bc4-109">在**频率**字段中，输入频率。</span><span class="sxs-lookup"><span data-stu-id="71bc4-109">In the **Frequency** field, type the frequency.</span></span> <span data-ttu-id="71bc4-110">必须将该频率作为系数与范围相乘，以获取服务协议间隔。</span><span class="sxs-lookup"><span data-stu-id="71bc4-110">The frequency is the factor by which you must multiply the range to obtain the interval for a service agreement.</span></span>
6. <span data-ttu-id="71bc4-111">按 **Alt+S** 保存服务间隔。</span><span class="sxs-lookup"><span data-stu-id="71bc4-111">Press **Alt+S** to save the service interval.</span></span>

## <a name="example"></a><span data-ttu-id="71bc4-112">示例</span><span class="sxs-lookup"><span data-stu-id="71bc4-112">Example</span></span>

<span data-ttu-id="71bc4-113">您要创建为期 10 天的服务间隔。</span><span class="sxs-lookup"><span data-stu-id="71bc4-113">You want to create a service interval of 10 days.</span></span>

<span data-ttu-id="71bc4-114">**创建 10 天的服务间隔**</span><span class="sxs-lookup"><span data-stu-id="71bc4-114">**Create a 10-day service interval**</span></span>

1. <span data-ttu-id="71bc4-115">单击**服务管理** \> **设置** \> **服务协议** \> **服务间隔**。</span><span class="sxs-lookup"><span data-stu-id="71bc4-115">Click **Service management** \> **Setup** \> **Service agreements** \> **Service intervals**.</span></span>
2. <span data-ttu-id="71bc4-116">创建新的服务间隔。</span><span class="sxs-lookup"><span data-stu-id="71bc4-116">Create a new service interval.</span></span>
3. <span data-ttu-id="71bc4-117">输入 ID 和服务间隔的描述。</span><span class="sxs-lookup"><span data-stu-id="71bc4-117">Enter the ID and description of the service interval.</span></span>
4. <span data-ttu-id="71bc4-118">在**范围**字段中，选择**每天**。</span><span class="sxs-lookup"><span data-stu-id="71bc4-118">In the **Range** field, select **Daily**.</span></span>
5. <span data-ttu-id="71bc4-119">在**频率**字段中键入 10。</span><span class="sxs-lookup"><span data-stu-id="71bc4-119">In the **Frequency** field, type 10.</span></span>
6. <span data-ttu-id="71bc4-120">按 **Alt+S** 保存服务间隔。</span><span class="sxs-lookup"><span data-stu-id="71bc4-120">Press **Alt+S** to save the service interval.</span></span>

## <a name="related-topics"></a><span data-ttu-id="71bc4-121">相关主题</span><span class="sxs-lookup"><span data-stu-id="71bc4-121">Related topics</span></span>

[<span data-ttu-id="71bc4-122">服务间隔</span><span class="sxs-lookup"><span data-stu-id="71bc4-122">Service intervals</span></span>](service-intervals.md)  
