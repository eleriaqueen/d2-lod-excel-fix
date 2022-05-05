# Diablo II - LOD - "Excel" Fix

Allow "Diablo II - Lord of Destruction" to load and use tabbed txt files while they are open in an Excel-like application.

The goal is to set the flag FILE_SHARE_WRITE (0x00000002) in addition to FILE_SHARE_READ (0x00000001) before the game calls CreateFileA().

## Details

This repository contains enough info to be able to manually patch most Storm.dll versions with the fix.

## Thanks

Yohann Nicolas : Finding the right ordinal to patch was quick thanks to their 1.11b fix for this issue.
