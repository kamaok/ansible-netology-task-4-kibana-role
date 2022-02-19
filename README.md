Kibana role
=========

Роль для установки kibana на хостах с ОС: CentOS, RHEL.

Requirements
------------

Поддерживаются только ОС семейств EL.

Role Variables
--------------

| Variable name | Default | Description |
|-----------------------|----------|-------------------------|
| elk_stack_version | "7.14.0" | Параметр, который определяет какой версии kibana будет установлен |
| kibana_server_port | "5601" | Порт,на котором будет слушать запросы Kibana
| kibana_server_host | "0.0.0.0" | IP-адрес,на котором будет слушать запросы Kibana
| kibana_server_name | "My Kibana" | Имя сервера Kibana


Example Playbook
----------------
```bash
  - hosts: kibana
    become: true
    roles:
      - { role: kibana-role, tags: kibana }
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
