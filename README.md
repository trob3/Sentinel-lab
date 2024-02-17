Failed RDP to IP Geolocation Information
Description

The Powershell script in this repository is responsible for parsing out Windows Event Log information for failed RDP attacks and using a third-party API to collect geographic information about the attackers' location.

The script is used in this demo where I set up Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot. We will observe live attacks (RDP Brute Force) from all around the world. I will use a custom PowerShell script to Look up the attackers' Geolocation information and plot it on an Azure Sentinel Map!

![image](https://github.com/trob3/Sentinel-lab/assets/157558777/4e3b7e5a-b7d5-41bf-a77a-c5ba20c60af0)

Languages Used
PowerShell: Extract RDP failed logon logs from Windows Event Viewer
Utilities Used
ipgeolocation.io: IP Address to Geolocation API
Attacks from China coming in; Custom logs being output with geodata


![image](https://github.com/trob3/Sentinel-lab/assets/157558777/b45b3d7f-c4b4-4277-8dee-631b1308f1e3)

World map of incoming attacks after 24 hours (built custom logs including geodata)

![image](https://github.com/trob3/Sentinel-lab/assets/157558777/52243c9f-4640-41ef-8a1b-9cf8c4b41549)


