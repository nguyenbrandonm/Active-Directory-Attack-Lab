# Active-Directory-Attack-Lab

## Objective
The AD Attack Lab project aims to establish a controlled environment for simulating the mapping and attacking of a small AD environment. The primary goal is to experiment with and develop a methodical approach to enumeration, exploitation, and pivoting through the network, from regular workstations up to compromising Windows Server / Domain Administrator. The lab supports two complementary configurations:

* Dual-NIC simulated compromise (pivot practice)
* Attack-and-enumerate configuration (standalone)

Both configurations follow a standard methodology: recon, enumeration, exploitation, escalation, lateral movement, and maintain/cleanup. The lab emphasizes an iterative workflow where initial enumeration and attacks feed into post-compromise enumeration and follow-on attacks that conclude with persistence and cleanup.

## Lab Topology and Machines

This lab uses four virtual machines in total:

- Kali Linux attack box
- Windows 10 workstation 1
- Windows 10 workstation 2
- Windows Server (Domain Controller)


### Skills Learned

* Methodical AD enumeration and asset discovery: mapping domain structure, hosts, and trusts.
* Focused service enumeration: SMB discovery and interrogation, SSH, HTTP, HTTPS, RPC, LDAP.
* Iterative attack workflow: initial enumeration, initial attacks, post-compromise enumeration, targeted follow-on attacks, persistence, and cleanup.
* Identifying and prioritizing attack paths: service accounts, exposed shares, weak ACLs.
* Credential harvesting techniques and defensive signal recognition.
* Practical pivoting from a compromised host using routing, port-forwarding, and proxy tools.
* Safe use of offensive tooling and telemetry generation to evaluate detection coverage.
* Building repeatable attack workflows and writing concise technical findings.

### Tools Used

| Phase | Tools |
|---|---|
| **Enumeration** | `nmap`, `smbclient`, **BloodHound**, `ldapdomaindump` |
| **Initial attacks** | `responder`, `ntlmrelayx`, `mitm6` |
| **Post-compromise attacks** | `crackmapexec`, `secretsdump.py`, `GetUserSPNs.py`, `psexec.py`, `msfconsole`, `xfreerdp`, `Mimikatz` (memory dumps) |
| **Persistence** | `secretsdump.py` (NTDS.dit extraction), `Mimikatz` (golden tickets, token theft) |
| **Pivoting** | `Ligolo-NG`, `proxychains` |

## Steps
Coming soon...
