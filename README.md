# RDAgent Installers

This repository contains MSI installer files for deploying the **Microsoft Remote Desktop Agent** and **Boot Loader** on Windows machines. These components are typically used in environments such as **Azure Virtual Desktop (AVD)** or **Windows Virtual Desktop (WVD)** to enable remote session capabilities.

## Repository Contents

| File | Description |
|------|-------------|
| `Microsoft.RDInfra.RDAgent.Installer-x64-1.0.10004.2100.msi` | Main Remote Desktop Agent installer for 64-bit Windows. |
| `Microsoft.RDInfra.RDAgentBootLoader.Installer-x64-1.0.8925.0.msi` | Boot Loader component for initializing the agent. |

## Usage

1. Download the required MSI files from this repository.
2. Run the installers with administrative privileges:

   ```powershell
   msiexec /i Microsoft.RDInfra.RDAgent.Installer-x64-1.0.10004.2100.msi /quiet
   msiexec /i Microsoft.RDInfra.RDAgentBootLoader.Installer-x64-1.0.8925.0.msi /quiet
   ```

3. (Optional) Reboot the system after installation for changes to take effect.

## Requirements

- Windows 10/11 or Windows Server 2016 and later
- Administrative rights to install software

## Notes

- These installers are typically used for onboarding virtual machines to Azure Virtual Desktop (AVD).
- Ensure that your system meets all prerequisites before installation (e.g., network connectivity, domain join status, etc.).

## License

Please refer to Microsoft's licensing terms when using these components. This repository is provided for convenience and internal deployment purposes.

---
**Repository**: [sariamubeen/RDAgent](https://github.com/sariamubeen/RDAgent)
