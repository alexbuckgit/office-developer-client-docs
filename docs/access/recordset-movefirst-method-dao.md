---
title: "Recordset.MoveFirst Method (DAO)"
 
 
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
  
localization_priority: Normal
ms.assetid: 338f7e86-6997-b80a-fc7a-a395d10b4a62
description: "Moves to the first record in a specified Recordset object and make that record the current record."
---

# Recordset.MoveFirst Method (DAO)

Moves to the first record in a specified **Recordset** object and make that record the current record. 
  
## Syntax

 *expression*  . **MoveFirst**
  
 *expression*  A variable that represents a **Recordset** object. 
  
## Remarks

Use the **Move** methods to move from record to record without applying a condition. 
  
If you edit the current record, be sure you use the **Update** method to save the changes before you move to another record. If you move to another record without updating, your changes are lost without warning. 
  
When you open a **Recordset**, the first record is current and the **BOF** property is **False**. If the **Recordset** contains no records, the **BOF** property is **True**, and there is no current record. 
  
If the first or last record is already current when you use **MoveFirst** or **MoveLast**, the current record doesn't change. 
  
If  _recordset_ refers to a table-type **Recordset** (Microsoft Access workspaces only), movement follows the current index. You can set the current index by using the **Index** property. If you don't set the current index, the order of returned records is undefined. 
  
You can't use the **MoveFirst**, **MoveLast**, and **MovePrevious** methods on a forward-only-type **Recordset** object. 
  
To move the position of the current record in a **Recordset** object a specific number of records forward or backward, use the **Move** method. 
  
