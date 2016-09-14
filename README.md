# Ansible Logstash Role

## What it does
Installs java, logstash and installs configs

## Usage
Install in roles and call from playbook with:

```
- hosts: logstash_servers
  roles:
   - {
     role: logstash
    }
```

## Notes
Add as many logstash configs as you need in files/ and refrence them in tasks/main.yml

iptables task will insert a rule to allow ingress for external logstash inputs
