# 注意:這只是個人製作自用的程式碼，若要使用的話需要自行更改檔案位置!
## windows
```
@echo off
title ECLIPSE備份 Version 0 Beta 6.1D "NOT AUTOMATIC!!"
:Z
color F
:A
cls
echo 輸入"exit"即可退出
set /p copy=請輸入隨身碟磁區編號(D~I不分大小寫,不要輸入符號):
if /i "%copy%" EQU "D" goto DSA
if /i "%copy%" EQU "E" goto ESA
if /i "%copy%" EQU "F" goto FSA
if /i "%copy%" EQU "G" goto GSA
if /i "%copy%" EQU "H" goto HSA
if /i "%copy%" EQU "I" goto ISA
if /i "%copy%" EQU "exit" goto ET
echo 輸入錯誤，重新輸入
pause
goto A


:DSA
echo 備份操作: "1"從隨身碟備份到I2604電腦 "2"從I2604電腦備份到隨身碟 "3"從筆記型電腦備份到隨身碟 "4"從隨身碟備份到筆記型電腦
echo 注意!!!!!紅色顯示時請不要關閉視窗，以免資料遺失!!
echo 輸入"ex"即可返回，"exit"即可退出
:DSA1
set /p copy=請輸入數字(不要輸入小數點):
if /i "%copy%" EQU "1" goto 11
if /i "%copy%" EQU "2" goto 12
if /i "%copy%" EQU "3" goto 13
if /i "%copy%" EQU "4" goto 14
if /i "%copy%" EQU "exit" goto ET
if /i "%copy%" EQU "ex" goto E
echo 輸入錯誤，重新輸入
pause
goto DSA1
:11
color C
echo 請稍後...
del E:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy D:\eclipse___AAJS\516027\eclipse-workspace E:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:12
color C
echo 請稍後...
del D:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy E:\eclipse___AAJS\516027\eclipse-workspace D:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:13
color C
echo 請稍後...
del D:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace D:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:14
color C
echo 請稍後...
del C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy D:\eclipse___AAJS\516027\eclipse-workspace C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z


:ESA
echo 備份操作:"1"從筆記型電腦備份到隨身碟 "2"從隨身碟備份到筆記型電腦
echo 注意!!!!!紅色顯示時請不要關閉視窗，以免資料遺失!!
echo 輸入"ex"即可返回，"exit"即可退出
:ESA1
set /p copy=請輸入數字(不要輸入小數點):
if /i "%copy%" EQU "1" goto 21
if /i "%copy%" EQU "2" goto 22
if /i "%copy%" EQU "exit" goto ET
if /i "%copy%" EQU "ex" goto E
echo 輸入錯誤，重新輸入
pause
goto ESA1
:21
color C
echo 請稍後...
del E:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace E:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:22
color C
echo 請稍後...
del C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy E:\eclipse___AAJS\516027\eclipse-workspace C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z

:FSA
echo 備份操作: "1"從隨身碟備份到I2604電腦 "2"從I2604電腦備份到隨身碟 "3"從筆記型電腦備份到隨身碟 "4"從隨身碟備份到筆記型電腦
echo 注意!!!!!紅色顯示時請不要關閉視窗，以免資料遺失!!
echo 輸入"ex"即可返回，"exit"即可退出
:FSA1
set /p copy=請輸入數字(不要輸入小數點):
if /i "%copy%" EQU "1" goto 1
if /i "%copy%" EQU "2" goto 2
if /i "%copy%" EQU "3" goto 3
if /i "%copy%" EQU "4" goto 4
if /i "%copy%" EQU "exit" goto ET
if /i "%copy%" EQU "ex" goto E
echo 輸入錯誤，重新輸入
pause
goto FSA1
:1
color C
echo 請稍後...
del E:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy F:\eclipse___AAJS\516027\eclipse-workspace E:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:2
color C
echo 請稍後...
del F:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy E:\eclipse___AAJS\516027\eclipse-workspace F:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:3
color C
echo 請稍後...
del F:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace F:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:4
color C
echo 請稍後...
del C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy F:\eclipse___AAJS\516027\eclipse-workspace C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z

:GSA
echo 備份操作: "1"從隨身碟備份到I2604電腦 "2"從I2604電腦備份到隨身碟 "3"從筆記型電腦備份到隨身碟 "4"從隨身碟備份到筆記型電腦
echo 注意!!!!!紅色顯示時請不要關閉視窗，以免資料遺失!!
echo 輸入"ex"即可返回，"exit"即可退出
:GSA1
set /p copy=請輸入數字(不要輸入小數點):
if /i "%copy%" EQU "1" goto 31
if /i "%copy%" EQU "2" goto 32
if /i "%copy%" EQU "3" goto 33
if /i "%copy%" EQU "4" goto 34
if /i "%copy%" EQU "exit" goto ET
if /i "%copy%" EQU "ex" goto E
echo 輸入錯誤，重新輸入
pause
goto GSA1
:31
color C
echo 請稍後...
del E:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy G:\eclipse___AAJS\516027\eclipse-workspace E:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:32
color C
echo 請稍後...
del G:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy E:\eclipse___AAJS\516027\eclipse-workspace G:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:33
color C
echo 請稍後...
del G:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace G:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:34
color C
echo 請稍後...
del C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy G:\eclipse___AAJS\516027\eclipse-workspace C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z

:HSA
echo 備份操作: "1"從隨身碟備份到I2604電腦 "2"從I2604電腦備份到隨身碟 "3"從筆記型電腦備份到隨身碟 "4"從隨身碟備份到筆記型電腦
echo 注意!!!!!紅色顯示時請不要關閉視窗，以免資料遺失!!
echo 輸入"ex"即可返回，"exit"即可退出
:HSA1
set /p copy=請輸入數字(不要輸入小數點):
if /i "%copy%" EQU "1" goto 5
if /i "%copy%" EQU "2" goto 6
if /i "%copy%" EQU "3" goto 7
if /i "%copy%" EQU "4" goto 8
if /i "%copy%" EQU "exit" goto ET
if /i "%copy%" EQU "ex" goto E
echo 輸入錯誤，重新輸入
pause
cls
goto HSA1
:5
color C
echo 請稍後...
del E:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy H:\eclipse___AAJS\516027\eclipse-workspace E:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:6
color C
echo 請稍後...
del H:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy E:\eclipse___AAJS\516027\eclipse-workspace H:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:7
color C
echo 請稍後...
del H:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace H:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:8
color C
echo 請稍後...
del C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy H:\eclipse___AAJS\516027\eclipse-workspace C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z


:ISA
echo 備份操作: "1"從隨身碟備份到I2604電腦 "2"從I2604電腦備份到隨身碟 "3"從筆記型電腦備份到隨身碟 "4"從隨身碟備份到筆記型電腦
echo 注意!!!!!紅色顯示時請不要關閉視窗，以免資料遺失!!
echo 輸入"ex"即可返回，"exit"即可退出
:ISA1
set /p copy=請輸入數字(不要輸入小數點):
if /i "%copy%" EQU "1" goto 9
if /i "%copy%" EQU "2" goto 10
if /i "%copy%" EQU "3" goto 11
if /i "%copy%" EQU "4" goto 12
if /i "%copy%" EQU "exit" goto ET
if /i "%copy%" EQU "ex" goto E
echo 輸入錯誤，重新輸入
pause
goto ISA1
:9
color C
echo 請稍後...
del E:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy I:\eclipse___AAJS\516027\eclipse-workspace E:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:10
color C
echo 請稍後...
del I:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy E:\eclipse___AAJS\516027\eclipse-workspace I:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:11
color C
del C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy I:\eclipse___AAJS\516027\eclipse-workspace C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z
:12
color C
del I:\eclipse___AAJS\516027\eclipse-workspace /F /S /Q
xcopy C:\Users\%username%\Desktop\eclipse___AAJS\516027\eclipse-workspace I:\eclipse___AAJS\516027\eclipse-workspace /E /R /Y
color A
echo 已完成!!
pause
cls
goto Z

:E
cls
goto Z

:ET
cls
exit
```
