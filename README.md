# scom-rhel8
Management packs for SCOM to support RHEL 8

SCOM 2016:
Prerequisites:
- All standard SCOM 2016 UNIX/Linux prerequisities apply including:
  - Firewall ports (https://docs.microsoft.com/en-us/system-center/scom/plan-security-config-firewall?view=sc-om-2016), namely ICMP ping, TCP port 22 (SSH) and TCP port 1270 from SCOM Management server to the UNIX/Linux server.
  - Configuration of SCOM UNIX/Linux accounts (https://kevinholman.com/2016/11/11/monitoring-unix-linux-with-opsmgr-2016/)
  - Local UNIX/Linux monitoring account creation including sudo configuration (https://social.technet.microsoft.com/wiki/contents/articles/7375.scom-configuring-sudo-elevation-for-unix-and-linux-monitoring.aspx#D)
- The latest System Center Management Pack for UNIX and Linux Operating Systems is required (https://www.microsoft.com/en-au/download/details.aspx?id=29696).

Installation:
- Download the Management Pack Bundle (.mpb) for your version of SCOM and import into SCOM via console.
- Wait for a short while after import completes (~5 - 10 mins) before discovering RHEL 8 hosts.
