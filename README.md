# Ansible-Role: acr-ansible-mattermost-add-playbook

AIT-CyberRange: Adds a mattermost playbook to all teams. 


## Requirements

- Mattermost installation

## Role Variables

```yaml
mattermost_url: http://127.0.0.1:8065
mattermost_user: admin
mattermost_password: password
mattermost_playbook_json: incident_response_plan.json
```

## Example Playbook

```yaml
- hosts: localhost
  roles:
    - acr-ansible-mattermost-add-playbook
      vars:
        mattermost_playbook_json: "/path/to/local/playbook.json"
```

## License

GPL-3.0

## Author

- Lenhard Reuter