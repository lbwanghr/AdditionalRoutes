# Additional Routes
> Additional routes is a native feature provided by **networksetup** in terminal, which could set up permanent routes under any network service.

This app provides a GUI to help you implement your route plan easily and safely.  
[Download](https://github.com/lbwanghr/AdditionalRoutes/releases/download/v1.0/AdditionalRoutes.app.zip) now!

## Security & Privacy
* This app neither requests privileges nor collects your information.  
* Any changes to additional routes can be reverted.

## Examples
### Case 1
Assume you have two network services "Ethernet"(192.168.0.0/24) and "Wi-Fi"(192.168.3.0/24), and your default network service is "Ethernet".  

If a host H1(192.168.3.14/24) under service "Wi-Fi" is unreachable, you need to add following additional routes.  

**Destination:** 192.168.3.0  
**Mask:** 255.255.255.0  
**Gateway:** 192.168.3.1  
**Network Service:** Wi-Fi  

### Case 2
Assume there is a router R1(192.168.1.1) connected with R0(192.168.0.1), and you are connected with R0 via service "Ethernet".  

If R1 is unreachable, you need to add following additional routes.  

**Destination:** 192.168.1.1  
**Mask:** 255.255.255.255  
**Gateway:** 192.168.0.1  
**Network Service:** Ethernet  

## Q&A 

**1. I deleted an additional route, but nothing seems to happen, what's going on?**  
The routing table may not refresh immediately, but restarting your mac could help.


---
If you have questions or typical cases to share with me, please email lbwanghr@icloud.com.
