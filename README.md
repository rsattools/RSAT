## Download RSAT (Remote Server Administration Tools)

Download latest version from Releases:       
https://github.com/confyra/RSAT/releases/tag/1.412

RSAT allows IT professionals to manage Windows Server roles and features remotely from a device running either Windows 10 or Windows 7 Service Pack 1.

## Introduction

RSAT cannot be installed on systems running Home or Standard editions of Windows. It is exclusively available for Professional or Enterprise versions of the Windows client OS. Unless explicitly stated on the download page that RSAT supports a beta, preview, or other prerelease version of Windows, a full (RTM) release of the operating system is required for installation and use. Some individuals have resorted to manually bypassing the RSAT MSU restrictions to install it on unsupported editions or builds of Windows. Such actions violate the terms outlined in the Windows end-user license agreement.

Installing RSAT is comparable to installing Adminpak.msi on client machines running Windows 2000 or Windows XP. However, there's a key distinction: in Windows 7, the tools aren't available right after installation. You must manually activate the desired tools using the Control Panel. To do this, navigate to **Start** > **Control Panel** > **Programs and Features**.

In RSAT packages for Windows 10, all tools are enabled by default once installed. To disable any tools you don’t plan to use on Windows 7, open **Turn Windows features on or off**.

For Windows 7 users, it's necessary to manually enable the tools for the roles and features you intend to manage after completing the installation of the RSAT package.

If you're managing roles or features running on remote servers from Windows Server 2012 R2, there's no need to install additional tools. Launch the Add Roles and Features Wizard in Windows Server 2012 R2 or newer, then on the **Select Features** screen, expand **Remote Server Administration Tools**, choose the specific tools you need, and finish the wizard to complete the installation.

## RSAT for Windows 10, version 1809 or later versions

> **Note**
> The **Turn Windows features on and off** dialog in Control Panel is not available for use.

Installing RSAT in Windows 10 version 1809 and beyond differs slightly from earlier approaches. RSAT is now bundled with the operating system and can be installed through **Optional Features**.
