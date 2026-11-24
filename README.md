# 波動函數實驗室（Wave Function Lab）

互動式繁體中文 HTML 教學網頁：輸入任一個波動參數，其他相關參數自動連動，並以 Canvas 即時顯示行進波和駐波動畫。

## 功能

- 可調 `v`（波速）、`λ`（波長）、`f`（頻率）、`T`（週期）、`ω`（角頻率）、`k`（波數）。
- 自動滿足 `v = fλ`、`T = 1/f`、`ω = 2πf`、`k = 2π/λ`。
- 改變 `f`、`T`、`ω` 時，保持 `λ` 不變；改變 `λ`、`k` 時，保持 `f` 不變；改變 `v` 時，保持 `f` 不變並調整 `λ`。
- 顯示向右行進波 `y₁(x,t) = A sin(kx − ωt)`。
- 勾選後另顯示向左行進波 `y₂(x,t) = A sin(kx + ωt)` 與駐波 `y₁ + y₂ = 2A sin(kx) cos(ωt)`。
- 可調振幅 A、觀察範圍、時間軸和播放速度；可暫停、重新開始或切換範例。
- 點擊圖上任意位置可查看該點的即時位移。
- 無框架、無套件、無後端、無網路連線依賴。

## 使用

直接雙擊 `index.html`，用 Chrome、Edge、Safari 或 Firefox 開啟。

## GitHub Pages 部署

1. 到 GitHub 新增一個儲存庫（例如 `wave-function-lab`），建議設為 **Public**。
2. 把 `index.html` 上傳至該儲存庫的**根目錄**（README.md 可一起上傳）。
3. 開啟儲存庫的 **Settings → Pages**。
4. **Build and deployment → Source** 選擇 **Deploy from a branch**。
5. **Branch** 選 `main`、資料夾選 `/(root)`，按 **Save**。
6. 網站網址一般為：`https://你的GitHub帳號.github.io/wave-function-lab/`。

如儲存庫名稱不同，網址中的路徑也須相應修改。GitHub Pages 的部署狀態可在儲存庫 Actions 或 Pages 畫面查看。

## 模型限制

這是一維線性行進波與疊加的**教學動畫**，並非波浪水槽、法拉第波或非牛頓流體的數值求解器。實際液面波可能存在色散、阻尼、非線性和邊界效應。
