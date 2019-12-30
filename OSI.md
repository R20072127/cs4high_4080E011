# Physical Layer 實體層 1 Layer
```
由於網路媒體只能**傳送 0 與 1**這種位元串，因此實體層必須定義所使用的媒體設備之電壓與訊號等，  
同時還必須瞭解資料訊框轉成位元串的編碼方式，最後連接實體媒體並傳送/接收位元串。
```
# Data Link Layer 資料連結層 2 Layer
```
這一層是比較特殊的一個階層，因為底下是實體的定義，而上層則是軟體封裝的定義。  
因此第二層又分兩個子層在進行資料的轉換動作。  
  
在偏硬體媒體部分，主要負責的是 **MAC (Media Access Control)** ，我們稱這個資料包裹為 MAC 訊框 (frame)，  
MAC 是網路媒體所能處理的主要資料包裹，這也是最終被實體層編碼成位元串的資料。MAC 必須要經由通訊協定來取得媒體的使用權，  
目前最常使用的則是 IEEE 802.3 的乙太網路協定。
  
至於偏向軟體的部分則是由 **LLC(logical link control)** 所控制，主要在多工處理來自上層的封包資料 (packet) 並轉成 MAC 的格式，
負責的工作包括訊息交換、流量控制、失誤問題的處理等等。
```
# Network Layer網路層 3 Layer
```
我們提及的 IP (Internet Protocol) 就是在這一層定義的。  
同時也定義出電腦之間的連線建立、終止與維持等，資料封包的**傳輸路徑選擇**等等，因此這個層級當中最重要的除了 IP 之外，  
就是封包能否到達目的地的**路由(route)** 概念。 
協定:  
  IP（V4 V6）、ICMP（V4、V6）、IPsec  
# Transpoet Layer 傳輸層 4 Layer
這一個分層定義了發送端與接收端的連線技術(如 **TCP**, **UDP** 技術)， 同時包括該技術的封包格式，  
**資料封包的傳送、流程的控制、傳輸過程的偵測檢查與復原重新傳送**等等， 以確保各個資料封包可以正確無誤的到達目的端。  
協定:   
  TCP、UDP
```
# Session Layer 會議層 5 Layer
```
在這個層級當中主要定義了**兩個位址之間的連線通道之連接與掛斷**，亦可建立應用程式之對談、提供其他加強型服務如網路管理、簽到簽退、對談之控制等等。  
如果說傳送層是在判斷資料封包是否可以正確的到達目標， 那麼會談層則是在確定網路服務建立連線的確認。  
```
# Presentation Layer 表現層 6 Layer
```
我們在應用程式上面所製作出來的資料格式不一定符合網路傳輸的標準編碼格式，所以，在這個層級當中，主要的動作就是：  
將來自本地端應用程式的**資料格式轉換** (或者是重新編碼)成為網路的標準格式， 然後再交給底下傳送層等的協定來進行處理。  
所以，在這個層級上面主要定義的是網路服務(或程式)之間的**資料格式的轉換**，包括**資料的加解密**也是在這個分層上面處理。  
```
# Application Layer 應用層 7 Layer
```
應用層本身並不屬於應用程式所有，而是在定義應用程式如何進入此層的溝通介面，以將資料接收或傳送給應用程式，最終展示給使用者。
協定:  
  HTTP、SSH、DNS、SNMP、FTP、TELNET、DHCP
```