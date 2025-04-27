# Frida-Scripts
Frida Scripts To Bypass SSL Pinning

# Usage
You don't need to configure iptables for Android or OpenVPN for iOS. Just follow the steps below.
```
1. Set up burp invisible proxy on the host machine
```

2. Specifiy burp ip and port on the script
At the very end of the script.js, specifiy BURP_PROXY_IP and BURP_PROXY_PORT

3. Attach
frida -Uf <package name> -l Flutter-SSL-Pinning.js
