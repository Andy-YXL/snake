# 貪食蛇 Snake

用 HTML + JavaScript + Canvas 實作的貪吃蛇。

## 線上試玩
https://andy-yxl.github.io/snake/

## 操作方式
方向鍵或 WASD 移動，R 重新開始。

## 使用技術
HTML5 Canvas 2D、JavaScript、CSS Flexbox

## 實作內容
- 蛇身以陣列儲存，移動由增加並去掉尾巴的方式實現，吃到食物時跳過去尾過程，達到變長的效果。
- 用查表的方式對應按鍵與方向的關係，這樣新增按鍵不用改控制邏輯。
- 碰撞判定在更新蛇身之前執行，避免新頭被納入自身碰撞檢查
- 與目前行進方向相反的轉向指令不接收，以達到驗證輸入的效果

## 已知問題
- 食物有機會生成在蛇身上，預計加入判斷方式進行食物重抽。
- 同一個更新週期內連按兩次方向鍵可繞過反向檢查，預計改為記憶前一次移動方向來解決。

## 遊戲畫面
<img width="1034" height="898" alt="snake" src="https://github.com/user-attachments/assets/bd3dc92a-beb0-43fd-91ca-a15d6428257a" />
