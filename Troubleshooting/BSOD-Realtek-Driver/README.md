
##  Troubleshooting Case Study: BSOD Analysis (Realtek USB WiFi Driver)

### Error Details
- Bug Check String: `SYSTEM_THREAD_EXCEPTION_NOT_HANDLED`
- Bug Check Code: `0x1000007e`
- Triggered Module: `ks.sys`
- Root Cause Driver: `RtUsbA64_03F00269.sys` (Realtek USB WiFi)

### Summary
This case study documents the investigation and resolution of a BSOD encountered while running a Kali Linux VM and configuring proxy interception with Burp Suite. Minidump analysis identified a Realtek USB WiFi network driver fault aggravated by VM networking load.

### Tools Used
- BlueScreenView
- Minidump analysis
- Device Manager diagnostics
- Power configuration review
- VM network mode testing

### Key Findings
- Realtek USB drivers are unstable under VM bridged networking
- USB Selective Suspend contributed to driver crashes
- Switching VM network mode to NAT prevents recurrence
- Power management settings directly affect driver stability

### Included Documentation
📄 **[BSOD Fix Guide (pdf)](Troubleshooting/BSOD-Realtek-Driver/BSOD_FIX_GUIDE.pdf)**  
