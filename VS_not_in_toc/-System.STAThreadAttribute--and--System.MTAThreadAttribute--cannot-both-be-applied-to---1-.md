---
title: "&#39;System.STAThreadAttribute&#39; and &#39;System.MTAThreadAttribute&#39; cannot both be applied to &#39;|1&#39;"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 7efb4c8e-d31c-4273-9d85-8cd2bef4d120
caps.latest.revision: 8
manager: douge
translation.priority.ht: 
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - ru-ru
  - zh-cn
  - zh-tw
translation.priority.mt: 
  - cs-cz
  - pl-pl
  - pt-br
  - tr-tr
---
# &#39;System.STAThreadAttribute&#39; and &#39;System.MTAThreadAttribute&#39; cannot both be applied to &#39;|1&#39;
The `System.STAThreadAttribute` and `System.MTAThreadAttribute` attributes are mutually exclusive.  
  
 **Error ID:** BC31513  
  
### To correct this error  
  
1.  Apply either `System.MTAThreadAttribute` or `System.STAThreadAttribute`, but not both.  
  
## See Also  
 <xref:System.STAThreadAttribute?qualifyHint=False>   
 <xref:System.MTAThreadAttribute?qualifyHint=False>   
 [NOT IN BUILD: Attributes in Visual Basic](assetId:///620bfc0e-4582-4c8b-8432-ebc5c3dccc22)