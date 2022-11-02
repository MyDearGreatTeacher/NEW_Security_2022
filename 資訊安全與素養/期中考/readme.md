## 期中考報告
```
1.資訊安全目標:CIA
   破換CIA的各種資安情境
   保護CIA的各種技術
2.雜湊函數與實戰
3.密碼學的基本認知
4.WINDOWS 安全實戰技術
  netstat 
  taskkill
5.Linux-CTF解題
```

## 2.雜湊函數與實戰
- 雜湊函數 Hash function
  - [英文版wiki說明](https://en.wikipedia.org/wiki/Hash_function)
  - [中文版wiki說明:雜湊函式](https://zh.wikipedia.org/wiki/%E6%95%A3%E5%88%97%E5%87%BD%E6%95%B8)
- 雜湊函數實戰:linux指令
  - md5sum  ==> MD5 128-bit checksums
    - [How to Use the md5sum Command in Linux](https://phoenixnap.com/kb/md5sum-linux) 
    - [Linux md5sum command](https://www.computerhope.com/unix/md5sum.htm)
    - 範例用法:  md5sum date.txt
  - shasum 
    - [SHASUM Command on Linux](https://linuxhint.com/shasum-linux/)  
      - SHA-256 — generates a digest of 32 bytes
        - 範例用法: shasum demo.txt
        - 範例用法: sha1sum demo.txt 
        - 範例用法: shasum -a 256 demo.txt
      - SHA-384 — generates a digest of 48 bytes
        - [Linux sha384sum command](https://www.computerhope.com/unix/sha384sum.htm) 
        - 範例用法: sha384sum example.iso
      - SHA-512 — generates a digest of 64 bytes
        - [Linux sha512sum command](https://www.computerhope.com/unix/sha512sum.htm)
        - 範例用法: sha512sum example.iso 
- 雜湊函數實戰:Windows指令:

```
C:\Users\User>certutil /?

動詞:
  -dump             -- 傾印設定資訊或檔案
  -dumpPFX          -- 傾印 PFX 結構
  -asn              -- 剖析 ASN.1 檔案

  -decodehex        -- 將十六進位編碼的檔案解碼
  -decode           -- 將 Base64 編碼的檔案解碼
  -encode           -- 將檔案以 Base64 編碼

  -deny             -- 拒絕擱置要求
  -resubmit         -- 重新提交擱置要求
  -setattributes    -- 設定擱置要求的屬性
  -setextension     -- 設定擱置要求的延伸
  -revoke           -- 撤銷憑證
  -isvalid          -- 顯示目前的憑證配置

  -getconfig        -- 取得預設的設定字串
  -ping             -- 抓取 Active Directory 憑證服務要求介面
  -pingadmin        -- 抓取 Active Directory 憑證服務管理介面
  -CAInfo           -- 顯示 CA 資訊
  -ca.cert          -- 抓取 CA 憑證
  -ca.chain         -- 抓取 CA 的憑證鏈結
  -GetCRL           -- 取得 CRL
  -CRL              -- 發佈新的 CRL [或僅限 delta CRL]
  -shutdown         -- 關閉 Active Directory 憑證服務

  -installCert      -- 安裝憑證授權單位憑證
  -renewCert        -- 更新憑證授權單位憑證

  -schema           -- 傾印憑證架構
  -view             -- 傾印憑證檢視
  -db               -- 傾印原始資料庫
  -deleterow        -- 刪除伺服器資料庫資料行

  -backup           -- 備份 Active Directory 憑證服務
  -backupDB         -- 備份 Active Directory 憑證服務資料庫
  -backupKey        -- 備份 Active Directory 憑證服務的憑證及私密金鑰
  -restore          -- 還原 Active Directory 憑證服務
  -restoreDB        -- 還原 Active Directory 憑證服務資料庫
  -restoreKey       -- 還原 Active Directory 憑證服務的憑證及私密金鑰
  -importPFX        -- 匯入憑證及私密金鑰
  -dynamicfilelist  -- 顯示動態檔案清單
  -databaselocations -- 顯示資料庫位置
  -hashfile         -- 透過檔案產生並顯示密碼編譯雜湊

  -store            -- 傾印憑證存放區
  -enumstore        -- 列舉憑證存放區
  -addstore         -- 將憑證加入存放區
  -delstore         -- 從存放區刪除憑證
  -verifystore      -- 確認存放區中的憑證
  -repairstore      -- 修復金鑰關聯或更新憑證內容或金鑰安全性描述元
  -viewstore        -- 傾印憑證存放區
  -viewdelstore     -- 從存放區刪除憑證
  -UI               -- 叫用 CryptUI
  -attest           -- 驗證金鑰證明要求

  -dsPublish        -- 將憑證或 CRL 發佈到 Active Directory

  -ADTemplate       -- 顯示 AD 範本
  -Template         -- 顯示註冊原則範本
  -TemplateCAs      -- 顯示範本 CA
  -CATemplates      -- 顯示 CA 範本
  -SetCASites       -- 管理 CA 的站台名稱
  -enrollmentServerURL -- 顯示、新增或刪除 CA 關聯的註冊伺服器 URL
  -ADCA             -- 顯示 AD CA
  -CA               -- 顯示註冊原則 CA
  -Policy           -- 顯示註冊原則
  -PolicyCache      -- 顯示或刪除註冊原則快取項目
  -CredStore        -- 顯示、新增或刪除認證存放區項目
  -InstallDefaultTemplates -- 安裝預設憑證範本
  -URLCache         -- 顯示或刪除 URL 快取項目
  -pulse            -- 脈衝式自動註冊事件或 NGC 工作
  -MachineInfo      -- 顯示 Active Directory 機器物件資訊
  -DCInfo           -- 顯示網域控制站資訊
  -EntInfo          -- 顯示公司資訊
  -TCAInfo          -- 顯示 CA 資訊
  -SCInfo           -- 顯示智慧卡資訊

  -SCRoots          -- 管理智慧卡根憑證

  -DeleteHelloContainer -- 刪除 Hello 登入容器。
     ** 使用者使用此選項後，必須登出才能使它完成。 **
  -verifykeys       -- 確認公開/私密金鑰組
  -verify           -- 確認憑證、CRL 或鏈結
  -verifyCTL        -- 驗證 AuthRoot 或不允許的憑證 CTL
  -syncWithWU       -- 與 Windows Update 同步
  -generateSSTFromWU -- 從 Windows Update 產生 SST
  -generatePinRulesCTL -- 產生 PIN 規則 CTL
  -downloadOcsp     -- 下載 OCSP 回應並寫入到目錄
  -generateHpkpHeader -- 使用所指定檔案或目錄中的憑證來產生 HPKP 標頭
  -flushCache       -- 在選取的處理序中排清指定的快取，例如 lsass.exe
  -addEccCurve      -- 新增 ECC 曲線
  -deleteEccCurve   -- 刪除 ECC 曲線
  -displayEccCurve  -- 顯示 ECC 曲線
  -sign             -- 重新簽署 CRL 或憑證

  -vroot            -- 建立/刪除網路虛擬根目錄及檔案共用
  -vocsproot        -- 建立/刪除 OCSP Web Proxy 的 Web 虛擬根目錄
  -addEnrollmentServer -- 新增註冊伺服器應用程式
  -deleteEnrollmentServer -- 刪除註冊伺服器應用程式
  -addPolicyServer  -- 新增原則伺服器應用程式
  -deletePolicyServer -- 刪除原則伺服器應用程式
  -oid              -- 顯示 ObjectId 或設定顯示名稱
  -error            -- 顯示錯誤碼訊息文字
  -getreg           -- 顯示登錄值
  -setreg           -- 設定登錄值
  -delreg           -- 刪除登錄值

  -ImportKMS        -- 將使用者金鑰及憑證匯入伺服器資料庫以保存金鑰
  -ImportCert       -- 將憑證檔案匯入資料庫
  -GetKey           -- 抓取封存的私密金鑰修復 Blob、產生修復指令碼，
      或復原封存的金鑰
  -RecoverKey       -- 修復備份私密金鑰
  -MergePFX         -- 合併 PFX 檔案
  -ConvertEPF       -- 將 PFX 檔案轉換為 EPF 檔案

  -add-chain        -- (-AddChain) 新增憑證鏈結
  -add-pre-chain    -- (-AddPrechain) 新增簽署前憑證鏈結
  -get-sth          -- (-GetSTH) 取得已簽署的樹狀首節點
  -get-sth-consistency -- (-GetSTHConsistency) 取得已簽署的樹狀首節點變更
  -get-proof-by-hash -- (-GetProofByHash) 透過雜湊取得證明
  -get-entries      -- (-GetEntries) 取得項目
  -get-roots        -- (-GetRoots) 取得根目錄
  -get-entry-and-proof -- (-GetEntryAndProof) 取得項目和證明
  -VerifyCT         -- 驗證憑證 SCT
  -?                -- 顯示這個使用訊息


CertUtil -?              -- 顯示動詞清單 (命令清單)
CertUtil -dump -?        -- 顯示 "dump" 命令的說明文字
CertUtil -v -?           -- 顯示全部命令的所有說明文字

CertUtil: -? 命令成功完成。
```

```
C:\Users\User>certutil -hashfile /?
使用量:
  CertUtil [選項] -hashfile InFile [HashAlgorithm]
  透過檔案產生並顯示密碼編譯雜湊

選項:
  -Unicode          -- 以 Unicode 寫入重新導向的輸出
  -gmt              -- 用 GMT 格式顯示時間
  -seconds          -- 顯示時間 (秒，毫秒)
  -v                -- 詳細資訊操作
  -privatekey       -- 顯示密碼與私密金鑰資料
  -pin PIN                  -- 智慧卡 PIN
  -sid WELL_KNOWN_SID_TYPE  -- 數值 SID
            22 -- 本機系統
            23 -- 本機服務
            24 -- 網路服務

雜湊演算法: MD2 MD4 MD5 SHA1 SHA256 SHA384 SHA512

CertUtil -?              -- 顯示動詞清單 (命令清單)
CertUtil -hashfile -?    -- 顯示 "hashfile" 命令的說明文字
CertUtil -v -?           -- 顯示全部命令的所有說明文字
```
