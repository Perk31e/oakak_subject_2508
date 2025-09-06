# oakak_subject_2508
To Provide Solution for ryk

## Repository Contents

### Analysis Tools
- `decrypt.py` - Decrypts RYK ransomware encrypted files (requires valid decryption key)
- `ryuk.yara` - YARA rules for RYK ransomware detection using IOCs
- `check_digitalsig.ps1` - PowerShell script to verify digital signatures of binary files

### SIEM Integration
- `SecuritySolution_Rules/for_client/ossec.conf` - Wazuh agent configuration for log collection and FIM
- `SecuritySolution_Rules/for_client/sysmon_ryk_client.xml` - Sysmon configuration for RYK-specific event logging  
- `SecuritySolution_Rules/for_server/local_rules.xml` - Wazuh server rules to process Sysmon events

### Update Log

2025-08-28 Add yara rule, decrypt.py
2025-09-02 Add Check_digitalsig.ps1
2025-09-06 Add Wazuh+Sysmon Rules

### Known Issues
- SIEM rules require testing and validation in production environment
- Event collection needs optimization to reduce false positives
- Documentation needs expansion for deployment procedures

![No Error with local_Rules.xml](https://github.com/user-attachments/assets/d9c70d50-6a94-4225-9a6a-bc2760a31747)  <br />
![No Error with sysmon_ryk_client.xml](https://github.com/user-attachments/assets/20a3f861-3d10-4694-b59b-caac854c27ae)  <br />
