# Ansible configuration

Ansible configuration(s) to configure Linux environment.

## Quick start

1. Install Ansible
1. Clone the repo
1. Run the command:

```
ansible-playbook fedora_default.yml --ask-become-pass
```

## Examples

### Example 1

Run the playbook with Desktop role enabled

```
ansible-playbook fedora_default.yml --extra-vars "enable_desktop=true" --ask-become-pass
```

### Example 2

Run the playbook with Gaming role enabled

```
ansible-playbook fedora_default.yml --extra-vars "enable_gaming=true" --ask-become-pass
```

### Example 3

Run the playbook with Desktop and Gaming role enabled

```
ansible-playbook fedora_default.yml --extra-vars "enable_desktop=true enable_gaming=true" --ask-become-pass
```

### Example 4

Run the playbook and get variable definitions from a file

```
ansible-playbook fedora_default.yml --extra-vars "@./variables/desktop_gaming.yml" --ask-become-pass
```
