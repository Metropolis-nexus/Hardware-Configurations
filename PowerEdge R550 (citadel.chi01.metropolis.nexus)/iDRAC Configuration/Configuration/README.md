## Configuration

### Power Management
- Do **NOT** enable power cap. It breaks BIOS live scanning.
- Set power to A/B Grid redundant.
- Make sure hot spare is enabled.

### Virtual Console
- Keep VNC server disabled, but change SSL Encryption to 256-Bit or higher.

### Licenses
- Upgrade to Datacenter license

### System settings

#### Alert Configuration
- Alerts -> Enable
- Quick Alert Configuration -> Select all categories, critical and warning, recieve notifications with email
- Alert Configuration -> Security Event -> Enable informational email notifications
- SMTP (Email) Configuration -> Add email address to receive notifications and check the "State" checkbox

#### Hardware Settings
- Thermal Profile Optimization -> Maximum Performance
- Fan speed offset -> Low (Shouldn't be needed, but the P4608 drives *allegedly* has very low max operating temperature according to *some websites*)
- Maximum PCIe Inlet Temperature Limit -> 45 °C

### BIOS Setting
- Verify everything is as expected with what's set in System BIOS.
- System Security -> Measure UEFI CA Scope Setting to TPM PCR[7] -> Yes