# Ansible role: OpenShift Origin on Fedora

Ensures that OpenShift is installed and running as a systemd service. Also installs `oc` and `oadm` clients.

## Compatibility

This playbook has been tested against Fedora 25.

## Installation 

    ansible-galaxy install hekonsek.openshift,0.0

## Variables

- `project_name` - Kubernetes project name to use. Default is `default`.

## Example playbook

    - hosts: localhost
      remote_user: root
      roles:
        - { role: "hekonsek.openshift,0.0" }

## License

Apache 2.0
