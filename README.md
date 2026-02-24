## 🌿 Git Branching Strategy

This repository follows a structured branching strategy to ensure code quality, stability, and smooth CI/CD deployments.

### 🔹 Main Branches

| Branch | Purpose |
|--------|----------|
| `main` | Production-ready code. Always stable and deployable. |
| `develop` | Integration branch for testing features before release. |

---

### 🔹 Supporting Branches

#### 🚀 Feature Branches
- Naming: `feature/<feature-name>`
- Created from: `develop`
- Purpose: Develop new features or enhancements.
- Merged back into: `develop` via Pull Request (PR)

Example:
feature/add-vpc-module
feature/update-eks-config

---

#### 🛠 Hotfix Branches
- Naming: `hotfix/<issue-name>`
- Created from: `main`
- Purpose: Fix critical production issues.
- Merged back into: `main` and `develop`

Example:
hotfix/fix-security-group
hotfix/critical-terraform-bug