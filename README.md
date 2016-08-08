# 4d-macros
## Macros for 4D Developers

#### Easy Installation:

1) Run this method:

```
// install macro
C_LONGINT($code)
C_BLOB($macroBlob)
C_TEXT($macroFileURL;$macroFolder;$macroFileOnDisk)
$macroFolder:=Get 4D folder(Active 4D Folder)+"Macros v2"
$macroFileURL:="https://github.com/tpenner/4d-macros/raw/master/Macros%20v2/aaMyMacros.xml"
$macroFileOnDisk:=$macroFolder+Folder separator+"tpenner_macros.xml"
$code:=HTTP Get($macroFileURL;$macroBlob)
If ($code=200)
BLOB TO DOCUMENT($macroFileOnDisk;$macroBlob)
End if 
```

---

#### Manual Installation:

1) Download the [latest macro file][1]
[1]: https://github.com/tpenner/4d-macros/raw/master/Macros%20v2/aaMyMacros.xml

2) Place the `aaMyMacros.xml` file in to the following location:
* Windows: `C:\Users\username\AppData\Roaming\4D\Macros v2`
* Mac OS X: `/Users/username/Application Data/4D/Macros v2/`

---
