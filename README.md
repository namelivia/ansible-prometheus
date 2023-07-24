# Prometheus Ansible role [![Ansible Lint](https://github.com/namelivia/ansible-prometheus/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/namelivia/ansible-prometheus/actions/workflows/ansible-lint.yml)

The project depends on the collection `community.docker` but apparently this [cannot be listed as a dependency](https://github.com/ansible/ansible/issues/62847) so make sure you add it to your `requirements.yml` file like:

```yml
---

collections:
  - community.docker

roles:
  - src: https://github.com/namelivia/ansible-prometheus
```

 - `loki_url` Loki endpoint to send logs.
 - `host_port` Port to be mapped in the host machine.
