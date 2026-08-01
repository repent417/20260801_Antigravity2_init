---
name: antigravity-obsidian
description: 在 AntiGravity 連接 Obsidian MCP (MCPVault)。說「連接 Obsidian」「設定 Obsidian」時載入。
---

# 連接 Obsidian（AntiGravity 版）

## 步驟

### 1. 找到 vault
請先確認 Obsidian vault 的實體路徑。常見位置：
- `C:\Users\<你>\OneDrive\文件\Secondbrain`
- `C:\Users\<你>\Documents\<vault 名稱>`
- `G:\我的雲端硬碟\<vault 名稱>`

### 2. 安裝 MCPVault
在命令提示字元或 PowerShell 中執行安裝：
```powershell
npm.cmd install -g @bitbonsai/mcpvault
where.exe mcpvault
```
常見路徑為：
`C:\Users\<你>\AppData\Roaming\npm\mcpvault.cmd`

### 3. 註冊 Obsidian MCP
請依 AntiGravity 實際 MCP 設定方式加入設定檔：
```json
"obsidian": {
  "type": "local",
  "command": [
    "C:\\Users\\<你>\\AppData\\Roaming\\npm\\mcpvault.cmd",
    "C:\\Users\\<你>\\OneDrive\\文件\\Secondbrain"
  ],
  "enabled": true
}
```

完成後重啟 AntiGravity 測試連接。
