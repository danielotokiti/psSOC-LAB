## Day 3 – Atomic Red Team + MITRE Attack Simulation + Wazuh Dashboard Customization

### Tasks Completed
- Cloned Atomic Red Team repo inside the Windows VM  
- Installed `Invoke-AtomicRedTeam` PowerShell module manually (offline)  
- Resolved PowerShell module dependency (`powershell-yaml`) using `.nupkg`
- Integrated Windows Defender and Sysmon logs in the OSSEC Config file.  
- Ran MITRE simulation: T1059.001 (PowerShell command execution) and T1003.001 (Credential Dumping)
- Customized File Integrity Monitoring to monitor Windows VM download folder
  


### Screenshots 
- Cloning Atomic Red Team in PowerShell  
- Running `Invoke-AtomicTest T1059.001` and `Invoke-AtomicTest T1003.001`  
- Event logs showing proof of threat hunting and file integrity monitoring. 



### Key Commands
```powershell
# Clone Atomic Red Team & Invoke module
git clone https://github.com/redcanaryco/atomic-red-team.git
git clone https://github.com/redcanaryco/invoke-atomicredteam.git

# Import attack module
Import-Module "C:\Windows\System32\atomic-red-team\invoke-atomicredteam\Invoke-AtomicRedTeam.psd1"

# Run MITRE ATT&CK test
Invoke-AtomicTest T1059.001


