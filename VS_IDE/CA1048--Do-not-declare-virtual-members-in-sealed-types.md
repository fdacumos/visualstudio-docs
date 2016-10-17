---
title: "CA1048: Do not declare virtual members in sealed types"
ms.custom: na
ms.date: 10/03/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - vs-devops-test
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 5dcf4a30-6f98-48a8-b8cc-7b89ea757262
caps.latest.revision: 13
manager: douge
translation.priority.ht: 
  - cs-cz
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - pl-pl
  - pt-br
  - ru-ru
  - tr-tr
  - zh-cn
  - zh-tw
---
# CA1048: Do not declare virtual members in sealed types
|||  
|-|-|  
|TypeName|DoNotDeclareVirtualMembersInSealedTypes|  
|CheckId|CA1048|  
|Category|Microsoft.Design|  
|Breaking Change|Breaking|  
  
## Cause  
 A public type is sealed and declares a method that is both `virtual` (`Overridable` in Visual Basic) and not final. This rule does not report violations for delegate types, which must follow this pattern.  
  
## Rule Description  
 Types declare methods as virtual so that inheriting types can override the implementation of the virtual method. By definition, you cannot inherit from a sealed type, making a virtual method on a sealed type meaningless.  
  
 The Visual Basic .NET and C# compilers do not allow types to violate this rule.  
  
## How to Fix Violations  
 To fix a violation of this rule, make the method non-virtual or make the type inheritable.  
  
## When to Suppress Warnings  
 Do not suppress a warning from this rule. Leaving the type in its current state can cause maintenance issues and does not provide any benefits.  
  
## Example  
 The following example shows a type that violates this rule.  
  
 [!CODE [FxCop.Design.SealedVirtual#1](../CodeSnippet/VS_Snippets_CodeAnalysis/FxCop.Design.SealedVirtual#1)]