---
description: >-
  We highly recommend you to follow these steps if you are experiencing troubles
  with launching our software:
icon: joystick
---

# Predator Products

<details>

<summary>Required Disabled</summary>



* Disable antivirus + delete it if needed
* Disable Microsoft Defender
* Disable all driver Anti-cheats: For Faceit: launch cmd as an admin and write "sc stop faceit" For Valorant: launch cmd as an admin and write "sc stop vgc" then "sc stop vgk"
* Make sure, that you are NOT using "-vulcan" launch option (we do not support it)
* Make sure, that time in Windows settings is synchronized
* Make sure, you have last version of Steam/other launcher. Do manual update check or reinstall it

</details>

> #### **List of known problems & their solution:​**

<mark style="color:$danger;">**1) Problem: "An error occured in the secure channel support" / "The request has timed out" / "The operation timed out"**</mark>\
\
Solution: Traffic is being blocked by something (Anti-cheat, Anti-virus, Firewall, Internet provider):\
\- Fully delete anti-virus + other anti-cheats - sometimes disabling it is not enough, it requires full uninstallation;\
\- Resync your time + region in Windows settings;\
\- Try out enabling/disabling vpn\
\
<mark style="color:$danger;">**2) Problem: "Hardware mismatch"**</mark>\
\
Solution: HWID (Hardware ID) can be reset only once in 7 days here - [https://predator.systems/panel/hardware-reset](https://predator.systems/panel/hardware-reset)\
\- This error appears in case something has changed in your PC from previous inject\
\
<mark style="color:$danger;">**3) Problem: "Internal public server error"**</mark>\
\
Solution: Traffic is being blocked by something (Anti-cheat, Anti-virus, Firewall, Internet provider):\
\- Fully delete anti-virus + other anti-cheats - sometimes disabling it is not enough, it requires full uninstallation\
\
<mark style="color:$danger;">**4) Problem: Infinite "Waiting for the game initialization" (Marvel Rivals)**</mark>\
\
Solution: Follow these steps\
\- Should be launched through steam only, not other launchers\
\- Steam overlay must be turned on. Press Shift + Tab while compiling shaders\
\- Remove all launch options and add these: -d3d12 -dx12\
\
<mark style="color:$danger;">**5) Problem: "Antivirus Interference detected"**</mark>\
\
Solution: Traffic is being blocked by something (Anti-cheat, Anti-virus, Malware):\
\- Fully delete anti-virus + other anti-cheats - sometimes disabling it is not enough, it requires full uninstallation;\
\- Scan your PC with some tools to make sure that your computer is not infected. (Example of the tool for scan: [https://free.drweb.ru/cureit/](https://free.drweb.ru/cureit/))\
\
<mark style="color:$danger;">**6) Problem: Reason: \[\<code>] sym: \<some info>**</mark>\
\
Solution: Create ticket in support section ([https://predator.systems/support](https://predator.systems/support)). Provide screenshot of this information there: Press WIN + R, type "winver"\
\
<mark style="color:$danger;">**7) Problem: Reason: modules::load\_module: failed to create section**</mark>\
\
Solution: Fully delete anti-virus + other anti-cheats - sometimes disabling it is not enough, it requires full uninstallation
