# Diablo II - LOD - "Excel" Fix

Allow "Diablo II - Lord of Destruction" to load and use tabbed txt files while they are open in an Excel type application.

## How to use the info in this repository

Bare minimum you need a hexadecimal editor and need to know how to search for and how to modify hex values using this type of software.

Recommended hex editor : [ImHex](https://github.com/WerWolv/ImHex)

## Details

Target: SFileOpenFileEx (Storm.dll Ordinal 268).

Method : Add FILE_SHARE_WRITE (0x02) to the call to [CreateFileA()](https://docs.microsoft.com/en-us/windows/win32/api/fileapi/nf-fileapi-createfilea)

## Thanks

Yohann Nicolas : Finding the right ordinal to patch was quick thanks to their 1.11b fix for this issue.
