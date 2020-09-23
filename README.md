<div align="center">

## Detect "\\" in directory


</div>

### Description

Suppose You try to get the app.path when the app is in the C Drive. the result is "C:\". if the app is in another directory the result may be "C:\Directory". notice there is no backslash. most people skip this because they don't think it is a problem, but it is. when you put in a program, app.path & "\filename.file", when it is in the C Drive or if you put app.path & "filename.file" in a named directory, the computer will either return "C:\\filename.file" or "C:\Directoryfilename.file". this code will show you how to detect the backslash and deal with it.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Eric LeBourgeois](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/eric-lebourgeois.md)
**Level**          |Beginner
**User Rating**    |2.7 (24 globes from 9 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__1-43.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/eric-lebourgeois-detect-in-directory__1-10775/archive/master.zip)





### Source Code

```
'this code will give you a valid filename, whether the app.path return has a backslash or not, and displays a message box.
'Please Vote for me at Planet Source Code
if right(app.path,1) = "\" then 'sees if the directory has a backslash at the end of it
msgbox app.path & "filename.file"
goto ResumeMe
end if
msgbox app.path & "\filename.file"
ResumeMe:
```

