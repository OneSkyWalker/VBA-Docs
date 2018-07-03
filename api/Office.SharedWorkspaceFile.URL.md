---
title: SharedWorkspaceFile.URL Property (Office)
keywords: vbaof11.chm266001
f1_keywords:
- vbaof11.chm266001
ms.prod: office
api_name:
- Office.SharedWorkspaceFile.URL
ms.assetid: cbdcb807-235b-2904-8407-0cb276c6d342
ms.date: 06/08/2017
---


# SharedWorkspaceFile.URL Property (Office)

Gets the full Uniform Resource Locator (URL) and file name of the shared workspace file. Read-only.

> [!NOTE] 
> Beginning with Microsoft Office 2010, this object or member has been deprecated and should not be used.


## Syntax

 _expression_. `URL`

 _expression_ A variable that represents a [SharedWorkspaceFile](./Office.SharedWorkspaceFile.md) object.


### Return Value

String


## Remarks

The  **URL** property returns the address of the shared workspace file in this format: `http://server/sites/user/workspace/Shared%Documents/MyWorkbook.xls`. The  **URL** property returns a URL-encoded string. For example, a space in the folder name is represented by %20. The **SharedWorkspaceFile** object does not have a **Name** or **FileName** property. The filename must be extracted from the **URL** property.


## Example

The following example displays the URL of the shared workspace file.


```vb
MsgBox "URL: " &amp; ActiveWorkbook.SharedWorkspaceFile.URL, _ 
        vbInformation + vbOKOnly, "Shared Workspace File URL"
```


## See also


[SharedWorkspaceFile Object](Office.SharedWorkspaceFile.md)



[SharedWorkspaceFile Object Members](./overview/sharedworkspacefile-members-office.md)
