## logcheck [![Build Status](https://travis-ci.org/Oefenweb/ansible-logcheck.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-logcheck)

Set up logcheck in Debian-like systems.

#### Requirements

None

#### Variables

* `logcheck_install`: [default: `[logcheck, syslog-summary]`]:
* `logcheck_reportlevel`: [default: `server`]:
* `logcheck_sendmailto`: [default: `root`]:
* `logcheck_syslogsummary`: [default: `true`]:
* `logcheck_logfiles`: [default: `[/var/log/{syslog,auth.log,mail.log,kern.log]`]:

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
