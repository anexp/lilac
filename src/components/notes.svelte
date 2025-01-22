

<p>
# Windows and Linux Dual Boot - Time mismatch

# Set RealTimeIsUniversal to 1
New-ItemProperty -Path "HKLM:\System\CurrentControlSet\Control\TimeZoneInformation" -Name "RealTimeIsUniversal" -Value 1 -PropertyType DWord -Force

# Optional: Verify the value is set correctly
Get-ItemProperty -Path "HKLM:\System\CurrentControlSet\Control\TimeZoneInformation" -Name "RealTimeIsUniversal"

# To remove the value:
# Remove-ItemProperty -Path "HKLM:\System\CurrentControlSet\Control\TimeZoneInformation" -Name "RealTimeIsUniversal" -Force



# Winget blue text problem

Download from https://aka.ms/getwinget
Add-AppPackage -Path .\Microsoft.DesktopAppInstaller_8wekyb3d8bbwe.msixbundle
</p>