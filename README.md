## Requirements

### General
- ansible (prefer newer ansible versions which are python 3 compatible)

### Prometheus
- jmespath (installing host)
- unzip (target host)

## Deployment Instructions

### Prometheus
- `ansible-galaxy install cloudalchemy.prometheus`
- `ansible-playbook -i environments/production/inventory.yml playbooks/install_prometheus.yml`

### Signal tower
- Copy `ansible.cfg.example` to `ansible.cfg`
- `ansible-playbook -i environments/production/inventory.yml playbooks/install_signaltower.yml`
