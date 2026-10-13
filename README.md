# Nicholas White

**IT professional moving into GRC and security operations** · New York City area

10+ years in NYC government operations and HIPAA-regulated environments, now building and
documenting security labs that treat evidence the way an auditor would: test whether a control
actually works, record what was and wasn't verified, and keep risks open until they are really
closed.

CompTIA A+ · Network+ · Security+ · ITIL 4 Foundation · Microsoft AZ-900 · B.S. Cloud and Network
Engineering (WGU, in progress)

## Home lab portfolio

| Lab | What it shows | Highlights |
| --- | --- | --- |
| [home-lab-foundation](https://github.com/Nlwhite20/home-lab-foundation) | Lab scope, safety rules and network plan | Authorized-scope rules and an isolated UTM lab design |
| [noc-monitoring-lab](https://github.com/Nlwhite20/noc-monitoring-lab) | Monitoring and alerting: Prometheus, Grafana, Uptime Kuma, Discord | Controlled outage tests with scripted evidence; found an alert rule bypassing its notification policy; published a dated correction when a VM clock error affected earlier timestamps |
| [wazuh-siem-lab](https://github.com/Nlwhite20/wazuh-siem-lab) | Wazuh SIEM deployment, configuration audit, alert triage | Found and fixed a dashboard exposure that contradicted the documented baseline (mapped to NIST CM-2/3/6, CA-7); first investigation correlated 7 IDS alerts to SIEM records on four fields and logged an agent queue overflow as an open risk |
| [network-security-lab](https://github.com/Nlwhite20/network-security-lab) | Suricata IDS feeding Wazuh; scoped exposure audit | Proved the same alert end to end (matching flow ID); scoped Nmap audit found no undocumented open ports; documented that default rules did not flag the scan as a port scan |
| [vulnerability-management-lab](https://github.com/Nlwhite20/vulnerability-management-lab) | One vulnerability assessment cycle on one Linux host | 10,743 findings traced to one kernel CVE set counted across three kernels; removed an unused kernel (findings to 7,095, as predicted); documented exceptions with pending owner decisions. Not all vulnerabilities are remediated |
| [backup-restore-lab](https://github.com/Nlwhite20/backup-restore-lab) | Encrypted, scheduled backups with tested restores (restic, append-only rest-server) | Restore tests with hash verification (folder restored in under 1 s against a 30-minute target); a client's attempt to delete a backup was refused by the append-only server; missed-backup detection; verified third copy. Not off-site, and retention pruning and alert notification are still open |

## How I work

- **Evidence over claims:** every lab separates what was verified from what was assumed, and
  marks missing evidence instead of filling the gap.
- **Change control:** scope and approvals written before changes, and a build log in each lab.
  Changes found without a record are documented as findings (for example, wazuh-siem-lab Finding 001).
- **AI collaboration, human validation:** I use Claude as an assistant. The five lab repos each
  have an "AI Collaboration and Human Validation" section recording where its suggestions were
  corrected.

## Contact

[LinkedIn](https://www.linkedin.com/in/nicholas-white-980190262)
