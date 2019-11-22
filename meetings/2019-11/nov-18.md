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

## Discussion Notes

[Force Push](https://github.com/screwdriver-cd/data-schema/pull/360) API is done, and UI work is still in progress.

For [Disk Optimzation](https://github.com/screwdriver-cd/screwdriver/issues/1830), the YJapan team would like to see more diagrams and charts to help with understanding how the infrastructure was setup and how to take advantage of the disk cache.

For [Performance issue of webhook](https://github.com/screwdriver-cd/screwdriver/issues/1468), the YJapan team is taking a look into it.

K8s upgrade: screwdriver infra's k8s config is not up to date. see [issue 1846](https://github.com/screwdriver-cd/screwdriver/issues/1846) for more details.


Lack of documentations on which what token types are, i.e. `SD_UI_TOKEN`, `SD_API_TOKEN`, and `SD_STORE_TOKEN`. It would be nice to add more clearification to the guide or docs, see [issue 1848](https://github.com/screwdriver-cd/screwdriver/issues/1848), and more documentations on developing locally. 
