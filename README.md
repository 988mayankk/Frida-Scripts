# Frida-Scripts
Frida Scripts To Bypass SSL Pinning for Flutter Applications

# Usage
You don't need to configure iptables for Android or OpenVPN for iOS. Just follow the steps below.
```
1. Set up burp invisible proxy on the host machine
```
```
2. Specifiy burp ip and port on the script
At the very end of the script.js, specifiy BURP_PROXY_IP and BURP_PROXY_PORT
```
```
3. Attach
frida -Uf <package name> -l Flutter-SSL-Pinning.js
```

# Credits
[reflutter](https://github.com/Impact-I/reFlutter)<br>
[NVISO blog post 1](https://blog.nviso.eu/2020/05/20/intercepting-flutter-traffic-on-android-x64/)<br>
[NVISO blog post 2](https://blog.nviso.eu/2022/08/18/intercept-flutter-traffic-on-ios-and-android-http-https-dio-pinning/)
