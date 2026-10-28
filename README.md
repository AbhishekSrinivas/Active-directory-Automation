# Active Directory Automation

PowerShell for creating Active Directory users in bulk from a CSV.

- `scripts/New-AD-Users-from-CSV.ps1` creates users with only the required attributes
- `scripts/New-AD-Users-from-CSV-v2.ps1` is a variant
- `samples/users-sample.csv` is a sample input with placeholder values

Change `contoso.com` in the script to your UPN suffix, fill in the CSV (the password column holds `<PASSWORD>`), and run from a machine with the ActiveDirectory module:

```powershell
Import-Module ActiveDirectory
.\scripts\New-AD-Users-from-CSV.ps1
```

Try it in a lab domain first.
