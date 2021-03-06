---
title: ftp literal_1
description: Reference topic for **** - 

ms.prod: windows-server


ms.technology: manage-windows-commands

ms.topic: article
ms.assetid: fb81aa2d-07fa-4e79-bf44-1fb5526fdf14 vhorne
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/16/2017
---
# ftp: literal_1

> Applies to: Windows Server (Semi-Annual Channel), Windows Server 2019, Windows Server 2016, Windows Server 2012 R2, Windows Server 2012
Sends verbatim arguments to the remote ftp server. A single ftp reply code is returned.   

## Syntax  
```  
literal <Argument> [ ]  
```  
#### Parameters  

| Parameter  |                    Description                    |
|------------|---------------------------------------------------|
| <Argument> | Specifies the argument to send to the ftp server. |

## Remarks  
The **literal** command is identical to the **quote** command.  
## Examples  
Send a **quit** command to the remote ftp server.  
```  
literal quit  
```  
## Additional References  
-   [ftp: quote](ftp-quote.md)  
-   - [Command-Line Syntax Key](command-line-syntax-key.md)  
