## Day 4 – Custom Detection Rules + Alert Output

### Tasks Completed
- Created a Wazuh rule to detect suspicious `powershell.exe` usage with Base64 encoding
- Tuned rules for `svchost.exe` to lower severity for common legitimate usage and reduce false positives
- Set up Slack integration for high-severity alerts

  


### Screenshots 
- local_rules.xml showing the new PowerShell and svchost rules
- Wazuh dashboard alert for a triggered Base64 PowerShell event
- Slack message from the Wazuh integration after an alert





