# OpenShift Cluster on Equinix Metal

Using Ansible to deploy a OpenShift cluster (4.15+) on Equinix Metal

Features:
- Support for one (Single Node Openshift), three (Compact Cluster), and five or more (Standard) node configurations
- Leverages Agent-based installer
- Uses iPXE for RHCOS bootstrap

## Using venv

```
python -m venv env
env/bin/pip install ansible equinix_metal ansible_specdoc
```

## Getting Started

1. Get a Equinix Metal API key
1. Copy `secrets.yml.tpl` to `secrets.yml` and also configure `vars.yml`
1. Create a VLAN 100 network
1. Run `ansible-playbook playbook.yml`
