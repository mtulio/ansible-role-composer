# Ansible Role: Composer

Installs Composer, the PHP Dependency Manager, on any Linux or UNIX system.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `vars/main.yml`):

    composer_path: /usr/local/bin/composer

The path where composer will be installed and available to your system. Should be in your user's `$PATH` so you can run commands simply with `composer` instead of the full path.

## Dependencies

  - geerlingguy.php (Installs PHP).

## Example Playbook

    - hosts: servers
      roles:
        - { role: geerlingguy.composer }

After the playbook runs, `composer` will be placed in `/usr/local/bin/composer`, and will be accessible from normal system accounts.

## License

MIT / BSD

## Author Information

This role was created in 2014 by Jeff Geerling (@geerlingguy), author of Ansible for DevOps. You can find out more about the book at http://ansiblefordevops.com/, and learn about the author at http://jeffgeerling.com/.
