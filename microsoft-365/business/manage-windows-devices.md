---
title: Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: 365 korumak Microsoft etkinleştirmeyi öğrenin Yerel AD alanına katılmış Windows 10 aygıtlar.
ms.openlocfilehash: 6e66a2c5417c9037232c1ada654d4cac3c520607
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982660"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="d8850-103">Etki alanına katılmış Windows 10 cihazlarını Microsoft 365 İş tarafından yönetilecek şekilde etkinleştirme</span><span class="sxs-lookup"><span data-stu-id="d8850-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="d8850-p101">Kuruluşunuz yerinde Windows Server Active Directory kullanıyorsa, Microsoft 365 iş hala yerinde yerel kimlik doğrulaması gerektiren kaynaklara erişimi koruyarak Windows 10 aygıtlarınızın korumak için ayarlayabilirsiniz. Bu ilk Active Directory Azure Windows 10 aygıtları ile Azure AD kaydetme ve bunları Microsoft 365 Business tarafından mobil aygıt yönetimi için kaydolma ve ardından, Active Directory ile eşitlenmesi yoluyla ayarlayabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8850-p101">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication. You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="d8850-106">Microsoft 365 işletme tarafından yönetilecek etki alanına katılmış aygıtları Ayarla</span><span class="sxs-lookup"><span data-stu-id="d8850-106">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="d8850-p102">Kuruluşunuzun etki alanına katılmış aygıtları Azure yerinde Active Directory ek olarak Active Directory tarafından sağlanan yeteneklerinin sağladığı avantajlardan yararlanabilmenizi ayarlamak için **karma Azure AD alanına bağlı aygıtlar**uygulayabilirsiniz. Bunlar hem yerinde Active Directory ve Active Directory Azure katılan aygıtlardır. Karma Azure AD alanına bağlı aygıtların korumalı ve Microsoft 365 işletme tarafından yönetilen...</span><span class="sxs-lookup"><span data-stu-id="d8850-p102">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**. These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory. Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business..</span></span> 
  
<span data-ttu-id="d8850-110">Windows 10 aygıtlarınızın karma katıldı ve Microsoft 365 işletme tarafından yönetilen Azure Reklam yapmak için aşağıdaki adımları tamamlayın.</span><span class="sxs-lookup"><span data-stu-id="d8850-110">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="d8850-111">Azure Active Directory'ye, kullanıcıları, grupları ve yerel Active Directory'den kişileri eşitlemek için dizin eşitleme Sihirbazı ve Azure Active Directory [dizin eşitleme için Office 365 ayarlamak](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846)açıklandığı gibi bağlanmak çalışır.</span><span class="sxs-lookup"><span data-stu-id="d8850-111">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="d8850-112">Tam olarak Microsoft 365 iş için aynı adımlardır.</span><span class="sxs-lookup"><span data-stu-id="d8850-112">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="d8850-113">Karma Azure AD alanına bağlı olarak Windows 10 aygıtları etkinleştirmek için 3 adım tamamlamadan önce aşağıdaki önkoşulları karşıladığından emin olmanız gerekir:</span><span class="sxs-lookup"><span data-stu-id="d8850-113">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>
    
   - <span data-ttu-id="d8850-114">Azure AD'ın en son sürümünü çalıştırdığınızı bağlayın.</span><span class="sxs-lookup"><span data-stu-id="d8850-114">You are running the latest version of Azure AD connect.</span></span>
    
   - <span data-ttu-id="d8850-p103">Azure AD bağlanmak karma Azure AD alanına dahil olmasını istediğiniz aygıtların tüm bilgisayar nesneleri eşitlendi. Bilgisayar nesnelerine ait belirli kuruluş birimleri (OU), sonra bu OU Azure AD alanında eşitleme için ayarlandığından emin olun, aynı zamanda bağlayın.</span><span class="sxs-lookup"><span data-stu-id="d8850-p103">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined. If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="d8850-117">Karma Azure AD katılmış olması ve Mobil Aygıt Yönetimi tarafından Intune (Microsoft 365 iş) kaydolmak için varolan etki alanına katılmış Windows 10 aygıtları kaydedin:</span><span class="sxs-lookup"><span data-stu-id="d8850-117">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="d8850-p104">[Karma Azure Active Directory alanına bağlı aygıtları yapılandırma hakkında](https://go.microsoft.com/fwlink/p/?linkid=872870)adım adım yönergeleri izleyin. Bu, şirket içi Active Directory eşitlemesine olanak sağlar Windows 10 bilgisayar katıldı ve bunları bulut hazır olun.</span><span class="sxs-lookup"><span data-stu-id="d8850-p104">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870). This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="d8850-p105">Windows 10 aygıt taşınabilir aygıt yönetimi için kaydolmak için [Grup İlkesi kullanarak Intune Windows 10 aygıtla kaydetmek](https://go.microsoft.com/fwlink/p/?linkid=872871) yönergeler için bkz. Grup İlkesi yerel bilgisayar düzeyinde ayarlayabilirsiniz veya toplu işlemler için etki alanı denetleyicisi sunucunuzda bu Grup İlkesi ayarı oluşturabilirsiniz.</span><span class="sxs-lookup"><span data-stu-id="d8850-p105">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions. You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span> 
    
