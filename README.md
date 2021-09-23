ASBRL-NODE-EXPORTER
=========

Deploy an official Node Exporter (Linux) as a Docker container.

Requirements
------------

- Need to be Docker engine installed.

Role Variables
--------------

- CONTAINER_NAME: 'node-exporter'
- DOCKER_NETWORK_MODE: 'host'
- CONTAINER_STATE: 'started'
- IMAGE: 'prom/node-exporter'
- BUILD: 'v1.2.2'
- DOCKER_LOG_DRIVER: "json-file"
- DOCKER_LOG_OPTIONS: '{"max-size":"64m","max-file": "3"}'

Dependencies
------------

None

Example Playbook
----------------

    - name: Deploy Node Exporter
      include_role:
        name: asbrl-node-exporter
      tags:
        - asbrl-node-exporter

License
-------

BSD

Author Information
------------------

Francisco Chantada
