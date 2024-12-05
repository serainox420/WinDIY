# WinDIY
> ### Windows "Do It Yourself"
> Collection of various both Official & Unoficial tools and resources for debloating & customizing Windows yourself!\
> **"If you have to use Windows, at least make it usable" ~ sx**

> # Windows .ISO
> ### **Official: [Microsoft.com]**
> For oficial, maximally debloated Windows 11, download 11 LTSC Enterprise edition .iso from:\
> [Windows 11 LTSC Enterprise](https://www.microsoft.com/en-us/evalcenter/download-windows-11-iot-enterprise-ltsc-eval) \
> [Windows 10 LTSC Enterprise](https://www.microsoft.com/de-de/evalcenter/download-windows-10-enterprise)\
> Enterprise edition minimizes inclusion of non-essential Microsoft features to enhance performance and reduce potential disruptions from frequent updates, for example Microsoft Store, Cortana, Edge etc are not included.
> 
> ---
> ### **Unofficial**
> **Vanilla**\
> Default archival .iso files\
> [Internet Archive - Windows 7 Enterprise](https://archive.org/download/en_windows_7_enterprise_with_sp1_x64_dvd_u_677651_202107)\
> **Fork**\
> If you preffer already maximally debloated Windows ISO, called "Blessed" from my friend PandoraMishima, feel free to get it here:\
> [Windows Blessed](https://mega.nz/folder/fp5T1D7Z#hCIXPPQSb4RCkmcb9sCxUA)

---

# Tools

> ### Activation
> [Microsoft Activation Tool](https://github.com/massgravel/Microsoft-Activation-Scripts) \
> [Microsoft Product Keys](https://gist.github.com/rvrsh3ll/0810c6ed60e44cf7932e4fbae25880df)

---

# Debloating
> ### Microsoft Application Wizard
> Launches the Programs and Features window, allowing you to manage installed applications and optional Windows features.\
Accessible by pressing Win + R, typing ```appwiz.cpl```, and pressing Enter.\
The "Turn Windows features on or off" option is available on the left-hand side.
>
> ---
>
> ### PowerShell
> Open PowerShell as administrator, and type:\
> **To list all Microsoft features you can disable / enable**\
> ```Get-WindowsOptionalFeature -Online | Where-Object State -EQ "Disabled"``` \
> **Enable a feature** (Put actual feature name in "FeatureName")\
> ```Enable-WindowsOptionalFeature -Online -FeatureName "FeatureName"``` \
> **Disable a feature**\
> ```Disable-WindowsOptionalFeature -Online -FeatureName "FeatureName"```\
