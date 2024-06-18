# Use Case 1 - Test with Firewall Rules

## Test cases

* Using SANS institute [Firewall checklist template](https://www.sans.org/media/score/checklists/FirewallChecklist.pdf) as reference.

### Case 1:

In the Firewall Checklist, there are port restrictions checklist which provides guidelines which ports should be blocked.
One rule about https port is `SSL (except to external TCP 443 web servers)` which mean we can allow 443 port for external webservers which intends to be exposed outside but internal webservers in secure network should not be exposed even if its https port.

**Question 1:**
Please check the below mentioned firewall rule is compliance with firewall checklist
"server: webserver, type: internal, destination ip: 6.7.8.9, destination port: 443, source ip: 0.0.0.0/0, Description: Allow 443 port in internal webserver from internet"
**Question 2:**
Please check the below mentioned firewall rule is compliance with firewall checklist
"server: webserver, type: external, destination ip: 6.7.8.9, destination port: 443, source ip: 0.0.0.0/0, Description: Allow 443 port in external webserver from internet"

**Answer:**

[attachment](attachment-1.png)
