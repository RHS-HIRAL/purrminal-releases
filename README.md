# Purrminal downloads

Desktop pets that grow while you work. Free to play, for Windows 10 and 11 (64-bit).

**[Download the latest release](https://github.com/RHS-HIRAL/purrminal-releases/releases/latest)** · [purrminal.com](https://purrminal.com)

This repository only hosts the downloads. The source code isn't public.

## Which file do I need?

Every release has three files:

| File | What it is |
|---|---|
| `Purrminal-Setup-<version>.exe` | The installer. Recommended. No admin rights needed. |
| `Purrminal-<version>-win-x64-portable.zip` | Portable version: unzip anywhere and run `Purrminal.exe`. Use it if Windows Smart App Control blocks the installer. |
| `SHA256SUMS.txt` | Checksums, to check that your download is exactly the file we published. |

## "Windows protected your PC"

Purrminal is new and not code-signed yet, so Windows SmartScreen warns about an unknown publisher the first time. Click **More info**, then **Run anyway**. If you'd like to be sure the file is ours first, check it as below.

## Check your download

In PowerShell, in the folder you downloaded to:

```powershell
Get-FileHash .\Purrminal-Setup-1.0.0.exe -Algorithm SHA256
```

The result must match the line for that file in the release's `SHA256SUMS.txt` (upper or lower case doesn't matter). If it doesn't, don't run it, and email us. Only download Purrminal from this page or from purrminal.com, which links here.

## What Purrminal connects to

Purrminal runs on your PC and talks only to your own computer (a small helper on `127.0.0.1`), with one exception: if you enter a Premium licence key or a coin code, the key and your PC name are checked through purrminal.com with Creem, our payment provider, and re-checked every few days. There is no tracking. Details: [privacy policy](https://purrminal.com/privacy).

## Uninstall

Settings > Apps > Purrminal > Uninstall. This also removes Purrminal's Claude Code hooks. Your pets and coins stay in `%LOCALAPPDATA%\Purrminal`, so reinstalling keeps them; delete that folder to remove them too.

## Help

- Questions, bugs, lost licence keys, moving Premium to a new PC: [hello@purrminal.com](mailto:hello@purrminal.com)
- FAQ: [purrminal.com/#faq](https://purrminal.com/#faq)
- Security problems: email [hello@purrminal.com](mailto:hello@purrminal.com) with "Security" in the subject, not in public.

## Licence

Purrminal is free to download and use under the [Terms of Service](https://purrminal.com/terms). The files here may not be modified or redistributed. Premium and coin packs are sold by Creem, our Merchant of Record.

Works with Claude Code. Not affiliated with or endorsed by Anthropic.
