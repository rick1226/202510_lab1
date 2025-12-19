# 202510_lab1

## 程式碼品質分析

本專案使用 SonarCloud 進行程式碼品質分析。

### 品質設定檔變更通知

The quality profile assigned to this project has changed. You can explore the change in the Activity page.

### SonarCloud 設定

- 專案金鑰：`rick1226_202510_lab1`
- 組織：`rick1226`
- 掃描來源：`app/` 目錄
- 排除檔案：node_modules、dist 目錄、壓縮的 JS 檔案

### CI/CD Pipeline

專案的 CI/CD Pipeline 包含以下安全掃描：
- SAST (原始碼安全掃描) - Semgrep
- SCA (依賴漏洞檢測) - OWASP Dependency-Check
- 容器映像掃描 - Trivy
- IaC 安全檢查 - Checkov
- Secret 掃描 - Gitleaks
- 程式碼品質分析 - SonarCloud