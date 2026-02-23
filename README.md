# Microsoft-Sentinel

Sentinel analytics rules and content managed as code. Pushes to `main` trigger automated deployment via GitHub Actions.

## CI/CD Configuration

- **App Registration:** `Sentinel-GitHub-CICD` (09cd9c56-51d4-4f48-aef0-cbcd1f506517)
- **Authentication:** OIDC federated credential (no secrets stored)
- **RBAC Roles:** Microsoft Sentinel Contributor + Contributor on `PWS-RG-AVD-01`
- **Target:** `microsoft-sentinel-law` workspace in `PWS-RG-AVD-01`

## Structure

```
AnalyticsRules/     # Sentinel analytics rules (ARM templates)
.github/workflows/  # CI/CD deployment pipeline
```