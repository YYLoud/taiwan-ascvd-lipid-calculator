# ASCVD 風險評估與血脂治療計算器

單一檔案的網頁計算器（`index.html`，無需安裝、可離線使用），整合台灣三份文件的判定準則：

| 分頁 | 內容 | 依據 |
|---|---|---|
| ① 10 年 CAD 風險與 CAC | TwCCCC 點數計分（0–24 分）→ 10 年冠心病風險與分層；CAC 風險修正演算法 | TSOC 2024 ASCVD 初級預防指引 Part I，Table 4／Figure 5 |
| ② 血脂治療目標與路徑 | 五級風險分層 → LDL-C／non-HDL-C 目標與臨床路徑步驟 | 2025 台灣血脂臨床路徑共識，Table 1／Figure 1／Figure 2 |
| ③ 健保給付與用藥建議 | 表一（新制）門檻與目標、表二（舊制）對照、健保碼查詢、statin 強度建議 | 健保署藥品給付規定 2.6.1／2.6.2／2.6.3，115/9/1 生效 |
| ④ 病歷輸出 | 依前三頁自動產生病歷文字（中文完整／中文精簡／English SOAP），可複製、下載 .txt 或列印 | — |

## 功能

- **跨分頁自動同步**：年齡、性別、身高體重、血壓、LDL-C、HDL-C、TC、CAC、吸菸、家族史等在任一分頁修改都會同步。
- **依檢驗值自動勾選危險因子**：填入舒張壓、腰圍、空腹血糖、TG、HbA1c、eGFR／UACR 後，高血壓、糖尿病、CKD、代謝症候群各子項會自動判定；手動點選即改為人工控制，並可一鍵回復自動判定。
- **高血壓判定**：採 2022 台灣高血壓指引之標準化 722 居家血壓 ≥ 130/80 mmHg，或已使用降壓藥物。
- **健保碼查詢**：內建 2.6.1 不適用表一之 116 項、2.6.2 之 4 項、2.6.3 之 10 項共 130 個健保代碼，判定該品項走表一或表二、等待期為 6~8 週或 3 個月。

## 使用方式

下載 `index.html` 後用瀏覽器開啟即可；所有計算都在瀏覽器本機執行，不會傳送任何資料。

## 資料來源

1. Chao TH, et al. 2024 Guidelines of the Taiwan Society of Cardiology on the Primary Prevention of Atherosclerotic Cardiovascular Disease — Part I. *Acta Cardiol Sin* 2024;40:479–543.
2. Chao TH, et al. 同系列 Part II. *Acta Cardiol Sin* 2024;40:669–715.（§5.6.1、Figure 2：高血壓診斷門檻）
3. Li YH, Shih CL, et al. 2025 Consensus on the Clinical Pathway of Blood Cholesterol Management in Taiwan. *Acta Cardiol Sin* 2025;41:161–165.
4. 衛生福利部中央健康保險署「藥品給付規定」第 2 節 2.6.1／2.6.2／2.6.3，115 年 9 月 1 日生效之修訂。

## 免責聲明

本工具僅供醫療專業人員參考與衛教用途，**不能取代臨床判斷**。用藥種類、劑量與適應症請依藥品仿單辦理；健保給付判定僅依健保碼比對，實際給付以健保署最新公告為準。
