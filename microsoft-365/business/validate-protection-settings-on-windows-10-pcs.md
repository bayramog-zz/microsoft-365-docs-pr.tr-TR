---
title: Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Windows 10 cihazlarında Microsoft 365 İş uygulaması koruma ayarlarını nasıl doğrulayayarılamayı öğrenin.
ms.openlocfilehash: c54b053c1f6efbca8fd02431c416793a044c6821
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: tr-TR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721870"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Windows 10 bilgisayarlarda uygulama koruma ayarlarını doğrulama

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Kullanıcıların şirket cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama

[Uygulama koruma ilkelerini ayarladıktan](protection-settings-for-windows-10-devices.md) sonra, ilkenin kullanıcı cihazlarında geçerlilik kazanması birkaç saat sürebilir. Kullanıcıların şirket verilerini kişisel dosyalara kopyalamasını Engelley'i **açtıysanız** ve iş dosyalarını şirkete ait cihazlar için İş için **OneDrive'a kaydetmeye zorladıysanız,** azure AD'ye bağlanıp oturum açtıktan sonra bunu kullanıcının aygıtında denetleyebilirsiniz. 
  
 **Bağlantı ayarlarını doğrulama**
  
1. [Microsoft 365 İş kullanıcıları için Windows cihazlarını ayarlama](set-up-windows-devices.md) konusunda açıklandığı gibi Microsoft 365 İş kimlik bilgileriyle oturum açtıktan ve Azure AD'ye bağlandıktan sonra, **Windows Ayarları** \> **Hesaplar** \> **İş yeri veya okula eriş** seçeneğine gidin. **Bağlanılan \<kiracı adı\> Azure AD**'yi seçin ve sonra da **Bilgi**'yi seçin.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. \<Kiracı\> adı tarafından **yönetilen** sayfada, aşağıdaki şekilde gösterildiği gibi bir Yönetim **Sunucusu Adresi** içeren Bağlantı **bilgilerini** görebilirsiniz. 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Yönetilmeyen bir uygulamaya şirket verilerini yapıştıramayacağınızı doğrulayın**
  
1. Microsoft 365 İş tarafından yüklenmiş olan Outlook 2016'yı açın.
    
2. Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.
    
    Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.
    
    Uygulamanın içeriğe erişemediğini belirten bir hata alırsınız.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Kullanıcıların kişisel cihazlarındaki kişisel dosyalarına şirket verilerini kopyalayamadıklarını doğrulama

 **Bağlantı ayarlarını doğrulama**
  
1. Yerel bir kullanıcı olarak oturum açtığınız Windows 10 kişisel cihazınızda **Windows Ayarları'na**gidin ve **HesaplarA** \> **Erişim çalışmasına veya okuluna**tıklayın veya dokunun.
    
2. **İş yeri veya okula eriş** alanının altında **Bağlan**'ı seçin.
    
3. **İş yeri veya okul hesabı oluştur iletişim kutusu** \> **Oturum aç** için Microsoft 365 İş kimlik bilgilerinizi girin.
    
4. **İş yeri veya okula eriş** sayfasında, **İş veya okul hesabı**'nı ve sonra da **Bilgi**'yi seçin.
    
    ![İş veya okul hesabı iletişim kutusundaKi Bilgiler'i tıklatın veya dokunun.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Access **çalışmasında veya okul** sayfasında, aşağıdaki şekilde gösterildiği gibi bir **Yönetim Sunucusu Adresi** içeren ve içindeki *silme* ve *mam* sözcülerini içeren **Bağlantı bilgilerini** görebilirsiniz. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Yönetilmeyen bir uygulamaya şirket verilerini yapıştıramayacağınızı doğrulayın**
  
1. Outlook 2016'yı açın, gerekirse Microsoft 365 İş hesabınızı ekleyin ve Microsoft 365 İş kimlik bilgilerinizle oturum açın.
    
2. Bir e-postayı açın ve içeriğinin bir bölümünü kopyalayın.
    
    Not Defteri'ni açın ve içeriği oraya yapıştırmayı deneyin.
    
    App'in içeriğe erişemediğini belirten bir hata alırsınız.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Öte yandan, içeriği Word 2016'yı yapıştırabilirsiniz.
    

