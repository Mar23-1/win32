---
title: Api.TryMovePrevious method  (Microsoft.Isam.Esent.Interop)
TOCTitle: 'TryMovePrevious method '
ms:assetid: M:Microsoft.Isam.Esent.Interop.Api.TryMovePrevious(Microsoft.Isam.Esent.Interop.JET_SESID,Microsoft.Isam.Esent.Interop.JET_TABLEID)
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.isam.esent.interop.api.trymoveprevious(v=EXCHG.10)
ms:contentKeyID: 55100940
ms.date: 07/30/2014
ms.topic: article
f1_keywords:
- Microsoft.Isam.Esent.Interop.Api.TryMovePrevious
dev_langs:
- CSharp
- JScript
- VB
- other
api_name: 
- Microsoft.Isam.Esent.Interop.Api.TryMovePrevious
topic_type: 
- kbSyntax
- apiref
api_type: 
- Managed
api_location: 
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW

---

# Api.TryMovePrevious method

Try to move to the previous record in the table. If there is not a previous record this returns false, if a different error is encountered an exception is thrown.

**Namespace:**  [Microsoft.Isam.Esent.Interop](hh596136\(v=exchg.10\).md)  
**Assembly:**  Microsoft.Isam.Esent.Interop (in Microsoft.Isam.Esent.Interop.dll)

## Syntax

``` vb
'Declaration
Public Shared Function TryMovePrevious ( _
    sesid As JET_SESID, _
    tableid As JET_TABLEID _
) As Boolean
'Usage
Dim sesid As JET_SESID
Dim tableid As JET_TABLEID
Dim returnValue As Boolean

returnValue = Api.TryMovePrevious(sesid, _
    tableid)
```

``` csharp
public static bool TryMovePrevious(
    JET_SESID sesid,
    JET_TABLEID tableid
)
```

#### Parameters

  - sesid  
    Type: [Microsoft.Isam.Esent.Interop.JET_SESID](hh596745\(v=exchg.10\).md)  
    
    The session to use.

<!-- end list -->

  - tableid  
    Type: [Microsoft.Isam.Esent.Interop.JET_TABLEID](hh566310\(v=exchg.10\).md)  
    
    The cursor to position.

#### Return value

Type: [System.Boolean](https://msdn.microsoft.com/en-us/library/a28wyd50)  
True if the move was successful.  

## See also

#### Reference

[Api class](dn292211\(v=exchg.10\).md)

[Api members](dn292213\(v=exchg.10\).md)

[Microsoft.Isam.Esent.Interop namespace](hh596136\(v=exchg.10\).md)
