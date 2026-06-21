# Microsoft Visio Diagram and Stencil Troubleshooter

Created by **Dewald Pretorius**.

The repository includes the original diagram, stencil, shape, template, rendering, and printing diagnostics plus a guarded `Repair.ps1` helper.

```powershell
.\Repair.ps1 -Action Diagnose
.\Repair.ps1 -Action ResetOfficeCache -WhatIf
.\Repair.ps1 -Action ResetOfficeCache -Confirm
```

Visio must be closed before repair. Existing Office cache data is preserved as a timestamped backup, and the diagnostic snapshot inventories the user's custom stencil folder. Source-reviewed for PowerShell 5.1; not runtime-tested against every diagram or Visio build.
