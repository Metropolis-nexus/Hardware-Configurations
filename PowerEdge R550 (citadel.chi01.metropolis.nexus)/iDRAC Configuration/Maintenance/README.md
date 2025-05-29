## Maintenance

### System Update

- Location Type: HTTPS
- Use default address
- Uncheck "Apply Downgrade Versions"
- Expired or invalid certificate action -> Show Error
- Server Certificate -> Upload downloads.dell.com current certificate
- Check for updates

Get the current certificate with: `</dev/null openssl s_client -connect <downloads.dell.com's IP>:443 -servername downloads.dell.com | openssl x509 > dell.cert`

### Automatic Updates

**Automatic Updates is only enabled for the time being, before proper Secure Boot can be set up with Proxmox.**
- Enable Automatic Update
- Location Type: HTTPS
- Use default address
- Uncheck "Apply Downgrade Versions"
- Start: 23:00 (We start 1 hour before BIOS Live scanning)

### Diagnostics

- BIOS Live Scanning -> Daily
- Time -> 0:00. There's a weird thing in iDRAC right now that makes it impossible to set the schedule time to be less than the current local time. One workaround is to copy the request as a curl command from the browser dev tools and change the date to the day after.

If it complains about a job existing, try setting it to "never", hit submit, then change to daily and resubmit.