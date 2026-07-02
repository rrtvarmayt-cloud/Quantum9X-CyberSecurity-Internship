# Task 1 - Unauthorized Device Detection in a Corporate Network

## Objective

The objective of this task was to identify the active devices connected to my local network and understand how unauthorized devices can be detected using network scanning.

## Tools Used

- Nmap 7.99
- Windows Command Prompt
- Windows 11

## Procedure

1. Installed Nmap on my laptop.
2. Opened Command Prompt and used the `ipconfig` command to identify my network details.
3. Performed a network scan using:

```bash
nmap -sn 10.229.88.0/24
```

4. Observed all active devices detected by Nmap.

## Results

The following devices were detected:

- Motorola MotoBook 60 Pro (Laptop)
- Moto Edge 50 Fusion (Mobile Phone)
- Wi-Fi Router

No unauthorized devices were found during the scan.

## Conclusion

This task helped me understand how Nmap can be used to discover active devices on a network and verify whether any unknown or unauthorized devices are connected.
