# ansible-ssh-on-drugs

Ansible role that secures the SSH daemon of any remote Debian server.

## Examples

``inventory``

        [all]
        remote.server.com

``playbook.yml``

        ---
        hosts: all
        remote_user: foo
        sudo: yes
        roles: {role: "ansible-ssh-on-drugs"}

Invoke playbook

        ansible-playbook -i inventory playbook.yml
