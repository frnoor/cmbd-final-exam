# Kernel and System Hardening
## 1. Patch Management
The most effective defense against Dirty COW and similar kernel exploits is a robust patch management lifecycle. 
- **Action:** Automate security updates for critical system headers and the Linux kernel.

## 2. Principle of Least Privilege
Regularly audit SUID/SGID binaries to reduce the attack surface for local privilege escalation.
- **Action:** Remove the SUID bit from non-essential binaries like `exim4`.

## 3. Defense in Depth
Implement AppArmor or SELinux profiles to restrict the capabilities of service users (like `distccd`), preventing them from accessing or writing to sensitive system files even if the service is compromised.
