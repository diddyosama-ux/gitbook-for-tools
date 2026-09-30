---
icon: triangle-exclamation
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: true
  actions:
    visible: true
  anchors:
    visible: true
---

# Anti Virus Setup

Before you begin, you may be wondering why the tool requires certain Windows security settings to be changed. Some tools use drivers that Windows does not allow to run by default, which can cause errors or prevent the tool from working properly.

#### <mark style="color:blue;">**Anti-Virus Setup**</mark>

{% stepper %}
{% step %}
### <mark style="color:blue;">Make Sure Your Turn Off All Virus & Threat Protection</mark>
{% endstep %}

{% step %}
### <mark style="color:blue;">Download Windows Disabler</mark>

Download [Sordum Defender Control](https://www.sordum.org/files/downloads.php?st-defender-control=)
{% endstep %}

{% step %}
### <mark style="color:blue;">Download File Extracter</mark>

Download [Winrar](https://www.win-rar.com/fileadmin/winrar-versions/winrar/winrar-x64-701.exe)
{% endstep %}

{% step %}
### <mark style="color:blue;">Open Defender Control using Winrar.</mark>

Use the Password 'sordum' To Extract.
{% endstep %}

{% step %}
### <mark style="color:blue;">Run The Program & Disable Antivirus</mark>
{% endstep %}

{% step %}
### Now turn all 3 options in your Firewall off.

<figure><img src="../.gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### <mark style="color:blue;">Now Head To "App & Browser Control"</mark>

Scroll Down To "Exploit Protection" & click "Exploit Protection Settings"

<figure><img src="../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### <mark style="color:blue;">Turn These All Off ONE BY ONE</mark>

<figure><img src="../.gitbook/assets/image (68).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### <mark style="color:blue;">In "DEVICE SECURITY" Make Sure "Core Isolation" Is All Off.</mark>

<figure><img src="../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

<br>

### <mark style="color:blue;">**CPU Virtualization Setup**</mark>

{% stepper %}
{% step %}
### Open Task Manager And Click On "Performance"

<figure><img src="../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Make Sure Virtualization Is Enabled,

once again if its Disabled you will need to go into your BIOS and enable it. If your stuck once again search up a youtube tutorial.
{% endstep %}
{% endstepper %}

<br>

### **Faceit / Riot Clients**

{% stepper %}
{% step %}
### Search Add Or Remove Program

<figure><img src="../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Make Sure There Is None Of The Following Are Enabled:

* RIOT CLIENT
* VANGUARD
* FACEIT
* Or Any Other 3rd Party Antivirus Software
{% endstep %}
{% endstepper %}

1.
