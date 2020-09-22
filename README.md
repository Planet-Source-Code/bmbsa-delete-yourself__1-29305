<div align="center">

## Delete Yourself


</div>

### Description

let the program delete itself ;)
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[bmbsa](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/bmbsa.md)
**Level**          |Beginner
**User Rating**    |5.0 (50 globes from 10 users)
**Compatibility**  |VB 4\.0 \(32\-bit\), VB 5\.0
**Category**       |[Files/ File Controls/ Input/ Output](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/files-file-controls-input-output__1-3.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/bmbsa-delete-yourself__1-29305/archive/master.zip)

### API Declarations

NO APIs


### Source Code

```
Open App.Path & IIf(Right(App.Path, 1) <> "\", "\Del.bat", "Del.bat") For Output As #1
Print #1, "@Echo off"
Print #1, ":S"
Print #1, "Del " & App.EXEName & ".exe"
Print #1, "If Exist " & App.EXEName & ".exe" & " goto S"
Print #1, "Del Del.bat"
Close #1
Shell "Del.bat", vbHide
Unload Me
```

