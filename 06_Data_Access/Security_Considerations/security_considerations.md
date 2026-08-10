Explanation: This section outlines considerations that must be taken in place to have proper security when accessing the management server.

Security Considerations
Management Server Isolation: The management server should be completely isolated and on its own VLAN so that it can’t be accessed anywhere except the access node.
Authentication Requirements: All users who access the Management Server should be properly authenticated and use MFA to reduce the risks of compromised accounts.
Logging and Monitoring: All actions should be audited and logged to ensure changes can be detected or monitored.
Security Practices: The only point of entry to these services should be the Management Server, all unused ports should be closed, all credentials should meet requirements for complexity and be stored in a credential vault.
