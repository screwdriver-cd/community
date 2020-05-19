# Meeting Notes - 2020-05-18

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Lakshminarasimhan Parthasarathy](https://github.com/parthasl)
- [Keisuke Kumada](https://github.com/kumada626)
- [Yoshika Shota](https://github.com/s-yoshika)
- [Supratik Das](https://github.com/supra08)
- Yahoo! JAPAN Team

## Agenda

#### From Yahoo! JAPAN:

Completed Work

1. Ability disable build cache for a job. [#1748](https://github.com/screwdriver-cd/screwdriver/issues/1748)
1. Fix for webhook not being added for child pipeline [#2056](https://github.com/screwdriver-cd/screwdriver/issues/2056)

Work In Progress 
1. Logging for capturing template usage stats. [PR-451](https://github.com/screwdriver-cd/models/pull/451)
1. SD Local mode updates. [#1314](https://github.com/screwdriver-cd/screwdriver/issues/1314).
    1. Refactoring config file changes complete. [#2050](https://github.com/screwdriver-cd/screwdriver/issues/2050)
    1. Working on blog post.

Operational issues and feature requests
1. Duplicate builds since GHE upgrade. [#2086](https://github.com/screwdriver-cd/screwdriver/issues/2086)
1. Piping of sd commands results in error. [#2090](https://github.com/screwdriver-cd/screwdriver/issues/2090)
1. Step order is broken in certain DB setups. [#2089](https://github.com/screwdriver-cd/screwdriver/issues/2089)


#### From Verizon Media:

Completed Work
1. Randomize build exectutor selection to shift build traffic dynamically to `Kata` nodes. [#2083](https://github.com/screwdriver-cd/screwdriver/issues/2083)
1. Fix for restarted jobs to find conext across all linked events. [#1785](https://github.com/screwdriver-cd/screwdriver/issues/1785)


Work In Progress 
1. New on-boarding UI. PRs open to auto-create pull requests.  [#1922](https://github.com/screwdriver-cd/screwdriver/issues/1922)
1. Aggregate view with job list UI. [#1967](https://github.com/screwdriver-cd/screwdriver/issues/1967)
    1. All pull requests have been merged. Waiting on review from design team and few more [changes](https://github.com/screwdriver-cd/screwdriver/issues/1967#issuecomment-630981995).


Operational issues and feature requests
1. GHE SSHCA feature is breaking webhook signature validation. [#2017](https://github.com/screwdriver-cd/screwdriver/issues/1785)


#### From Supratik (GSoC):

Work in Progress
1. Validating `settings` in `screwdriver.yaml`. [#1574](https://github.com/screwdriver-cd/screwdriver/issues/1574)
1. Generate and use deploy keys. [#1079](https://github.com/screwdriver-cd/screwdriver/issues/1574)

## Discussion Notes

1. Related to step order issue, Lakshmi pointed out that using `GSLB` in DB might cause duplicate build id's in different databases. Yahoo! Japan team to verify this.
1. Yahoo! Japan team is testing `remote-join` and plan to make it available to users.
1. Verizon Media team is in the process of operationalizing `Kata` containers in internal build clusters.
1. Supratik is working with Screwdriver as part of [GSoC](https://summerofcode.withgoogle.com/projects/#6332388868620288). Welcome onboard.
