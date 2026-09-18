# Errors Part 2

### Error: Unknown network error

**Solution:** Check your internet connection and try again — this can also happen if you're using a VPN.

***

### Error: Failed to allocate memory/to map memory (x). Please reboot PC and try again

**Solution:** The driver was installed incorrectly. Reboot your PC and try again (on an internet cafe PC, try a different machine if the error repeats). If that doesn't help, clean up your autorun programs — [Autoruns](https://learn.microsoft.com/en-us/sysinternals/downloads/autoruns) can help you disable non-system startup entries, since drivers from deleted programs can sometimes linger.

***

### Error: Failed to load dependencies(x)(-x). Make sure all antiviruses are disabled

**Solution:** Turn off all protection and remove any anti-cheat readers and antiviruses from your PC. If that doesn't help, clean up your autorun programs.

***

### Error: Please uninstall Vanguard/Faceit first

**Solution:** Uninstall the Vanguard/Faceit anti-cheat from your PC and try again.

***

### Error: AES instruction set is not supported

**Solution:** Your processor doesn't support the AES instruction set, so this can't be fixed.

***

### Error: Please enable Intel VT-X/AMD-V in the BIOS

**Solution:** Enter the BIOS and enable the feature named "Intel Virtualization Technology," "Intel VT-X"/"AMD-V," or "SVM Mode."

***

### Error: VMX/SVM is not supported

**Solution:** Go to Control Panel → Programs and Features → Turn Windows features on or off, and make sure "Virtual Machine Platform" and "Hyper-V" are both disabled.

{% hint style="info" %}
If the error persists, open cmd as an administrator and run `bcdedit /set hypervisorlaunchtype off` (no quotes), then restart your computer.
{% endhint %}

If you're on Windows 11 and the above didn't help, run PowerShell as an administrator and paste in the following (in full):

```
takeown /F "C:\Windows\System32\hvix64.exe" icacls "C:\Windows\System32\hvix64.exe" /grant *$(([System.Security.Principal.WindowsIdentity]::GetCurrent()).User.Value):For takeown /F "C:\Windows\System32\hvax64.exe" icacls "C:\Windows\System32\hvax64.exe" /grant *$(([System.Security.Principal.WindowsIdentity]::GetCurrent()).User.Value):F del "C:\Windows\System32\hvix64.exe" del "C:\Windows\System32\hvax64.exe"
```

***

### Error: Either virtual or RAID disk is present. Please revert it back to normal state

**Solution:** Turn off the spoofer, or disable RAID in the BIOS settings and do a full reinstall of Windows.

***

### Error: Unsupported firmware

**Solution:** Convert the OS disk to GPT (the built-in `mbr2gpt` tool works, or any disk management utility), and switch the BIOS from Legacy mode to UEFI mode.

***

### Error: CRD failed at XXX with code XXXXXXXX / Failed to init render

**Solution:** On desktop, the graphics card is too old and unsupported. On laptop, disable the built-in graphics card in the BIOS.

***

### Error: Incorrect HWID

**Solution:** Open cmd as administrator and run these commands one at a time:

```
wmic diskdrive get Caption, SerialNumber
```

```
wmic baseboard get SerialNumber
```

{% hint style="info" %}
If either command fails, something else is wrong with your PC — try reinstalling Windows and check whether the problem goes away.
{% endhint %}
