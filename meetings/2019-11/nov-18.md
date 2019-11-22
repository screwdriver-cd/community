# Meeting Notes - 2019-11-18

## Attendees

- [Alan Dong](https://github.com/adong)
- [Keisuke Kumada](https://github.com/kumada626)

## Agenda

From VMG:

- [Force Push](https://github.com/screwdriver-cd/screwdriver/issues/1675) update during [freezeWindow](https://docs.screwdriver.cd/user-guide/configuration/workflow.html) time
- [Disk Optimzation](https://github.com/screwdriver-cd/screwdriver/issues/1830)
- [Parallel Fork](https://github.com/screwdriver-cd/screwdriver/issues/1710)

From YJapan:

- [SD Local](https://github.com/screwdriver-cd/screwdriver/issues/1314)
- [Template/Command list screen shows wrong VERSION](https://github.com/screwdriver-cd/screwdriver/issues/1723)
- [Performance issue of webhook](https://github.com/screwdriver-cd/screwdriver/issues/1468)
- [feature request: Teardown Job](https://github.com/screwdriver-cd/screwdriver/issues/1834)
- [feature request: Pipeline token should be able to create Secrets](https://github.com/screwdriver-cd/screwdriver/issues/1847)

## Discussion Notes

[Force Push](https://github.com/screwdriver-cd/data-schema/pull/360) API is done, and UI work is still in progress.

For [Disk Optimzation](https://github.com/screwdriver-cd/screwdriver/issues/1830), the YJapan team would like to see more diagrams and charts to help with understanding how the infrastructure was setup and how to take advantage of the disk cache.

For [Performance issue of webhook](https://github.com/screwdriver-cd/screwdriver/issues/1468), the YJapan team is taking a look into it.

K8s upgrade: Screwdriver's infra K8s config is not up to date. See [issue 1846](https://github.com/screwdriver-cd/screwdriver/issues/1846) for more details.


There is a lack of documentation on token types (e.g. `User API Token`, and `Pipeline API Token`). It would be nice to add more clarification to the guide or docs, see [issue 1848](https://github.com/screwdriver-cd/screwdriver/issues/1848); also would like to see more documentation on developing locally.
