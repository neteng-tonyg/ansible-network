## This template set is designed for A/P HA in Azure.  The following are created:

## Temporary suggestion for folder structure of an Ansible playbook

network-automation-project/
│
├── README.md
├── LICENSE
├── .gitignore
├── ansible.cfg
├── requirements.yml
│
├── inventory/
│   ├── hosts.yml
│   ├── group_vars/
│   │   ├── all.yml
│   │   ├── cisco.yml
│   │   ├── juniper.yml
│   │   └── firewalls.yml
│   │
│   └── host_vars/
│       ├── switch1.yml
│       └── router1.yml
│
├── playbooks/
│   ├── site.yml
│   ├── backup_configs.yml
│   ├── vlan_provision.yml
│   ├── compliance_check.yml
│   └── firewall_rules.yml
│
├── roles/
│   ├── base_config/
│   │   ├── tasks/
│   │   │   └── main.yml
│   │   ├── templates/
│   │   ├── defaults/
│   │   │   └── main.yml
│   │   └── meta/
│   │
│   ├── vlan_management/
│   │   ├── tasks/
│   │   ├── templates/
│   │   └── defaults/
│   │
│   ├── config_backup/
│   │   ├── tasks/
│   │   └── templates/
│   │
│   └── compliance/
│       ├── tasks/
│       └── templates/
│
├── templates/
│   ├── cisco_interface.j2
│   ├── vlan_config.j2
│   └── syslog_config.j2
│
├── library/              # optional custom modules
│   └── network_utils.py
│
├── module_utils/         # optional helpers
│
├── filter_plugins/       # Jinja2 extensions
│
├── scripts/
│   ├── run_playbook.sh
│   └── inventory_sync.py
│
├── docs/
│   ├── architecture.md
│   ├── usage.md
│   ├── topology.png
│   └── troubleshooting.md
│
├── tests/
│   ├── test_inventory.yml
│   ├── test_connectivity.yml
│   └── lint.sh
│
└── .github/
    └── workflows/
        └── ansible-lint.yml
