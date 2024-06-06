Bloatware Removal Script

- What it does:
  - Remove AppX Packages (listed)
  - Remove associated reg keys
  - Disable Windows Feedback
  - Removes Cortana from Search
  - Removes Web Results from search
  - Disables Wi-Fi Sense
  - Disables Live Tiles
  - Removes unwanted scheduled tasks (Xbox Live etc.)
  - Removes Windows 11 specific apps (Teams Chat for example)
  - Clears start menu
  - Disables the hidden surfing game in Edge
  - Removes Dell specific bloat (by detecting manufacturer and deploying appropriately)
  - Removes McAfee (if detected)
  - Removes Windows Backup (win10 only)

- Log file location:
  C:\ProgramData\Debloat\Debloat.log

- How to deploy via Intune:
  1. Download **debloat-intune-script.ps1** and save it on your computer
  2. Go to: https://intune.microsoft.com/?feature.msaljs=false#view/Microsoft_Intune_DeviceSettings/DevicesMenu/~/scripts
  3. Switch to "Platform Script" -> Add "Windows 10 or more"
  4. Enter name & description
  5. Upload the script file **debloat-intune-script.ps1**, select options as follow ![image](https://github.com/HPC-Germany/Debloat/assets/45611820/a0e75041-f208-462d-812a-63018e39c73c)
  6. Assign to the needed SecGrp or Devices -> Done

