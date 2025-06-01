<!-- Space: Projects -->
<!-- Parent: AnsibleRoleK3s -->
<!-- Title: Examples AnsibleRoleK3s -->
<!-- Label: Examples -->
<!-- Include: ./../disclaimer.md -->
<!-- Include: ac:toc -->

## Common

### Install Dependencies

```bash
task setup
```

## packages

To run this playbook with default settings, for install package like this:

generate file `requirements.yml`

```yaml
- name: hadenlabs.ansible-role-k3s
  src: git+https://github.com/hadenlabs/ansible-role-k3s
  version: /main
```

```yaml
- hosts: all

  roles:
    - role: hadenlabs.ansible-role-k3s
      become: true
      vars:
        ansible-role-k3s_owner: ubuntu
```
