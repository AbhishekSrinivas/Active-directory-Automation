# Active Directory Automation

PowerShell scripts for bulk-creating Active Directory users from a CSV file.

## Layout

| Path | Purpose |
|---|---|
| `scripts/New-AD-Users-from-CSV.ps1` | Creates users from a CSV with only the required attributes |
| `scripts/New-AD-Users-from-CSV-v2.ps1` | Variant of the above |
| `samples/users-sample.csv` | Sample input with placeholder values |

## Usage

1. Replace `contoso.com` in the script with your UPN suffix.
2. Fill the CSV. The `password` column is a placeholder (`<PASSWORD>`); use strong, unique initial passwords and force change at next logon.
3. Run from a machine with the ActiveDirectory module:

```powershell
Import-Module ActiveDirectory
.\scripts\New-AD-Users-from-CSV.ps1
```

## Notes

- All sample data is fictional. Never commit real user data or passwords.
- Test in a lab domain before production.
