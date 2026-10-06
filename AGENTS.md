# AGENTS.md

## 語言與套件管理
- 專案語言為 Python，一律使用 conda 管理套件，不要使用 pip / venv / uv / poetry。
- 唯一的 conda 環境為 `iem_python`。執行任何 Python 指令前，先啟用該環境。

```powershell
conda activate iem_python
python --version
conda list
```

## 現況（2026-10-06）
- 剛初始化的空專案，只有 `README.md` + Python `.gitignore`，尚無原始碼、相依清單（`environment.yml` / `requirements*.txt`）、測試、lint、CI。
- 新增相依時只用 `conda install`（或必要時 `conda-forge` channel），並在此檔案補上匯出環境的實際指令。

## 尚未建立的驗證指令
- 目前沒有 build / test / lint / typecheck 指令。有測試或檢查工具後，請在此補上單一測試與完整驗證的確切指令。
