# Reconnaissance Phase
## Objective
Identify active hosts and accessible services within the target network segment.
## Techniques Used
- **Active Host Discovery:** Utilizing `netdiscover` to map the local layer-2 environment.
- **Port Scanning:** Conducting `nmap` service-intensity scans to fingerprint open ports and versions.
## Outcome
Identified an exposed `distccd` service (port 3632) and an outdated Linux kernel environment.
