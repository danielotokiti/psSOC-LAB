Day 2 – Windows VM + Sysmon + Log Forwarding

## Task Completed
- Imported Windows 10 VM from Microsoft Edge developer image
- Installed Sysmon with SwiftOnSecurity configuration  
- Verified Sysmon operational logs in Event Viewer  
- Deployed Wazuh agent to forward logs  
- Confirmed agent connection to Wazuh manager


   
## Screenshots:
- Windows 10 VM + Installation of Sysmon
- Sysmon in event viewer
- Agent forwarding set up
- Confirmed agent connection to wazuh manager
  

## Key Commands
```powershell
sysmon64.exe -accepteula -i sysmonconfig.xml
msiexec /i wazuh-agent.msi /qn WAZUH_MANAGER='10.0.0.215'

