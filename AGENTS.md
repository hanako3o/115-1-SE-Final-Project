# 軟體工程期末專題協作規則

- 三個模組共用一個 CodeIgniter 4 專案、一個 MySQL 資料庫，以及一套 CI4 Shield 登入。
- 網頁使用 CI4 View、HTML、CSS 和原生 JavaScript。開始修改前先讀 README.md 和現有程式。
- 模組一管院空間查詢使用 /spaces，模組二預約借用使用 /reservations，模組三志願排課使用 /scheduling。
- 模組一維護 rooms 表和 RoomModel。借用與排課使用 room_id 參照 rooms.id，帳號關聯使用 Shield 的使用者 ID。
- 角色統一為 member、teacher、admin。訪客可以查詢教室，其他功能依登入、帳號審核和角色檢查權限。
- 各模組透過自己的 migration 建表。需要變更共用帳號或教室資料時，先和主整合者確認。
- 各組員從 main 開功能分支，用自己的 GitHub 帳號推送，透過 Pull Request 合併。
- 資料庫密碼和本機 .env 留在各自電腦。
