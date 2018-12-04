---
title: Windows 10 cihazlara yönelik uygulama koruma ayarlarını belirleme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
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
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Bir uygulama yönetimi ilkesi oluşturabilir ve iş dosyalarını Windows 10 aygıtlarda korumak öğrenin.
ms.openlocfilehash: acf19a72d994185a35b2e425f8334a73a121ee10
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982830"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="0153a-103">Windows 10 cihazlara yönelik uygulama koruma ayarlarını belirleme</span><span class="sxs-lookup"><span data-stu-id="0153a-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="0153a-104">Windows 10 için uygulama yönetimi ilkesi oluşturma</span><span class="sxs-lookup"><span data-stu-id="0153a-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="0153a-105">Kullanıcılarınızın işle ilgili görevleri gerçekleştirdikleri kişisel Windows 10 cihazları varsa, verilerinizi bu cihazlarda da koruma altına alabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0153a-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="0153a-p101">Genel yönetici kimlik bilgileriyle [Microsoft 365 Business](https://portal.office.com)'da oturum açın. Yönetim merkezine gitmek için **Yönetici** kutucuğunu seçin.</span><span class="sxs-lookup"><span data-stu-id="0153a-p101">Sign in to [Microsoft 365 Business](https://portal.office.com) with global admin credentials. Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="0153a-108">Yönetici portalındaki **Cihaz ilkeleri** kartında **İlke ekle**'yi seçin.</span><span class="sxs-lookup"><span data-stu-id="0153a-108">On the **Device policies** card of the admin portal, choose **Add policy**.</span></span>
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. <span data-ttu-id="0153a-110">**İlke ekle** bölmesinde bu ilke için benzersiz bir ad girin.</span><span class="sxs-lookup"><span data-stu-id="0153a-110">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="0153a-111">**İlke türü**'nün altında **Windows 10 için Uygulama Yönetimi**'ni seçin.</span><span class="sxs-lookup"><span data-stu-id="0153a-111">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="0153a-112">Altında \*\* aygıt türü \*\*, **Kişisel** ya da **Şirket sahibi**seçin.</span><span class="sxs-lookup"><span data-stu-id="0153a-112">Under \*\* Device type \*\*, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="0153a-113">**İş dosyalarını şifrele** seçeneği otomatik olarak açılır.</span><span class="sxs-lookup"><span data-stu-id="0153a-113">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="0153a-114">Kullanıcıların çalışma dosyalarını kendi bilgisayarlarına kaydetmelerini istemiyorsanız, **Kullanıcıların şirket verilerini kişisel dosyalara kopyalamasını engelle ve çalışma dosyalarını OneDrive İş'e kaydetmelerini zorla** ilkesini **Açık** olarak ayarlayın.</span><span class="sxs-lookup"><span data-stu-id="0153a-114">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
8. <span data-ttu-id="0153a-p102">**Kullanıcıların Office dosyalarını aygıtlarda nasıl eriştiğini yönetmek** genişletin \> nasıl istediğiniz ayarları yapılandırın. \*\* **Kullanıcıların Office içeren aygıtlar mobil aygıtlarda nasıl eriştiğini yönetmek** varsayılan olarak kapalıdır\*\* , ancak **bunu açın** ve varsayılan değerleri kabul tavsiye edilir. Daha fazla bilgi için bkz: [kullanılabilir ayarları](protection-settings-for-windows-10-devices.md#bkmk_settings) .</span><span class="sxs-lookup"><span data-stu-id="0153a-p102">Expand **Manage how users access Office files on devices** \> configure the settings how you would like. The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values. See [Available settings](protection-settings-for-windows-10-devices.md#bkmk_settings) for more information.</span></span> 
    
    <span data-ttu-id="0153a-118">Varsayılan ayarlara dönmek için istediğiniz zaman **Varsayılan ayarlara sıfırla** bağlantısını kullanabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="0153a-118">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
9. <span data-ttu-id="0153a-119">**Windows cihazlarındaki verileri kurtar** seçeneğini genişletin; bu seçeneği **Açık** duruma getirmeniz önerilir.</span><span class="sxs-lookup"><span data-stu-id="0153a-119">Expand **Recover data on Windows devices** and it is recommended that you turn it **On**.</span></span>
    
    <span data-ttu-id="0153a-p103">Veri Kurtarma Aracısı sertifikasının konumuna göz atabilmeniz için, önce bir sertifika oluşturmanız gerekir. Yönergeler için bkz. [Şifreleme Dosya Sistemi (EFS) Veri Kurtarma Aracısı (DRA) sertifikasını oluşturma ve doğrulama](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="0153a-p103">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one. For instructions see, [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="0153a-p104">Varsayılan olarak iş dosyalarınız, cihazda depolanan ve kullanıcının profili ile ilişkilendirilmiş bir gizli anahtar kullanılarak şifrelenir. Yalnızca kullanıcı dosyanın şifresini çözebilir ve dosyayı açabilir. Bununla birlikte, cihaz kaybolursa veya kullanıcı kaldırılırsa, dosya şifrelenmiş halde kalabilir. Dosyanın şifresini çözmek için yönetici, Veri Kurtarma Aracısı (DRA) sertifikası kullanabilir.</span><span class="sxs-lookup"><span data-stu-id="0153a-p104">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile. Only the user can open and decrypt the file. However, if a device is lost or a user is removed, a file can be stuck in an encrypted state. The Data Recovery Agent (DRA) certificate can be used by an admin to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="0153a-p105">Listelenen tüm uygulamalardaki dosyaların korunduğundan emin olmak için başka etki alanları veya SharePoint Online konumları eklemek istiyorsanız, **Ek ağ ve bulut konumlarını koru** seçeneğini genişletin. Alanlara birden çok öğe girmeniz gerekiyorsa, öğeler arasında noktalı virgül (;) kullanın.</span><span class="sxs-lookup"><span data-stu-id="0153a-p105">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps will be protected. If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span> 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="0153a-p106">Sonra karar **Bu ayarları elde kim?** Varsayılan **Tüm kullanıcıların** güvenlik grubu kullanmak istemiyorsanız, **Değiştir**' i seçin, bu ayarları alırsınız güvenlik grupları seçin \> **seçin**.</span><span class="sxs-lookup"><span data-stu-id="0153a-p106">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="0153a-132">Son olarak, **Ekle**'yi seçerek ilkeyi kaydedin ve cihazlarınıza atayın.</span><span class="sxs-lookup"><span data-stu-id="0153a-132">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="0153a-133">Kullanılabilir ayarlar</span><span class="sxs-lookup"><span data-stu-id="0153a-133">Available settings</span></span>

<span data-ttu-id="0153a-134">Kullanıcıların Office iş dosyalarına erişimini yönetmek şu ayarlar kullanılabilir:</span><span class="sxs-lookup"><span data-stu-id="0153a-134">The following settings are available to manage how users access Office work files.</span></span>
  
<span data-ttu-id="0153a-135">Daha fazla bilgi için bkz. [Microsoft 365 İş'in koruma özellikleriyle Intune ayarları nasıl eşleşir?](map-protection-features-to-intune-settings.md)</span><span class="sxs-lookup"><span data-stu-id="0153a-135">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span>
  
|<span data-ttu-id="0153a-136">**Ayar**</span><span class="sxs-lookup"><span data-stu-id="0153a-136">**Setting**</span></span>|<span data-ttu-id="0153a-137">**Açıklama**</span><span class="sxs-lookup"><span data-stu-id="0153a-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0153a-138">Office uygulamalarına erişirken PIN veya parmak izi iste</span><span class="sxs-lookup"><span data-stu-id="0153a-138">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="0153a-139">Bu ayarlar **Açık** ise kullanıcıların Office uygulamalarını mobil cihazlarında kullanabilmeleri için kullanıcı adı ve parolalarının yanı sıra başka bir doğrulama biçimi daha sağlaması gerekir.</span><span class="sxs-lookup"><span data-stu-id="0153a-139">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="0153a-140">Belirli sayıda başarısız oturum açma girişimi yapıldığında PIN'i sıfırla</span><span class="sxs-lookup"><span data-stu-id="0153a-140">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="0153a-141">Yetkisiz bir kullanıcının PIN'i rastgele tahmin etmesini engellemek için belirlediğiniz sayıda yanlış giriş yapılırsa PIN sıfırlanır.</span><span class="sxs-lookup"><span data-stu-id="0153a-141">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="0153a-142">Office uygulamaları belirli bir süre boyunca boşta kalırsa kullanıcıların yeniden oturum açmasını iste</span><span class="sxs-lookup"><span data-stu-id="0153a-142">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="0153a-143">Bu ayar, bir kullanıcının yeniden oturum açması istenmeden önce ne kadar süreliğine boşta kalabileceğini belirler.</span><span class="sxs-lookup"><span data-stu-id="0153a-143">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
   
