---
title: "UML Sequence Diagrams: Reference"
ms.custom: na
ms.date: 10/03/2016
ms.prod: visual-studio-tfs-dev14
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 366fc324-aeeb-4894-bd13-ec2e40754b8e
caps.latest.revision: 41
manager: kamrani
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
# UML Sequence Diagrams: Reference
In Visual Studio, a *sequence diagram* shows an interaction, which represents the sequence of messages between instances of classes, components, subsystems, or actors. Time flows down the diagram, and it shows the flow of control from one participant to another. Use sequence diagrams to visualize instances and events, instead of classes and methods. More than one instance of the same type can appear on the diagram. More than one occurrence of the same message can also appear.  
  
 UML sequence diagrams are part of a UML model and exist only within UML modeling projects. To create a UML sequence diagram, on the **Architecture** menu, click **New UML or Layer Diagram**. Find out more about how to create and draw [UML sequence diagrams](../VS_IDE/UML-Sequence-Diagrams--Guidelines.md) or [UML modeling diagrams](../VS_IDE/Edit-UML-models-and-diagrams.md) in general.  
  
 To see which versions of Visual Studio support this feature, see [Version support for architecture and modeling tools](../VS_IDE/What-s-new-for-design-in-Visual-Studio.md#VersionSupport).  
  
## Reading Sequence Diagrams  
 The following table describes the elements that you can see on a sequence diagram. Find out more about these [elements' properties](../VS_IDE/Properties-of-elements-on-UML-sequence-diagrams.md).  
  
 ![Parts of a sequence diagram](../VS_IDE/media/UML_Sequence.png "UML_Sequence")  
  
|**Shape**|**Element**|**Description**|  
|---------------|-----------------|---------------------|  
|1|**Lifeline**|A vertical line that represents the sequence of events that occur in a participant during an interaction, while time progresses down the line. This participant can be an instance of a class, component, or actor.|  
|2|**Actor**|A participant that is external to the system that you are developing.<br /><br /> You can make an actor symbol appear at the top of a lifeline by setting its **Actor** property.|  
|3|**Synchronous message**|The sender waits for a response to a synchronous message before it continues. The diagram shows both the call and the return. Synchronous messages are used to represent ordinary function calls within a program, as well as other kinds of message that behave in the same way.|  
|4|**Asynchronous message**|A message that does not require a response before the sender continues. An asynchronous message shows only a call from the sender. Use to represent communication between separate threads or the creation of a new thread.|  
|5|**Execution occurrence**|A vertical shaded rectangle that appears on a participant's lifeline and represents the period when the participant is executing an operation.<br /><br /> The execution begins where the participant receives a message. If the initiating message was a synchronous message, the execution ends with a «return» arrow back to the sender.|  
|6|**Callback message**|A message that returns back to a participant that is waiting for the return from an earlier call. The resulting execution occurrence appears on top of the existing one.|  
|7|**Self message**|A message from a participant to itself. The resulting execution occurrence appears on top of the sending execution.|  
|8|**Create message**|A message that creates a participant. If a participant receives a create message, it should be the first it receives.|  
|9|**Found message**|An asynchronous message from an unknown or an unspecified participant.|  
|10|**Lost message**|An asynchronous message to an unknown or an unspecified participant.|  
|11|**Comment**|A comment can be attached to any point on a lifeline.|  
|12|**Interaction Use**|Encloses a sequence of messages that are defined in another diagram.<br /><br /> To create an **Interaction Use**, click the tool and then drag across the lifelines you want to include.|  
|13|**Combined Fragment**|A collection of fragments. Each fragment can enclose one or more messages. There are different kinds of combined fragments. For more information, see [Describe control flow with fragments on UML sequence diagrams](../VS_IDE/Describe-control-flow-with-fragments-on-UML-sequence-diagrams.md).<br /><br /> To create a fragment, right-click a message, point to **Surround With**, and then click a fragment type.|  
|14|**Fragment Guard**|Can be used to state a condition relevant to whether the fragment will occur.<br /><br /> To set the guard, select a fragment, then select the guard, and type a value.|  
|**X**|**Destruction Event**|Represents the point at which the object is deleted or no longer accessible. Appears at the bottom of every lifeline.|  
||**Interaction**|The collection of messages and lifelines that is displayed in the sequence diagram. To view the properties of an Interaction, you must select it in **UML Model Explorer**.|  
||**Sequence Diagram**|The diagram that displays an Interaction. To view its properties, click on an empty part of the diagram. **Note:**  The names of the Sequence Diagram, the Interaction that it displays, and the file that contains the diagram can all be different.|  
  
## See Also  
 [UML Sequence Diagrams: Guidelines](../VS_IDE/UML-Sequence-Diagrams--Guidelines.md)   
 [Edit UML models and diagrams](../VS_IDE/Edit-UML-models-and-diagrams.md)   
 [UML Use Case Diagrams: Reference](../VS_IDE/UML-Use-Case-Diagrams--Reference.md)   
 [UML Class Diagrams: Reference](../VS_IDE/UML-Class-Diagrams--Reference.md)   
 [UML Component Diagrams: Reference](../VS_IDE/UML-Component-Diagrams--Reference.md)   
 [UML Component Diagrams: Reference](../VS_IDE/UML-Component-Diagrams--Reference.md)