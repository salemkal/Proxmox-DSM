# Proxmox-DSM
Proxmox is a complete opensource server virtualization management solution. It offers the ability to manage virtual server (VPS) technology with the Linux OpenVZ and KVM technologies. Proxmox offers a web interface accessible after installation on your server which makes management easy, typically needing only a few clicks.

This DSM config will support parsing and alerting for almost all Proxmox events like kernel, ssh, authentication,pve-firewall - Proxmox VE Firewall Daemon, pvedaemon - Proxmox VE API Daemon, pveproxy - Proxmox VE API Proxy Daemon, pmxcfs - Proxmox Cluster File System and so on.

**This will be an open project so anyone can updates on this to make it even more better.**

# QRadar Changes

1. Create a new custom DSM called (Proxmox) using the DSM editor option under the admin settings window.
1. Once the custom DSM has been created close the window and click the Log Source Extensions option in the admin settings.
1. Click Add near the top right corner
1. Enter a name of "ProxmoxCustom_ext"
1. Select your newly created log source (Proxmox) that you created earlier.
1. Click the upload button and select the file "ProxmoxCustom_ext.xml"
1. Click done and proceed to open the DSM menu and select your log source (Proxmox) that you created earlier.
1. You will need to select Event Mappings tab in the DSM editor and create the manual entries located in the file "Event Mappings.txt"
1. Finally, you will need to create a new log source selecting the custom Log source type we just created.
