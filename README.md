# Active Directory Automation

PowerShell scripts for bulk-creating Active Directory users from a CSV file.

## Contents

| File | Purpose |
|---|---|
| `AD Users Creation with minimum required field.ps1` | Creates users from a CSV with only the required attributes |
| `AD Users Creation with minimum required field 1.ps1` | Variant of the above |
| `Test1.csv` | Sample input with placeholder values |

## Usage

1. Replace `contoso.com` in the script with your UPN suffix.
2. Fill the CSV. The `password` column is a placeholder (`<PASSWORD>`); use strong, unique initial passwords and force change at next logon.
3. Run from a machine with the ActiveDirectory module:

```powershell
Import-Module ActiveDirectory
.\"AD Users Creation with minimum required field.ps1"
```

## Notes

- All sample data is fictional. Never commit real user data or passwords.
- Test in a lab domain before production.
