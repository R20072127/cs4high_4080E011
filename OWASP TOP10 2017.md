```
https://www.owasp.org/index.php/Category:OWASP_Top_Ten_Project
T10 OWASP Top 10
A1:2017-注入 Injection
    將不受信任的數據作為命令或查詢的一部分發送到解析器時，會產生諸如SQL注入、NoSQL注入、OS
    注入和LDAP注入的注入缺陷。攻擊者的惡意數據可以誘使解析器在[沒有適當授權]的情況下執行非預
    期[命令或訪問]數據。
A2:2017-失效的身份認證 Broken Authentication
    通常，通過[錯誤]使用應用程序的身份認證和會話管理功能，攻擊者能夠[破譯密碼]、密鑰或會話令牌，
    或者利用其它開發[缺陷]來暫時性或永久性[冒充其他用戶]的身份。
A3:2017-敏感數據洩露 Sensitive Data Exposure
    許多Web應用程序和API都無法正確保護敏感數據，例如：財務數據、醫療數據和PII數據。攻擊者可
    以通過[竊取或修改未加密的數據]來實施信用卡詐騙、身份盜竊或其他犯罪行為。未加密的敏感數據
    容易受到破壞，因此，我們需要對敏感數據加密，這些數據包括：傳輸過程中的數據、存儲的數據
    以及瀏覽器的交互數據。
A4:2017-XML外部實體（XXE）XML External Entities 
    許多較早的或配置錯誤的XML處理器評估了XML文件中的外部實體引用。攻擊者可以[利用外部實體]竊
    取使用URI文件處理器的內部文件和共享文件、監聽內部掃描端口、執行遠程代碼和實施拒絕服務攻
    擊。
A5:2017-失效的訪問控制 Broken Access Control
    未對通過身份驗證的用戶實施恰當的[訪問控制]。攻擊者可以利用這些缺陷訪問未經授權的功能或數
    據，例如：訪問其他用戶的帳戶、查看敏感文件、修改其他用戶的數據、更改訪問權限等。
A6:2017-安全配置錯誤 Security Misconfiguration
    安全配置錯誤是最常見的安全問題，這通常是由於不安全的默認配置、不完整的臨時配置、開源雲
    存儲、錯誤的HTTP標頭配置以及包含敏感信息的詳細錯誤信息所造成的。因此，我們不僅需要對所
    有的操作系統、框架、庫和應用程序進行安全配置，而且必須及時修補和升級它們。
A7:2017-跨站腳本（XSS）Cross-Site Scripting
    當應用程序的新網頁中包含不受信任的、未經恰當驗證或轉義的數據時，或者使用可以創建HTML或
    JavaScript的瀏覽器API更新現有的網頁時，就會出現XSS缺陷。XSS讓攻擊者能夠在受害者的瀏覽器
    中[執行腳本]，並劫持用戶會話、破壞網站或將用戶重定向到惡意站點。
A8:2017-不安全的反序列化 Insecure Deserialization
    不安全的反序列化會導致遠程代碼執行。即使[反序列化缺陷]不會導致遠程代碼執行，攻擊者也可以
    利用它們來執行攻擊，包括：重播攻擊、注入攻擊和特權升級攻擊。
A9:2017-使用含有已知漏洞的組件 Using Componentswith Known Vulnerabilities
    組件（例如：庫、框架和其他軟件模塊）擁有和應用程序相同的權限。如果應用程序中含有已知漏
    洞的組件被攻擊者利用，可能會造成嚴重的數據丟失或服務器接管。同時，使用含有已知漏洞的組
    件的應用程序和API可能會破壞應用程序防禦、造成各種攻擊並產生嚴重影響。
A10:2017-不足的日誌記錄和監控 Insufficient Logging & Monitoring
    不足的日誌記錄和監控，以及事件響應缺失或無效的集成，使攻擊者能夠進一步攻擊系統、保持持
    續性或轉向更多系統，以及篡改、提取或銷毀數據。大多數缺陷研究顯示，缺陷被檢測出的時間超
    過200天，且通常通過外部檢測方檢測，而不是通過內部流程或監控檢測。
```
