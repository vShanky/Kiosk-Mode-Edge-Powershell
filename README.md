# Kiosk-Mode-Edge-Powershell

A simple PowerShell script to set up Windows Kiosk Mode using Microsoft
Edge and a predefined website.

## How It Works

-   Creates a kiosk user\
-   Sets Microsoft Edge as the kiosk app\
-   Opens your chosen website automatically\
-   Auto-logs into kiosk mode after reboot

## Usage

Edit the first three variables in `BootToKiosk.ps1`:

``` powershell
$domain   = "KioskUserName"
$password = "KioskUserPassword"
$website  = "https://your-website-url.com"
```

Run as Administrator:

``` powershell
powershell -ExecutionPolicy Bypass -File .\BootToKiosk.ps1
```

## Compatibility

-   Fully works on **Windows 10 (below 21H2)**
-   Limited support on **Windows 10 21H2+**

## License

BSD-3 Clause License.\
Based on the original idea by ProRedMax.
