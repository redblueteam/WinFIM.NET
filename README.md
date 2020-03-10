# WinFIM.NET
WinFIM.NET - File Integrity Monitoring For Windows

For detail introduction, please visit my <a href="https://redblueteam.wordpress.com/2020/03/11/winfim-net-windows-file-integrity-monitoring/"> My Cyber Security Corner</a>.

<b>#Introduction</b>
There are plenty of commercial tools to do file integrity monitoring (FIM). But, for freeware / Open Source, especially for Windows, it seems not much options.

I have developed a small Windows Service named “WinFIM.NET” (https://github.com/redblueteam/WinFIM.NET) trying to fill up this gap.

<b>#characteristics</b>
The characteristics of this small application are:

-It will identify add / remove / modify of files and directories
- Monitoring scope could be easily customized
- Path exclusion (e.g. sub-directory) could be configured
- File extension could be configured (e.g. *.bak, *.tmp, *.log, *.mdf, *.ldf, *.xel, *. installlog)
- All the events are saved as native Windows Events, which could easily integrate with users’ existing log management mechanism (e.g. Windows Event Subscription, Winlogbeat , nxlog, etc.)
- Deployment friendly
- Using SHA256 for hashing
