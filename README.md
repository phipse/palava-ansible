## Requirements

### General
- ansible (prefer newer ansible versions which are python 3 compatible)

### Prometheus
- jmespath (deployer host)
- unzip (target host)

### Grafana
- jmespath (deployer host)

## Deployment Instructions

### Grafana
- `ansible-galaxy install cloudalchemy.grafana`
- `ansible-playbook -i environments/production/inventory.yml playbooks/install_grafana.yml`

### Prometheus
- `ansible-galaxy install cloudalchemy.prometheus`
- `ansible-playbook -i environments/production/inventory.yml playbooks/install_prometheus.yml`

### Signal tower
- Copy `ansible.cfg.example` to `ansible.cfg`
- `ansible-playbook -i environments/production/inventory.yml playbooks/install_signaltower.yml`

### Palava Web
- `ansible-galaxy install community.general` (node)
- `ansible-playbook -i environments/production/inventory.yml playbooks/install_palava_web.yml`