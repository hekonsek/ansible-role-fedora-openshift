# Ansible role: OpenShift Origin on Fedora

Ensures that: 
- OpenShift is installed and running as a systemd service
- `oc` and `oadm` clients are installed
- integrated Docker registry is started and exposed as service to the outside world 

## Compatibility

This playbook has been tested against Fedora 25.

## Installation 

    ansible-galaxy install hekonsek.fedora-openshift,0.1

## Variables

- `project_name` - Kubernetes project name to use. Default is `default`.

## Example playbook

    - hosts: localhost
      remote_user: root
      roles:
        - { role: hekonsek.fedora-openshift,0.1 }

## License

Apache 2.0
