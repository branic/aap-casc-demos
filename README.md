# AAP Configuration Demos

These are basic playbooks to installand configure AAP for demonstation purposes.

The content is provided *as-is*.

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
