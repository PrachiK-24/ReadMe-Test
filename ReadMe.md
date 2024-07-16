# Steps to Install zabbix Agent on AWS EC2
---
### Step 1: Install zabbix repository
```
wget https://repo.zabbix.com/zabbix/6.0/rhel/8/x86_64/zabbix-agent-6.0.1-1.el8.x86_64.rpm
```
```
sudo yum install ./zabbix-agent-6.0.1-1.el8.x86_64.rpm
```
### Step 2: Change ServerIP, ActiveServerIP and Hostname.
```
nano /etc/zabbix/zabbix_agentd.conf
```
### Step 3: Start zabbix-agent service
```
systemctl enable zabbix-agent.service --now
```

