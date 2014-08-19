## logcheck [![Build Status](https://travis-ci.org/Oefenweb/ansible-logcheck.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-logcheck)

Set up logcheck in Debian-like systems.

#### Requirements

None

#### Variables

* `logcheck_install`: [default: `[logcheck, syslog-summary]`]: Packages to install
* `logcheck_reportlevel`: [default: `server`]: Controls the level of filtering
* `logcheck_sendmailto`: [default: `root`]: Controls the address mail goes to
* `logcheck_syslogsummary`: [default: `true`]: Controls if syslog-summary is run over each section
* `logcheck_logfiles`: [default: `[/var/log/{syslog,auth.log,mail.log,kern.log]`]: Log files to check

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
