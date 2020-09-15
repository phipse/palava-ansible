## Requirements

- ansible (prefer newer ansible versions which are python 3 compatible)

## Deployment Instructions

- Copy `ansible.cfg.example` to `ansible.cfg`
- `ansible-playbook -i environments/production/inventory.yml playbooks/install_signaltower.yml`
