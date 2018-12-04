---
title: Windows 10 cihazlarının güvenliğini sağlama
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: 'Varsayılan ve diğer ayarları Windows 10 aygıtlar güvenli hakkında bilgi edinin. '
ms.openlocfilehash: 0bdf6a56d880cb84f4a4f50550539d97c006ba49
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983660"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="63b6b-103">Windows 10 cihazlarının güvenliğini sağlama</span><span class="sxs-lookup"><span data-stu-id="63b6b-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="63b6b-p101">Burada yapılandırdığınız ayarlar, Windows 10 için varsayılan cihaz ilkesinin bir parçasıdır. Mobil cihazlar ve bilgisayarlar da dahil olmak üzere bir Windows 10 cihaza bağlanan tüm kullanıcılar, iş hesaplarıyla oturum açtığında bu ayarları otomatik olarak alır. Kurulum sırasında varsayılan ilkeyi kabul etmenizi ve daha sonra belirli kullanıcı gruplarını hedef alan ilkeler eklemenizi öneririz.</span><span class="sxs-lookup"><span data-stu-id="63b6b-p101">The settings that you configure here are part of the default device policy for Windows 10. All users that connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account, will automatically receive these settings. We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="63b6b-107">Windows 10 cihazlarının güvenliğini sağlayan ayarlar</span><span class="sxs-lookup"><span data-stu-id="63b6b-107">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="63b6b-p102">Varsayılan olarak tüm ayarlar **Açık** durumdadır. Aşağıdaki ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="63b6b-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="63b6b-110">Ayar</span><span class="sxs-lookup"><span data-stu-id="63b6b-110">Setting</span></span>  <br/> |<span data-ttu-id="63b6b-111">Açıklama</span><span class="sxs-lookup"><span data-stu-id="63b6b-111">Description</span></span>  <br/> |
|<span data-ttu-id="63b6b-112">Windows Defender Virüsten Koruma kullanarak bilgisayarların virüslere ve diğer tehditlere karşı korunmasına yardımcı ol</span><span class="sxs-lookup"><span data-stu-id="63b6b-112">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="63b6b-113">Bilgisayarları İnternet'e bağlı olmanın tehlikelerinden korumak için Windows Defender Virüsten Koruma programının açık olmasını gerektirir.</span><span class="sxs-lookup"><span data-stu-id="63b6b-113">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="63b6b-114">Bilgisayarları Microsoft Edge'de web tabanlı tehditlere karşı korumaya yardımcı ol</span><span class="sxs-lookup"><span data-stu-id="63b6b-114">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="63b6b-115">Edge'de, kullanıcıları kötü amaçlı sitelerden ve indirmelerden korumaya yardımcı olan ayarları açar.</span><span class="sxs-lookup"><span data-stu-id="63b6b-115">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="63b6b-116">Cihaz şu kadar süre boşta kaldığında ekranı kapat</span><span class="sxs-lookup"><span data-stu-id="63b6b-116">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="63b6b-p103">Kullanıcı cihaz başında olmadığında şirket verilerinin korunmasını sağlar. Kullanıcı bir kafe gibi herkese açık bir konumda çalışıyorken kısa süreliğine uzaklaşabilir veya başka bir şeyle ilgilenebilir, bu durumda cihaz rastgele bakışlara açık hale gelir. Bu ayar sayesinde ekran kapanmadan önce kullanıcının ne kadar süre boşta olabileceğini denetleyebilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="63b6b-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="63b6b-120">Kullanıcıların Microsoft Store'ndan uygulama indirmesine izin ver</span><span class="sxs-lookup"><span data-stu-id="63b6b-120">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="63b6b-p104">Kullanıcıların Microsoft Store'ndan uygulama indirmesine ve yüklemesine izin verir. Uygulamalar, oyunlardan üretkenlik araçlarına kadar her şeyi içerebilir, dolayısıyla bu ayar **Açık** durumdadır ancak ek güvenlik için kapatabilirsiniz.  </span><span class="sxs-lookup"><span data-stu-id="63b6b-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="63b6b-123">Kullanıcıların Cortana'ya erişmesine izin ver</span><span class="sxs-lookup"><span data-stu-id="63b6b-123">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="63b6b-p105">Cortana çok yararlı olabilir! Cortana sizin yerinize ayarları açıp kapatabilir, yol tarif edebilir ve randevularınıza zamanında gitmenizi sağlayabilir; dolayısıyla bu ayar varsayılan olarak **Açık** durumdadır.  </span><span class="sxs-lookup"><span data-stu-id="63b6b-p105">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="63b6b-126">Kullanıcıların Microsoft'tan Windows ipucu ve reklam almasına izin ver</span><span class="sxs-lookup"><span data-stu-id="63b6b-126">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="63b6b-127">Windows ipuçları kullanışlı olabilir ve yeni özellikler kullanıma sunulduğunda kullanıcıların yönlendirilmesine yardım edebilir.</span><span class="sxs-lookup"><span data-stu-id="63b6b-127">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="63b6b-128">Windows 10 cihazları otomatik olarak güncelleştir</span><span class="sxs-lookup"><span data-stu-id="63b6b-128">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="63b6b-129">Windows 10 cihazların son güncelleştirmeleri otomatik olarak aldığından emin olur.</span><span class="sxs-lookup"><span data-stu-id="63b6b-129">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
   
