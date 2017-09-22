hxpro.dnsmasq
=============

Install dnsmasq

This role is under development, do not use in production.

Requirements
------------


Role Variables
--------------

    dnsmasq_zone:
      - name: example.com
        records:
          - name: www
            type: A
            value: 192.168.1.20
          - name: mx
            type: MX
            value: 192.168.1.21
          - name:
            type: TXT
            value: 'v=spf1 a mx ~all'
      - name: example.net
        records:
          - name: web
            type: A
            value: 192.168.1.20
          - name: mx
            type: MX
            value: 192.168.1.21

Dependencies
------------


Example Playbook
----------------

    - hosts: servers
      roles:
         - role: hxpro.dnsmasq

License
-------

WTFPL

Author Information
------------------

Matěj Koudelka <matej@hxpro.cz>
