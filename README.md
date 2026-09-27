# 重症插管導航

依 **DAS/ICS/FICM/RCoA 2018 重症插管指引**與 **SCCM 2023 快速誘導插管（RSI）指引**製作的互動工具：插管前評估、檢核表、RSI 藥物劑量計算、困難氣道 Plan A–D 流程與插管後照護。

線上版：https://yht5582-source.github.io/ICU-intubation/

> ⚠️ **僅供插管流程輔助與教學，不取代臨床判斷與團隊領導。** 藥物劑量請依院內規範並經藥師確認；困難氣道時儘早求援。

## 功能

| 區塊 | 內容 |
|---|---|
| 1. 插管前評估 | 理想體重、瘦體重、BMI、休克指數；MACOCHA 分數（≥3 預期困難插管）；休克、嚴重酸中毒、右心衰竭等生理性困難氣道提示；P/F <150 提示以 NIV 前給氧 |
| 2. 檢核表 | 病人、器材、藥物、團隊四組共 25 項 |
| 3. RSI 藥物 | Ketamine、etomidate、propofol、midazolam；rocuronium、succinylcholine（勾選禁忌症會自動停用）；休克時自動改用減量；BMI ≥30 時誘導劑用瘦體重、rocuronium 用理想體重、succinylcholine 用實際體重；fentanyl、推注用升壓劑、sugammadex |
| 4. Plan A–D | A：插管最多 3 次＋資深者 1 次；B：第二代 SGA 最多 3 次；C：面罩通氣；D：CICO 時 scalpel–bougie–tube 頸前氣道；每步驟記錄時間 |
| 5. 插管後 | ETCO₂、X 光、呼吸器、鎮痛鎮靜、低血壓、氣囊壓力、紀錄；SCCM 2023 建議摘要 |

## 使用方式

直接用瀏覽器開啟 `index.html` 即可，不需安裝或建置。

## 在地化設定

| 項目 | 位置 |
|---|---|
| MACOCHA 項目 | `<script>` 內 `MAC` |
| Succinylcholine 禁忌 | `SUX_CI` |
| 藥物與劑量 | `drugs()` |
| 檢核表 | `render()` 內 `CL` |
| Plan A–D 內容 | `planHTML()` |

## 資料與隱私

- 所有資料只存在該瀏覽器的 `localStorage`，不會上傳。
- 只記錄床號，請勿輸入姓名或病歷號。

## 依據

1. Higgs A, McGrath BA, Goddard C, et al. Guidelines for the management of tracheal intubation in critically ill adults. *Br J Anaesth* 2018;120:323–352.
2. Acquisto NM, Mosier JM, Bittner EA, et al. Society of Critical Care Medicine clinical practice guidelines for rapid sequence intubation in the critically ill adult patient. *Crit Care Med* 2023;51:1411–1430. [doi:10.1097/CCM.0000000000006000](https://doi.org/10.1097/CCM.0000000000006000)
3. De Jong A, et al. Early identification of patients at risk for difficult intubation in the ICU (MACOCHA). *Am J Respir Crit Care Med* 2013;187:832–839.
4. Casey JD, et al. PreVent. *N Engl J Med* 2019;380:811–821；Prekker ME, et al. DEVICE. *N Engl J Med* 2023;389:418–429；Gibbs KW, et al. PREOXI. *N Engl J Med* 2024;390:2165–2177.
5. Janmahasatian S, et al. Quantification of lean bodyweight. *Clin Pharmacokinet* 2005;44:1051–1065.

## 授權

請依使用單位規定自行選擇授權方式（例如 MIT）。
