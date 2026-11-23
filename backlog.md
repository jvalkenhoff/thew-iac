# THEW IaC - Backlog
Yes - Backlog text generated with AI.

Later
- [ ] Revisit existing-account password aging: currently manage password_expire_max (365) and password_expire_min (1) only. Add the 7-day warning and 45-day post-expiry inactivity settings when supported by the installed ansible-core version, or implement an idempotent chage fallback.
- [ ] Explore Packer + cloud-init for repeatable Debian provisioning and first boot networking.
- [ ] Investigate VMware Workstation provisioning with Vagrant.
- [ ] Review further separation of OS and Kubernetes-specific roles.
- [ ] Strengthen check-mode handling for dependent bootstrap steps.
- [ ] Reconsider SSH forwarding restrictions only after VS Code Remote SSH is no longer needed.
Decisions
- Bootstrap access stays manual during Ansible development.
- Use network_ for variables in the network role.
- Keep forwarding available for VS Code Remote SSH during development.
- Stage the network configuration separately from the actual cutover.