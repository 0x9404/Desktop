# Desktop Windows 11



### Viewing network interfaces
- *>* netsh
- *netsh>* interface ipv4
- *netsh interface ipv4>* show interfaces



### Windows OOBE
- Unplug ethernet or disable NIC
- *>* OOBE\\BYPASSNRO

### Find windows product key
- *>* wmic path softwarelicensingservice get OA3xOriginalProductKey

### Azure AD enrollment status
- *>* dsregcmd /status

### Updating Group Policy settings
- *>* gpupdate /force

### View process with path
- *>* wmic process get ProcessID,ExecutablePath

### View directory structure with size
- *>* dir /s /w [:\drive]

### View largest files for the current user
- *>* dir $env:USERPROFILE -Recurse -File | Sort Length -Descending | Select-Object Length,FullName

### Drive mapping
- *>* NET USE V: /DELETE /Y
- *>* NET USE V: "\\github\"

### Show privileges
- *>* whoami /all
