# Meeting Notes - 2020-04-20

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Kevin Lu](https://github.com/klu909)
- [Lakshminarasimhan Parthasarathy](https://github.com/parthasl)
- [Keisuke Kumada](https://github.com/kumada626)
- [Yoshika Shota](https://github.com/s-yoshika)
- Yahoo! JAPAN Team

## Agenda

#### From Yahoo! JAPAN:

Completed Work

1. Bug fix for default collection UI.[PR #546](https://github.com/screwdriver-cd/ui/pull/546#pullrequestreview-391019455).
1. Bug fix for chain PR when restarting build.[#2029](https://github.com/screwdriver-cd/screwdriver/issues/2029).
1. Bug fix for branch filtering triggering on tags. [#2067](https://github.com/screwdriver-cd/screwdriver/issues/2067)
1. Bug fix for git cloning branches with `&` in name. [#2059](https://github.com/screwdriver-cd/screwdriver/issues/2059) 
1. Performance fix when deleting pipeline. [PR #445](https://github.com/screwdriver-cd/models/pull/445)

Work In Progress 
1. New feature to disable build cache for a job. [#1748](https://github.com/screwdriver-cd/screwdriver/issues/1748)
1. SD Local mode updates. [#1314](https://github.com/screwdriver-cd/screwdriver/issues/1314).
    1. Refactoring config file to support multiple clusters. [#2050](https://github.com/screwdriver-cd/screwdriver/issues/2050) in progress.
    1. Fix order of init step logs. [PR #340](https://github.com/screwdriver-cd/launcher/pull/340)

Operational issues and feature requests
1. UI does not display error message when sync webhook fails. [#2074](https://github.com/screwdriver-cd/screwdriver/issues/2074)


#### From Verizon Media:

Completed Work
1. Bug fixes for `queue-service` stability. [PR #15](https://github.com/screwdriver-cd/queue-service/pull/15)
1. Bug fix for `queue-service` and worker to automatically reconnect to queue. [#2052](https://github.com/screwdriver-cd/screwdriver/issues/2052)
1. Bug fix for `join` workflow. [#2070](https://github.com/screwdriver-cd/screwdriver/issues/2070)
1. Feature work for Kata container. [#818](https://github.com/screwdriver-cd/screwdriver/issues/818)


Work In Progress 
1. New on-boarding UI. PRs open to auto-create pull requests.  [#1922](https://github.com/screwdriver-cd/screwdriver/issues/1922)
1. Aggregate view with job list UI. [#1967](https://github.com/screwdriver-cd/screwdriver/issues/1967)


Operational issues and feature requests
1. Join build creation has a race condition bug which an result in multiple builds for same join job. [#2071](https://github.com/screwdriver-cd/screwdriver/issues/2071)

## Discussion Notes

1. Yahoo! Japan team is testing `queue-service` and fixed a performance issue related to it. Planning to push it to production soon.
1. Verizon Media is already running `queue-service` in production and rolled out further fixes to stabilize it. 
1. Created [UX 2.0](https://github.com/screwdriver-cd/screwdriver/milestone/1) milestone to track next gen UI work for Screwdriver.
