# Kernel Privilege Escalation (Dirty COW)
## Risk Level: Critical
## Description
The target system was running an outdated Linux kernel (v2.6.x) vulnerable to CVE-2016-5195. This race condition allows unauthorized modification of read-only memory mappings.
## Impact
**Full System Compromise.** Successful exploitation allowed the injection of a root-privileged user (`toor`) into `/etc/passwd`.
## Recommendation
Apply the latest kernel security patches (Kernel 4.8.3 or higher) immediately.
