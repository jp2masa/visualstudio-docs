---
title: "Debugger Cannot Display Source Code or Disassembly | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-debug"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "CSharp"
  - "VB"
  - "FSharp"
  - "C++"
helpviewer_keywords: 
  - "disassembly code, errors"
ms.assetid: 112d3ea3-fdd2-4bce-92b4-167a76258934
caps.latest.revision: 7
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# Debugger Cannot Display Source Code or Disassembly
This error reads:  
  
 The debugger cannot display source code or disassembly for the current location where execution has stopped.  
  
 This error message can occur for a number of reasons:  
  
-   You may have hit a breakpoint in a location for which there is no source code, while debugging a language that doesn't support disassembly. Open the **Breakpoints** window, locate the breakpoint, and delete it.  
  
-   If you are debugging script, you may have hit a breakpoint while there were no threads in your program. Choose **Step** or **Continue** from the **Debug** menu to resume debugging.  
  
-   Security considerations may have prevented the debugger from reading stack, thread, register, and other context information from the program you are debugging. This is most likely to happen if you are debugging a Web application and don't have the right permission to access the virtual directory. Set security for the virtual directory to Anonymous and try again.  
  
## See Also  
 [Debugging in Visual Studio](../debugger/index.md) 
 [Debugger Feature Tour](../debugger/debugger-feature-tour.md)   
 [Viewing Data in the Debugger](../debugger/viewing-data-in-the-debugger.md)