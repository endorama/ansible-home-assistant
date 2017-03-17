Ansible role: home-assistant
=========

Install [Home Assistant][home-assistant], using the [virtualenv installation][venv-install].

Is compatible with standards defined by [debops][debops].

[home-assistant]: https://home-assistant.io/
[venv-install]: https://home-assistant.io/docs/installation/virtualenv/
[debops]: https://debops.org/

Requirements
------------

None

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

- `homeassistant__config_dir`: The location of the config directory  
  *default:* "/srv/home-assistant-config"  
- `homeassistant__user`: The user used for install and run  
  *default:* "ha"  
- `homeassistant__port`: The home assistant webserver listening port  
  *default:* 8123  
- `homeassistant__version: `: The specific version to install or 'latest'  
  *default:* 'latest'  

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: endorama.home-assistant }

License
-------

MIT

Author Information
------------------

[@endorama](https://github.com/endorama)
