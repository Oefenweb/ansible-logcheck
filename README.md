## logcheck

[![Build Status](https://travis-ci.org/Oefenweb/ansible-logcheck.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-logcheck) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-logcheck-blue.svg)](https://galaxy.ansible.com/tersmitten/logcheck)

Set up logcheck in Debian-like systems.

#### Requirements

None

#### Variables

* `logcheck_install`: [default: `[syslog-summary]`]: Additional packages to install (e.g. `syslog-summary`)
* `logcheck_reportlevel`: [default: `server`]: Controls the level of filtering
* `logcheck_sendmailto`: [default: `root`]: Controls the address mail goes to
* `logcheck_logfiles`: [default: `[/var/log/{syslog,auth.log,mail.log,kern.log]`]: Log files to check
* `logcheck_custom_ignores`: [default: `[]`]: Additional rules for lines to ignore
* `logcheck_sortuniq`: [default: `false`]: Controls whether `sort -u` is used on log entries
* `logcheck_rulesdir`: [optional]: Controls the base directory for rules file location, this must be an absolute path
* `logcheck_manage_cron_d`: [default: `true`]: Whether or not to manage `/etc/cron.d/logcheck`
* `logcheck_cron`: [default: `@daily`]: cron.d timestamp when to execute logcheck

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
