## logcheck

[![Build Status](https://travis-ci.org/Oefenweb/ansible-logcheck.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-logcheck) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-logcheck-blue.svg)](https://galaxy.ansible.com/list#/roles/1417)

Set up logcheck in Debian-like systems.

#### Requirements

None

#### Variables

* `logcheck_install`: [default: `[logcheck, syslog-summary]`]: Packages to install
* `logcheck_reportlevel`: [default: `server`]: Controls the level of filtering
* `logcheck_sendmailto`: [default: `root`]: Controls the address mail goes to
* `logcheck_logfiles`: [default: `[/var/log/{syslog,auth.log,mail.log,kern.log]`]: Log files to check
* `logcheck_custom_ignores`: [default: `[]`]: Additional rules for lines to ignore
* `logcheck_rulesdir`: [default: undefined (default of logcheck which is `/etc/logcheck/`)]: Change the directory where logcheck will look for it’s rules.

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
    - logcheck
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-logcheck/issues)!
