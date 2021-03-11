https://github.com/isweluiz/ELK/blob/master/install-auditbeat.yml


```bash
[root@ansible-master playbook]# ansible-playbook install-audit.yml

PLAY [Install beat] *********************************************************************************************************************

TASK [Gathering Facts] ******************************************************************************************************************
ok: [host02]
ok: [host00]
ok: [host04]
ok: [host03]
ok: [host01]
ok: [host05]
ok: [host06]

TASK [copy audit] ***********************************************************************************************************************
ok: [host02]
changed: [host03]
changed: [host01]
changed: [host00]
changed: [host04]
changed: [host05]
changed: [host06]

TASK [install filebeat] *****************************************************************************************************************
ok: [host02]
changed: [host04]
changed: [host00]
changed: [host03]
changed: [host05]
changed: [host01]
changed: [host06]

TASK [copy configuration file] **********************************************************************************************************
changed: [host00]
changed: [host01]
changed: [host03]
ok: [host02]
changed: [host04]
changed: [host06]
changed: [host05]

TASK [Enable service] *******************************************************************************************************************
changed: [host00]
ok: [host02]
changed: [host04]
changed: [host01]
changed: [host03]
changed: [host05]
changed: [host06]

PLAY RECAP ******************************************************************************************************************************
host00                : ok=5    changed=4    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
host01                : ok=5    changed=4    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
host02                : ok=5    changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
host03                : ok=5    changed=4    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
host04                : ok=5    changed=4    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
host05                : ok=5    changed=4    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
host06                : ok=5    changed=4    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
```
