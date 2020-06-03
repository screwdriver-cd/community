# Meeting Notes - 2020-05-18

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Keisuke Kumada](https://github.com/kumada626)
- [Yoshika Shota](https://github.com/s-yoshika)
- Yahoo! JAPAN Team

## Agenda

#### From Yahoo! JAPAN:

Completed Work

1. Support exclusions in Source Paths. [#1044](https://github.com/screwdriver-cd/screwdriver/issues/1044)
1. Fix for chainPR and remote join [PR #398](https://github.com/screwdriver-cd/data-schema/pull/398)
1. Fix for tag/release triggers being dependent on changedFiles. [PR #454](https://github.com/screwdriver-cd/models/pull/454)

Work In Progress 
1. SD Local mode updates. [#1314](https://github.com/screwdriver-cd/screwdriver/issues/1314).
    1. Blog post pending review.

Operational issues and feature requests
1. First PR job is not running without an empty screwdriver.yaml  [#2094](https://github.com/screwdriver-cd/screwdriver/issues/2094)
1. Queued notifications are sent twice [#2096](https://github.com/screwdriver-cd/screwdriver/issues/2096)
1. Raw queries are broken with MySQL 5.7 [#2100](https://github.com/screwdriver-cd/screwdriver/issues/2100)


#### From Verizon Media:

Completed Work
1. Kata containers blog post is published. 
1. Aggregate view with job list UI. [#1967](https://github.com/screwdriver-cd/screwdriver/issues/1967)


Work In Progress 
1. New on-boarding UI. API now supports creating PR. [#1922](https://github.com/screwdriver-cd/screwdriver/issues/1922)
1. GHE SSHCA feature is breaking webhook signature validation. [#2017](https://github.com/screwdriver-cd/screwdriver/issues/1785)
1. Cache cleanup is broken with disk based cache. [#2087](https://github.com/screwdriver-cd/screwdriver/issues/2087)
1. Support relative path resolution in store-cli. [#2098](https://github.com/screwdriver-cd/screwdriver/issues/2098)
1. Builds are blocked by other builds which are already completed. [#2095](https://github.com/screwdriver-cd/screwdriver/issues/2095)


#### From Supratik (GSoC):

Work in Progress
1. Validating `settings` in `screwdriver.yaml`. [#1574](https://github.com/screwdriver-cd/screwdriver/issues/1574)
    1. Pull Requests are open.
1. Generate and use deploy keys. [#1079](https://github.com/screwdriver-cd/screwdriver/issues/1574)

## Discussion Notes

1. Yahoo! JAPAN to turn on Remote-Join feature in SD cluster.
1. Raw queries for aggregate view and restart build flow is blocking new API release for Yahoo! JAPAN. 
1. Exploring feasiblity of a webinar with Yahoo! JAPAN and Verizon Media team.
