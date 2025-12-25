This GitHub repository stores backups of all of the meeting minutes and other documents from the Wang Fuk Court Incorporated Owners' (宏福苑業主法立案法團) website.
> http://www.wangfuk.org/html/home/index.asp

---

### Compilation of meeting minutes for accessibility

The meeting minutes from 2021-06-28 to 2025-11-07 have been consolidated into Markdown format as follows.

https://github.com/sparktsang/wangfuk/blob/main/MINUTES_MARKDOWN.md

---

### Large files

The following files are too large and have therefore been uploaded separately to MEGA Cloud Storage: 
>https://mega.nz/folder/M5cHHAYa#W0VxI6dDM1b6fpf4K9Ma1w
* 大維修相關資訊 2. 工程解說會簡報(宏業及鴻毅).pdf (Maintenance Project Presention by Prestige & Will Power)
* 大維修相關資訊 8. 特別業主大會解說會簡報(14-3-2025).pdf (EGM Presentation / 2025-03-14)
* 宏福通訊 第12屆管理委員會-第4期.pdf (Wang Fuk Newsletter 12th MC - Vol 4)
* 宏福通訊 第12屆管理委員會-第5期.pdf (Wang Fuk Newsletter 12th MC - Vol 5)
* 宏福通訊 第12屆管理委員會-第9期.pdf (Wang Fuk Newsletter 12th MC - Vol 9)

---

### Data Integrity & Discrepancy Log

**1. Mismatched Record (10th Term):**
The [link](http://www.wangfuk.org/html/meeting/05/第9次全體委員會議記錄.pdf) for the *10th MC Minutes No.9 (December 18, 2018)* (第十屆第九次全體委員會議記錄) is incorrectly mapped. It redirects to the *11th MC Minutes No.9 (November 17, 2021)* (第十一屆第九次全體委員會議記錄) instead. Consequently, the original 2018 document is missing.

**2. Missing Agendas (9th Term):**
While the *Meeting Minutes* for the [9th Term](http://www.wangfuk.org/html/meeting/04.htm) are complete, multiple *Meeting Agendas* are missing from the source website.

**3. Incorrect Link (2018 EGM):**
The [link](http://www.wangfuk.org/html/meeting/05/2018.09.07-特別業主大會議程.pdf) for the *Agenda of the Extraordinary General Meeting (September 7, 2018)* (2018年9月7日特別業主大會議程) incorrectly points to the *Minutes* of the same day. As a result, the Agenda document is missing.

**4. Broken Document Link:**
The [link](http://www.wangfuk.org/html/comm/02/第33期%202023.12(印刷).pdf) for Wang Fuk Newsletter 11th MC - Vol.33 (宏福通訊 第11屆管理委員會-第33期) is inaccessible and displayed the error: `HTTP Error 404.0 - Not Found`.

**5. Broken External Links (MBIS/MWIS):**
Items 2 and 3 under the [*Mandatory Building Inspection & Window Inspection Scheme*](http://www.wangfuk.org/html/home/inspection.asp) (強制驗樓驗窗計劃 2. 及 3.) point to the following dead URLs:
*   `https://www.bd.gov.hk/chineseT/services/index_MBIS_MWIS.html`
*   `https://www.bd.gov.hk/chineseT/documents/guideline/GGMBISMWIS.pdf`

**6. Non-Document Redirection:**
Item 10 under the same scheme (強制驗樓驗窗計劃 10.) is not a hosted document but a direct link to the external Smart Tender platform:
*   `https://smarttender.brplatform.org.hk/zh-HK/index.htm`

---

### Batch download

To batch download the files from this repository, you may enter its URL into the following website: 

https://download-directory.github.io/

---

### Service Outage Report: December 3, 2025

Starting around the evening of December 3, 2025 (Hong Kong Time), the website’s homepage suddenly became inaccessible and displayed the error: `HTTP Error 404.0 - Not Found`. It had been functioning normally before that.

![](https://github.com/sparktsang/wangfuk/blob/main/Error.jpg)

**Incident Analysis: Server-Side Failure vs. Protocol Error**

It has been suggested that this downtime was caused by inadvertently using the HTTPS protocol. However, the forensic evidence proves otherwise:

1.  **The Error Page Distinction:** The screenshot above shows a **Native IIS 404.0 Error** (white background). This is a low-level server error indicating that the IIS web server itself was unable to map requests to the application directory.
2.  **HTTPS Behavior:** Accessing the site via HTTPS (which is currently misconfigured) results in a [**Plesk Custom Error** page](https://github.com/sparktsang/wangfuk/blob/main/HTTPS_error.png).

The presence of the raw IIS error confirms that this was a **server-side infrastructure failure** (system maintenance or configuration detachment) and not a client-side protocol mismatch. See also the [detailed analysis of this error](https://github.com/sparktsang/wangfuk/blob/main/error_analysis.md). 

By around 11:50 p.m. on the same day, the homepage returned to normal functionality via HTTP.

---

### Project description

This is part of a [project](https://sparktsang.github.io/life/2025/12/04/status.html) which examines the [tragic fire](https://en.wikipedia.org/wiki/Wang_Fuk_Court_fire) at Wang Fuk Court on 26 November 2025 during renovation works, which resulted in 161 deaths.

---

### Special thanks

**Special thanks** to **Eric** for selflessly coming to the rescue; with his professional data analytics skills, he organized a large volume of files, enabling this backup project to be completed.
