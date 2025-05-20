## System Security

- Set Setup Password
- Password Status -> Locked
- TPM Security -> On
- TPM Advanced Settings
    - TPM PPI Bypass Provision -> Enabled
    - TPM PPI Bypass Clear -> Enabled
    - TPM2 Algorithm Selection -> SHA256
- Memory Encryption -> Single Key (because the Xeon Silver 4310 only supports single key)
- SMM Security Mitigation -> Enabled
- Secure Boot -> Enabled
- Secure Boot Policy -> Custom
- Secure Boot Custom Policy Settings -> Delete All Policy Entries
- UEFI CA Certificate Scope -> Device Firmware

![Security 1](Security-1.png)
![Security 2](Security-2.png)
![Security 3](Security-3.png)
![Security 4](Security-4.png)
![Security 5](Security-5.png)