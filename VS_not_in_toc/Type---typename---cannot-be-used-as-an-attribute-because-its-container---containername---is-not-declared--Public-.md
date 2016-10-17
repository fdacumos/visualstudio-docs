---
title: "Type &#39;&lt;typename&gt;&#39; cannot be used as an attribute because its container &#39;&lt;containername&gt;&#39; is not declared &#39;Public&#39;"
ms.custom: na
ms.date: 10/02/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 3d1a8f41-8652-4e37-a6bd-40b0ad306c6f
caps.latest.revision: 7
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
# Type &#39;&lt;typename&gt;&#39; cannot be used as an attribute because its container &#39;&lt;containername&gt;&#39; is not declared &#39;Public&#39;
The class or module where this attribute is defined is not declared using the `Public` modifier. Classes and modules that do not specify an access modifier are declared as `Friend` by default.  
  
 **Error ID:** BC31517  
  
### To correct this error  
  
1.  Add the `Public` modifier to the class or module where this attribute is defined.  
  
## See Also  
 [Public](../Topic/Public%20\(Visual%20Basic\).md)