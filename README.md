# Phase 1: CI/CD Security Scan with Trivy

## 🔍 Objective
Create a GitHub Actions pipeline that automatically scans Docker images for vulnerabilities using Trivy, and blocks builds with critical issues.

## 🛠️ Tools Used
- GitHub Actions
- Trivy
- Docker
- Python (for sample app)

## Steps

*Ref 1: Cloned code to local machine from Github*



*Ref 2: Built a Minimal Python Web App*
  - Built a Minimal Python Web App
    - Used Flask to create a lightweight HTTP server
    - Added a route (/) that makes an external request using the requests library
    - Simple structure makes it easy to containerize and scan


   
*Ref 3: Created requirements.txt file*
  - The requirements.txt file defines the app's dependencies so they can be installed consistently across environments. It includes a known vulnerable version of requests to test Trivy's ability to detect outdated packages.



*Ref 4: 





## ✅ Outcome
- Created a pipeline triggered on PRs or commits
- Learned how to fail a build on CVEs
- Identified CVEs in `requests==2.19.1`

## 🧠 Lessons Learned
- Trivy detects OS + app-level vulnerabilities
- Using `--exit-code 1` stops insecure builds
