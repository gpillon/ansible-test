# Molecule Test Suite for role test_wf
# Molecule Structure (Default test)

    .
    ├── Dockerfile.j2
    ├── INSTALL.rst
    ├── README.md
    ├── converge.yml
    ├── destroy.yml
    ├── molecule.yml
    ├── prepare.yml
    ├── test_data
    └── verify.yml

This structure was autogenerated by `molecule init role_name` command

## Molecule.yml

    ---
    dependency:
      name: galaxy
    driver:
      name: podman
    platforms:
      - name: test_wf
        dockerfile: Dockerfile
        image: fedora:34
        pre_built_image: true

    provisioner:
      name: ansible
      config_options:
        defaults:
          callbacks_enabled: ansible.posix.profile_tasks
      options:
        vvv: true
      lint:
        name: ansible-lint
        enabled: true

    scenario:
      name: default
      test_sequence:
        - create
        - prepare
        - converge
        - verify
        - destroy

### Testing Environment

Podman

### Testing Scenario

 default

### Testing Phases

  - create
  - prepare
  - converge
  - verify
  - destroy

### Molecule Test Command (for any requirements, please refer to requirements.txt)

    [user@localhost]# molecule test