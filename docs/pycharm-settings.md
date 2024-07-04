# 在 PyCharm IDE 中設定並運行程式的步驟說明

以下是如何在 PyCharm 中設定並運行此配置的詳細步驟：

## 1. 打開 PyCharm 並載入專案

1. 打開 PyCharm。
2. 使用 `File` -> `Open`，選擇並載入你的專案目錄。

## 2. 配置運行設定

1. **打開 Run/Debug Configurations 窗口**：
   - 點擊 PyCharm 頂部工具欄的 `Run` 菜單，選擇 `Edit Configurations`。

2. **新增 Python 運行配置**：
   - 在左側欄中，點擊 `+` 按鈕，選擇 `Python`。

3. **填寫配置詳細信息**：
   - **Name**: `otomati-app`
   - **Module name**: `otomati-app`
   - **Environment Variables**:
     - 點擊右側的 `...` 按鈕，新增環境變量 `PYTHONUNBUFFERED`，值設為 `1`。
   - **Python interpreter**:
     - 確保選擇了 `Python 3.12 (otomati-app)`，如果沒有，點擊齒輪圖標，選擇或新增合適的 Python 解釋器。
   - **Working directory**:
     - 設定為 `$PROJECT_DIR$/otomati_app`。點擊右側的資料夾圖標，瀏覽並選擇專案目錄中的 `otomati_app` 資料夾。
   - **Script path**:
     - 設定為 `$PROJECT_DIR$/.venv/bin/streamlit`。瀏覽並選擇專案中的 `streamlit` 可執行文件。
   - **Parameters**:
     - 設定為 `run Home.py`。這表示執行 Streamlit，並運行 `Home.py` 文件。
   - **Add content roots to PYTHONPATH**:
     - 勾選此選項。
   - **Add source roots to PYTHONPATH**:
     - 勾選此選項。
   - **Run with Python Console**:
     - 不需要勾選此選項。
   - **Emulate terminal in output console**:
     - 不需要勾選此選項。

4. **Coverage 設定（可選）**：
   - **Extension**:
     - 確保添加了 `PythonCoverageRunConfigurationExtension`，並設定 `runner` 為 `coverage.py`。這步驟是為了啟用程式覆蓋率分析。

5. **其他選項**：
   - **Redirect input**:
     - 不需要勾選此選項。
   - **Input file**:
     - 留空。

6. **保存配置**：
   - 點擊 `Apply`，然後點擊 `OK` 保存配置。

## 3. 運行配置

1. **選擇配置**：
   - 在 PyCharm 頂部工具欄的運行配置選單中，選擇剛剛創建的 `otomati-app` 配置。

2. **運行程式**：
   - 點擊運行按鈕（綠色箭頭）或按下 `⌃ + R` 開始運行配置的程式。

3. **Debugging**:
   - 如果需要調試程式，可以使用 `Debug` 模式運行配置或按下 `⌃ + D`。

## 4. 驗證運行結果

1. 確保 PyCharm 的 `Run` 窗口中沒有顯示錯誤。
2. 你的 Streamlit 應用應該在瀏覽器中自動打開，顯示 `Home.py` 文件的內容。