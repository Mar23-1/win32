---
Description: 'Copy this rule.'
ms.assetid: 'b418de78-1e79-4048-81ad-8f1809038cd7'
title: 'CloneObject method of the MSFT\_NetConSecRule class'
---

# CloneObject method of the MSFT\_NetConSecRule class

Copy this rule.

## Syntax


```mof
uint32 CloneObject(
  [in]�string NewName,
  [in]�string NewPolicyStore,
  [in]�string NewGPOSession
);
```



## Parameters

<dl> <dt>

*NewName* \[in\]
</dt> <dd>

The new name for the rule.

</dd> <dt>

*NewPolicyStore* \[in\]
</dt> <dd>

The new policy store for the rule.

</dd> <dt>

*NewGPOSession* \[in\]
</dt> <dd>

The new GPOSession for the rule.

</dd> </dl>

## Requirements



|                                     |                                                                                        |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�8<br/>                                                                   |
| Minimum supported server<br/> | Windows Server�2012<br/>                                                         |
| Namespace<br/>                | Root\\StandardCimv2<br/>                                                         |
| MOF<br/>                      | <dl> <dt>WFasCim.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>WFasCim.dll</dt> </dl> |



## See also

<dl> <dt>

[**MSFT\_NetConSecRule**](msft-netconsecrule.md)
</dt> </dl>

�

�



