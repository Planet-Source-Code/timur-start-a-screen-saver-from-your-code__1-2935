<div align="center">

## Start a screen saver from your code \!\!\!


</div>

### Description

This code, you may insert in your program, allows to start a screensaver.

Many other usefull solutions you'll find on my site: http://www.netcity.ru/~timur555/

Glad to see you !!!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Timur](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/timur.md)
**Level**          |Unknown
**User Rating**    |4.2 (162 globes from 39 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__1-1.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/timur-start-a-screen-saver-from-your-code__1-2935/archive/master.zip)

### API Declarations

```
Private Declare Function SendMessage Lib "User32" Alias "SendMessageA" ( _
  ByVal hWnd As Long, _
  ByVal wMsg As Long, _
  ByVal wParam As Long, _
  ByVal lParam As Long) As Long
Private Const WM_SYSCOMMAND = &H112&
Private Const SC_SCREENSAVE = &HF140&
```


### Source Code

```
'Place this two lines of code any where in your program
'...
'enjoy!
 Dim tmp As Long
 tmp = SendMessage(Me.hWnd, WM_SYSCOMMAND, SC_SCREENSAVE, 0&)
```

