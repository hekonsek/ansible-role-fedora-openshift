# Ansible role: OpenShift Origin on Fedora

Ensures that: 
- OpenShift is installed and running as a systemd service
- `oc` and `oadm` clients are installed
- integrated Docker registry is started and exposed as service to the outside world 

## Compatibility

This playbook has been tested against Fedora 26.

## Installation 

    ansible-galaxy install hekonsek.fedora-openshift,0.5

## Variables

- `project_name` - Kubernetes project name to use. Default value is `default`.
- `router_host` - host name used by router to expose services to the outside world. Default value is `router.default.svc.cluster.local`.

## Example playbook

    - hosts: localhost
      remote_user: root
      roles:
        - { role: hekonsek.fedora-openshift,0.5 }

## License

Apache 2.0
