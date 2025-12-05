This GitHub repository is used to store backups of all of the meeting minutes, and other major documents, from the Wang Fuk Court Incorporated Owners' website.
> http://www.wangfuk.org/html/home/index.asp

---

### Service Outage Report: December 3, 2025

Starting around the evening of December 3, 2025 (Hong Kong Time), the website’s homepage suddenly became inaccessible and displayed the error: `HTTP Error 404.0 - Not Found`. It had been functioning normally before that.

![](https://github.com/sparktsang/wangfuk/blob/main/Error.jpg)

**Incident Analysis: Server-Side Failure vs. Protocol Error**

It has been [suggested](https://github.com/Hong-Kong-Emergency-Coordination-Hub/Hong-Kong-Fire-Documentary/issues/256#issuecomment-3612794080) that this downtime was caused by inadvertently using the HTTPS protocol. However, the forensic evidence proves otherwise:

1.  **The Error Page Distinction:** The screenshot above shows a **Native IIS 404.0 Error** (white background). This is a low-level server error indicating that the IIS web server itself was unable to map requests to the application directory.
2.  **HTTPS Behavior:** Accessing the site via HTTPS (which is currently misconfigured) results in a [**Plesk Custom Error** page](https://github.com/sparktsang/wangfuk/blob/main/HTTPS_error.png).

The presence of the raw IIS error confirms that this was a **server-side infrastructure failure** (system maintenance or configuration detachment) and not a client-side protocol mismatch. See also the [detailed analysis of this error](https://github.com/sparktsang/wangfuk/blob/main/error_analysis.md). 

By around 11:50 p.m. on the same day, the homepage returned to normal functionality via HTTP.

---

The meeting minutes from 2024-12-18 to 2025-11-07 have been consolidated into Markdown format as follows.

https://github.com/sparktsang/wangfuk/blob/main/MINUTES_MARKDOWN.md

---

法團網站中，2018年12月18日第十屆第九次全體委員會議記錄之連結有誤，導向至2021年11月17日第十一屆第九次全體委員會議記錄。因此，2018年12月18日第十屆第九次全體委員會議記錄缺漏。

第九屆全體委員會議記錄中，多項「會議議程」於網站缺漏，但「會議紀錄」完整。

2018年9月7日特別業主大會議程連結有誤，導向至同日會議紀錄。是故，當日議程缺漏。

強制驗樓驗窗計劃 2. 及 3. 各導向以下連結，均已失效。
* https://www.bd.gov.hk/chineseT/services/index_MBIS_MWIS.html
* https://www.bd.gov.hk/chineseT/documents/guideline/GGMBISMWIS.pdf

強制驗樓驗窗計劃 10. 非文件，係導向以下連結。
https://smarttender.brplatform.org.hk/zh-HK/index.htm

---

To batch download the files from this repository, you may enter its URL into the following website: 

https://download-directory.github.io/

---

The following files are too large and have therefore been uploaded separately to MEGA Cloud Storage: https://mega.nz/folder/M5cHHAYa#W0VxI6dDM1b6fpf4K9Ma1w
* 大維修相關資訊 2. 工程解說會簡報(宏業及鴻毅).pdf
* 大維修相關資訊 8. 特別業主大會解說會簡報(14-3-2025).pdf 
* 宏福通訊 第12屆管理委員會-第4期.pdf
* 宏福通訊 第12屆管理委員會-第5期.pdf
* 宏福通訊 第12屆管理委員會-第9期.pdf

---

This is part of a [project](https://sparktsang.github.io/life/2025/12/04/status.html) which examines the tragic fire at Wang Fuk Court during renovation works, which resulted in over 150 deaths.

---

**Special thanks** to **Eric** for selflessly coming to the rescue; with his professional data analytics skills, he organized a large volume of files, enabling this backup project to be completed.
