---
title: manage-bde WipeFreeSpace
description: Reference topic for **** - 

ms.prod: windows-server


ms.technology: manage-windows-commands

ms.topic: article
ms.assetid: b8d83a2a-c5c8-4019-9041-23d1d6abf282
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/16/2017
---

# manage-bde: WipeFreeSpace



Wipes the free space on the volume removing any data fragments that may have existed in the space. Running this command on a volume that was encrypted using the Used Space Only encryption method provides the same level of protection as the Full Volume Encryption encryption method.

## Syntax

```
manage-bde -WipeFreeSpace|-w [<Drive>] [-Cancel] [-computername <Name>] [{-?|/?}] [{-help|-h}]
```

#### Parameters

|Parameter|Description|
|---------|-----------|
|\<Drive>|Represents a drive letter followed by a colon, a volume GUID path, or a mounted volume.|
|-Cancel|Cancels a wipe of free space that is in process.|
|-computername|Specifies that Manage-bde.exe will be used to modify BitLocker protection on a different computer. You can also use **-cn** as an abbreviated version of this command.|
|\<Name>|Represents the name of the computer on which to modify BitLocker protection. Accepted values include the computer's NetBIOS name and the computer's IP address.|
|-? or /?|Displays brief Help at the command prompt.|
|-help or -h|Displays complete Help at the command prompt.|

## Examples

To illustrates using the **-w** command to create wipe the free space on drive C.
```
manage-bde -w C:
```
To illustrates using the **-w** command with the **-cancel** parameter to cancel the wipe the free space on drive C.
```
manage-bde -w -Cancel C:
```

## Additional References

-   - [Command-Line Syntax Key](command-line-syntax-key.md)
-   [Manage-bde](manage-bde.md)