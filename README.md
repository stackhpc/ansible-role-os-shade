OpenStack Shade
===============

This role can be used to install the python package `shade`.

Requirements
------------

None

Role Variables
--------------

`os_shade_venv` is a path to a directory in which to create a virtualenv.

`os_shade_install_epel`: Whether to install EPEL repository package.

`os_shade_install_package_dependencies`: Whether to install package
dependencies.

`os_shade_version`: Version of shade to install, or latest if empty.

Dependencies
------------

None

Example Playbook
----------------

The following playbook installs shade and its dependencies in a virtualenv.

    ---
    - name: Ensure shade is installed
      hosts: localhost
      roles:
        - role: stackhpc.os-shade
          os_shade_venv: "~/os-shade-venv"

Author Information
------------------

- Mark Goddard (<mark@stackhpc.com>)
