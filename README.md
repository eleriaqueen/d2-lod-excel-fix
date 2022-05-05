# Diablo II - LOD - "Excel" Fix

Allow "Diablo II - Lord of Destruction" to load and use tabbed txt files while they are open in an Excel-like application.

This method adds the FILE_SHARE_WRITE (0x02) flag to a specific [CreateFileA()](https://docs.microsoft.com/en-us/windows/win32/api/fileapi/nf-fileapi-createfilea) call found in Storm.dll ordinal 268.

## Details

This repository contains enough info to be able to manually patch most Storm.dll versions with the fix.

## Thanks

Yohann Nicolas : Finding the right ordinal to patch was quick thanks to their 1.11b fix for this issue.
