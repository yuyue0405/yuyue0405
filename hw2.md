```mermaid
graph TD
    A[1. 研擬計畫] --> B[2. 任務分配]
    A --> C[3. 取得硬體]
    B --> D[4. 程式開發]
    C --> E[5. 安裝硬體]
    D --> F[6. 程式測試]
    E --> G[7. 撰寫使用手冊]
    E --> H[8. 轉換檔案]
    F --> I[9. 系統測試]
    G --> J[10. 使用者訓練]
    H --> J
    I --> K[11. 使用者測試]
    
    %% 標註關鍵路徑
    style A fill:#f96
    style B fill:#f96
    style D fill:#f96
    style F fill:#f96
    style I fill:#f96
    style K fill:#f96



```markdown
```mermaid
gantt
    title 專案甘特圖
    dateFormat  X
    axisFormat  %j
    section 計畫階段
    1. 研擬計畫         :done, a1, 0, 1d
    2. 任務分配         :a2, after a1, 4d
    3. 取得硬體         :a3, after a1, 17d
    
    section 開發階段
    4. 程式開發         :a4, after a2, 70d
    5. 安裝硬體         :a5, after a3, 10d
    6. 程式測試         :a6, after a4, 30d
    
    section 文件與訓練
    7. 撰寫使用手冊     :a7, after a5, 25d
    8. 轉換檔案         :a8, after a5, 20d
    9. 系統測試         :a9, after a6, 25d
    10. 使用者訓練      :a10, after a7, 20d
    11. 使用者測試      :a11, after a9, 25d
