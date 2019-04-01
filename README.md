# ansible-xfsprogs

Ensures xfsprogs is installed on the system.

## Requirements

No special pre-requisites.

## Role Variables
- Name: apt_cache_valid_time
  Default: 21600
  Description: Run apt-get update if cache is older

## Dependencies

None.

## Example Playbook
```yml
---    
- hosts: servers
  roles:
    - { role: xfsprogs }
```
or 
``` yml
- hosts: servers
  roles:
    - { role: xfsprogs, apt_cache_valid_time: 3600 }
```
