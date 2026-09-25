# Wireless Security Monitoring with Kismet

## Overview

This lab focuses on wireless security monitoring and analysis using Kismet in a controlled Kali Linux environment.

The goal was to monitor wireless activity, observe security-related events, and understand what different Kismet alerts can indicate.

## Lab Environment

- Kali Linux
- Kismet
- Controlled wireless lab environment

## What I Observed

### DEAUTHFLOOD

Kismet detected a noticeable pattern of Deauthentication and Disassociation frames.

This type of alert can be associated with deauthentication activity, but the alert alone does not prove that an attack was successfully performed.

### NOCLIENTMFP

Kismet reported that a client did not support Management Frame Protection (MFP).

The absence of MFP can be a security consideration, but this alert by itself does not indicate malicious activity.

### SOURCEOPEN / SOURCEERROR

These events were related to the wireless monitoring source and its status during the monitoring session.

### ROOTUSER

Kismet was running with root privileges in the lab environment.

Root privileges may be required for some wireless monitoring operations. In production environments, using the minimum required privileges is preferable.

## Results

This lab provided practical experience with:

- Wireless network monitoring
- IEEE 802.11 activity
- Management Frames
- Deauthentication and Disassociation frames
- Management Frame Protection (MFP)
- Security event monitoring with Kismet

## Limitations

Kismet alerts should not automatically be treated as proof of an attack.

Further investigation, including packet capture and traffic analysis, would be required to confirm the cause of suspicious activity.

## Future Improvements

- Analyze captured traffic with Wireshark
- Compare Kismet alerts with packet-level evidence
- Add historical event analysis
- Develop custom detection rules
- Explore automated alerting

## Conclusion

This lab provided hands-on experience with wireless security monitoring using Kismet and improved my understanding of wireless management frames and security-related events.
