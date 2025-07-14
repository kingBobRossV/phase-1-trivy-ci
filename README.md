# Phase 1: CI/CD Security Scan with Trivy

## 🔍 Objective
Create a GitHub Actions pipeline that automatically scans Docker images for vulnerabilities using Trivy, and blocks builds with critical issues.

## 🛠️ Tools Used
- GitHub Actions
- Trivy
- Docker
- Python (for sample app)

## Steps



## ✅ Outcome
- Created a pipeline triggered on PRs or commits
- Learned how to fail a build on CVEs
- Identified CVEs in `requests==2.19.1`

## 🧠 Lessons Learned
- Trivy detects OS + app-level vulnerabilities
- Using `--exit-code 1` stops insecure builds
