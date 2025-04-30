# AAP Configuration Demos

## Included content/ Directory Structure

The directory structure follows best practices recommended by the Ansible
community. Feel free to customize this template according to your specific
project requirements.

```text
 ansible-project/
 |── .devcontainer/
 |    └── docker/
 |        └── devcontainer.json
 |    └── podman/
 |        └── devcontainer.json
 |    └── devcontainer.json
 |── .github/
 |    └── workflows/
 |        └── tests.yml
 |    └── ansible-code-bot.yml
 |── .vscode/
 |    └── extensions.json
 |── collections/
 |   └── requirements.yml
 |   └── ansible_collections/
 |       └── project_org/
 |           └── project_repo/
 |               └── README.md
 |               └── roles/sample_role/
 |                         └── README.md
 |                         └── tasks/main.yml
 |── inventory/
 |   └── groups_vars/
 |   └── host_vars/
 |   └── hosts.yml
 |── ansible-navigator.yml
 |── ansible.cfg
 |── devfile.yaml
 |── linux_playbook.yml
 |── network_playbook.yml
 |── README.md
 |── site.yml
```

## AAP 2.4 Collection requirements

To use the AAP 2.4 playbooks the following collections are needed.

```yaml
  galaxy:
    collections:
      - name: ansible.controller
        version: ">=4.5.0,<4.6.0"
      - name: infra.controller_configuration
      - name: infra.aap_utilities
```

## AAP 2.5 Collection requirements

To use the AAP 2.4 playbooks the following collections are needed.

```yaml
  galaxy:
    collections:
      - name: ansible.controller
        version: ">=4.6.0"
      - name: infra.aap_configuration
      - name: infra.aap_utilities
```

## Compatible with Ansible-lint

Tested with ansible-lint >=24.2.0 releases and the current development version
of ansible-core.
