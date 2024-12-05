# WinDIY
> ### Windows "Do It Yourself"
> Collection of various both Official & Unoficial tools and resources for debloating & customizing Windows yourself!\
> **"If you have to use Windows, at least make it usable" ~ sx**

---

> ## Contents:
1. [**System Image**](https://github.com/serainox420/WinDIY/edit/personal/README.md#system-image)
   - Official
   - Unofficial
3. **Tools**
   - Official
   - Unofficial
4. **Command Line**
   - Microsoft Application Wizard
   - PowerShell
   - DISM
   - Export Windows Image
6. **Miscelanous Software**

--- 

> ## **System Image**
> #### **Official Microsoft™** 
> For oficial, maximally debloated Windows 11, download 11 LTSC Enterprise edition .iso from:\
> [Windows 11 LTSC Enterprise](https://www.microsoft.com/en-us/evalcenter/download-windows-11-iot-enterprise-ltsc-eval) \
> [Windows 10 LTSC Enterprise](https://www.microsoft.com/de-de/evalcenter/download-windows-10-enterprise)\
> Enterprise edition minimizes inclusion of non-essential Microsoft features to enhance performance and reduce potential disruptions from frequent updates, for example Microsoft Store, Cortana, Edge etc are not included.
> 
> ---
> #### **Unofficial / Third Party** 
> **Vanilla**\
> Default archival .iso files\
> [Internet Archive - Windows 7 Enterprise](https://archive.org/download/en_windows_7_enterprise_with_sp1_x64_dvd_u_677651_202107)\
> **Fork**\
> If you preffer already maximally debloated Windows ISO, called "Blessed" from my friend PandoraMishima, feel free to get it here:\
> [Windows Blessed](https://mega.nz/folder/fp5T1D7Z#hCIXPPQSb4RCkmcb9sCxUA)

---

> ## Tools
> #### **Official Microsoft™**
> ### Activation
> [Microsoft™ Activation Tool](https://github.com/massgravel/Microsoft-Activation-Scripts) - Activate Windows / Office\
> [Microsoft™ Product Keys](https://gist.github.com/rvrsh3ll/0810c6ed60e44cf7932e4fbae25880df) - Some default Windows product keys\
> [Microsoft™ Deployment Toolkit](https://www.microsoft.com/en-us/download/details.aspx?id=54259) - Official tool for automating the deployment of Windows operating systems.\
> [Microsoft™ Media Creation Tool](https://support.microsoft.com/en-us/windows/create-installation-media-for-windows-99a58364-8c02-206f-aa6f-40c3b507420d) - Official tool for creating personalized Windows .iso
>
> ---
 
> ## Command Line
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
>
> ---
>
> ### DISM
> **(Deployment Image Servicing and Management)**\
> A built-in Windows tool to manage and modify Windows images (WIM or VHD files) and enable/disable Windows features.\
> Enable feature: \
> `DISM /Online /Enable-Feature /FeatureName:FeatureName /All` \
> Disable feature: \
> `DISM /Online /Disable-Feature /FeatureName:FeatureName`\
> Export Current System to ISO \
> `DISM /Capture-Image /ImageFile:C:\CustomInstall.wim /CaptureDir:C:\ /Name:"Custom Windows Image"`
>
> ---
#### Creating .iso
> ### PowerShell
> `Export-WindowsImage -SourceImagePath "C:\Path\install.wim" -DestinationImagePath "C:\CustomInstall.iso" -SourceIndex 1`

---

> #### Miscelanous Software
> [NTLite](https://www.ntlite.com) -  GUI-based tool for modifying Windows installation ISOs \
> [Media Creation Wrapper](https://github.com/AveYo/MediaCreationTool.bat) - A community script that customizes the official Microsoft Media Creation Tool. \
> [O&O ShutUp10++](https://www.oo-software.com/en/shutup10) - A privacy-focused tool for tweaking Windows 10/11 settings. \
> [Balena Etcher](https://etcher.balena.io) - Flash any system .iso on portable media like USB or CD \
> [Rufus](https://rufus.ie/en/) - Create bootable media on USB \
> [WimLib](https://wimlib.net) - An open-source tool for managing Windows WIM files. \
> [WinReducer](https://www.winreducer.net) - A GUI-based tool for customizing Windows ISO files, similar to NTLite. \
> [Chocolatey](https://chocolatey.org) - A package manager for Windows that automates software installation via scripts. \
