# Example of how I troubleshoot problems using the CompTIA troubleshooting methodology
Troubleshooting is an essential skill for IT professionals, as a significant portion of our work involves identifying why systems or devices aren't functioning as expected. While experience plays a major role in developing the ability to resolve computer and network issues, there is also a structured framework that helps guide the diagnostic process and leads us to effective solutions.

Although this content isn’t unique to CompTIA, it’s worth noting that nearly every CompTIA certification includes objectives focused on troubleshooting methodology. This structured process has been developed over time through real-world experience and serves as a valuable guide for newcomers in the IT field when approaching problem-solving.
### Here is the CompTIA troubleshooting methodology:
  - Identify the problem
  - Establish a theory of probable cause
  - Test the theory to determine the cause
  - Establish a plan of action to resolve the problem and identify potential effects
  - Implement the solution or escalate as necessary
  - Verify full system functionality and, if applicable, implement preventive measures
  - Document findings, actions, outcomes and lessons learned
## Example of how I used CompTIA troubleshooting methodology

![Image](https://github.com/user-attachments/assets/92132aff-74df-4a06-b8c6-f14115d1e075)

I log in to Peppermint and I see that a ticket that has not been solved. The title of the ticket is named "Internet not working!"

I click on the ticket and I read the rest of the message. 

The contact was my Mom. She has sent a ticket saying that the internet does not work despite the router being plugged in. Plus, her devices were not being connected to the internet. 

![Image](https://github.com/user-attachments/assets/f8d03c74-12b6-4dce-81da-c4a3a7490790)

So I start with the first step in the CompTIA Troubleshooting methodology which is **identify the problem.**

1. **Identify the Problem**
  - I ask the client questions:
    - “When did this issue start?”
    - "Did anything change recently? (for example: new device, storm, service outage)”
  - Checked the connections:
    - Ensure the router’s WAN port is connected to the modem.
    - Verify router lights (Power, Internet, Wi-Fi) are showing proper status.
2. **Establish a Theory of Probable Cause**
  - Some potential causes:
    - Router has lost internet connection (ISP issue or bad modem).
    - Wi-Fi is enabled, but internet is not being routed.
    - DHCP is not assigning IP addresses to devices.
    - DNS misconfiguration.
    - MAC address filtering or security settings blocking devices.
3.  **Test the Theory to Determine Cause**
  - Ping router’s IP address (e.g., 192.168.1.1) from a connected device.
    - If successful: LAN works, issue might be external (modem/ISP).
    - If unsuccessful: DHCP or router issue.
  - Check IP settings on a device (ipconfig)
    - If IP address is 169.x.x.x, the device is not receiving an IP from the router.
  - Login to router admin panel to verify:
    - WAN IP status.
    - DHCP server settings.
    - Wireless status (SSID broadcast and security settings).
    - Check for firmware updates.
4. **Establish a Plan of Action**
  - Based on the findings:
    - If WAN IP is missing → reboot modem & router.
    - If DHCP is disabled → re-enable and restart router.
    - If devices are blocked or MAC filtering is enabled → disable or adjust list.
    - If router is faulty → replace or escalate to networking team.
5. **Implement the Solution**
  - Reboot modem and router in sequence (modem first, then router).
  - Reset network settings or reconfigure DHCP.
  - Update firmware if needed.
  - Restore router to factory defaults (as a last resort) and reconfigure.
6. **Verify Full System Functionality**
  - Confirm all devices can now connect to the internet.
  - Run speed test to confirm performance.
  - Ask client (in this case, the client is my mom) to test email, browsing, and streaming.
7. Document Findings, Actions, and Outcomes
  - Problem: "Client (my mom) unable to connect personal devices to internet; router was powered on."
  - Cause: "Router DHCP service was disabled after recent power outage."
  - Resolution: "Re-enabled DHCP and rebooted router/modem."
  - Outcome: "All client devices restored to full connectivity."

Using the CompTIA troubleshooting methodology, I was able to close the ticket successfully! 


