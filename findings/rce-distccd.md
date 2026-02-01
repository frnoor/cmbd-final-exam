# Remote Command Execution (distccd)
## Risk Level: High
## Description
The `distccd` service was configured to allow unauthenticated command execution from remote hosts.
## Impact
Allows an attacker to execute arbitrary code with the privileges of the service user, leading to a complete shell foothold.
## Recommendation
Restrict `distccd` access to authorized IP addresses via firewall and update to a version requiring authenticated communication.
