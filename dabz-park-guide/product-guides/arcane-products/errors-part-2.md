# Errors Part 2

#### <mark style="color:$danger;">Error: Unknown network error.</mark>

* Solution: Problem with your internet connection, you need to check your connection and try again, maybe you are using VPN.

#### <mark style="color:$danger;">Error: Failed to allocate memory/to map memory (x) Please reboot pc and try again.</mark>

* Solution: The driver was installed incorrectly, you need to reboot the pc and try again(If you are in an internet cafe but the error is recurring, you need to try another PC). If it doesn't help, clean the autorun programs. If the error still persists, we recommend downloading Autoruns - https://learn.microsoft.com/en-us/sysinternals/downloads/autoruns and disabling all programs that are in the startup list but are not system programs. In some cases, drivers for deleted programs may remain in the system.

#### <mark style="color:$danger;">Error: Failed to load dependencies(x)(-x) Make sure all antiviruses are disabled.</mark>

* Solution: You need to turn off all protection and remove all anti-readers and antiviruses from your PC. If it doesn't help, clean the autorun programs.

#### <mark style="color:$danger;">Error: Please uninstall Vanguard/Faceit first.</mark>

* Solution: You need to uninstall the Vanguard/Faceit antichip from your PC and try again.

#### <mark style="color:$danger;">Error: AES instruction set is not supported.</mark>

* Solution: This error means the processor does not support AES instruction set, so it cannot be fixed.

#### <mark style="color:$danger;">Error: Please enable Intel VT-X/AMD-V in the BIOS.</mark>

* Solution: To fix this error, enter the BIOS and search for a feature named either "Intel virtualization technology" or "Intel VT-X"/"AMD-V" or "SVM mode" and enable it.

#### <mark style="color:$danger;">Error: VMX/SVM is not supported.</mark>

* Solution: To fix this error, go to "Control Panel" -> "Programs and Functions" -> "Enable or disable Windows Functions" and make sure that "Virtual Machine Platform" and "Hyper-V" are disabled.

{% hint style="info" %}
If the error persists, open cmd as an administrator and enter the following command without quotes "bcdedit /set hypervisorlaunchtype off", then press Enter and restart the computer.
{% endhint %}

If the Windows 11 user and the previous methods did not help him, then you should run PowerShell as an administrator and paste the following command there (in full):

```
takeown /F "C:\Windows\System32\hvix64.exe" icacls "C:\Windows\System32\hvix64.exe" /grant *$(([System.Security.Principal.WindowsIdentity]::GetCurrent()).User.Value):For takeown /F "C:\Windows\System32\hvax64.exe" icacls "C:\Windows\System32\hvax64.exe" /grant *$(([System.Security.Principal.WindowsIdentity]::GetCurrent()).User.Value):F del "C:\Windows\System32\hvix64.exe" del "C:\Windows\System32\hvax64.exe"

```

#### <mark style="color:$danger;">Error: Either virtual or RAID disk is present. Please revert it back to normal state.</mark>

* Solution: Turn off the spoofer or turn off the RAID in the BIOS settings with a complete reinstallation of Windows.

#### <mark style="color:$danger;">Error: Unsupported firmware.</mark>

* Solution: To fix this error, convert the disk containing the operating system to GPT format using the mbr2gpt tool built into Windows or any other disk management utility of your choice. The BIOS needs to switch from Legacy mode to UEFI mode.

#### <mark style="color:$danger;">Error: CRD failed at XXX with code XXXXXXXX / Failed to init render.</mark>

* Solution: For PC, the graphics card is old and unsupported. For laptops, you need to disable the built-in graphics card in the BIOS.

#### <mark style="color:$danger;">Error: Incorrect HWID.</mark>

* Solution: Open cmd as administrator, enter these commands one by one

```
wmic diskdrive get Caption, SerialNumber
```

```
wmic baseboard get SerialNumber
```



{% hint style="info" %}
if any of those commands failed with an error then something is wrong with your pc, try to reinstall Windows and check if the problem is gone.
{% endhint %}
