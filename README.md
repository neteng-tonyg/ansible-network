# ansible-network

.
├── ansible.cfg            # Core Ansible configuration
├── inventories/           # Environment-specific inventory data
│   ├── production/
│   │   ├── group_vars/    # Variables for all devices (e.g., DNS, NTP)
│   │   ├── host_vars/     # Device-specific data (e.g., IPs, Hostnames)
│   │   └── hosts          # Inventory file defining device groups
│   └── staging/
│       ├── group_vars/
│       ├── host_vars/
│       └── hosts
├── playbooks/             # Main workflow files (e.g., build, backup, deploy)
│   ├── site.yml           # Master playbook that calls others
│   ├── config_backup.yml
│   └── deploy_vlan.yml
├── roles/                 # Reusable task logic (e.g., Cisco-IOS, Juniper-Junos)
│   ├── common/            # Baseline configs shared across vendors
│   └── interface_config/  # Task files, templates, and defaults
├── templates/             # Jinja2 templates for configuration generation
├── requirements.yml       # External collections/roles dependencies (e.g., cisco.ios)
└── group_vars/            # (Optional) Global variables for all environments
