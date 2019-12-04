# Meeting Notes - 2019-12-02

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Keisuke Kumada](https://github.com/kumada626)
- [Shota Yoshika](https://github.com/s-yoshika)
- Yahoo! JAPAN Team

## Agenda

From VMG:

- [Disk Optimzation](https://github.com/screwdriver-cd/screwdriver/issues/1830)
- [Parallel Fork](https://github.com/screwdriver-cd/screwdriver/issues/1710)
- [Build timeout not reliable](https://github.com/screwdriver-cd/screwdriver/issues/1710)
- [Updating dependencies](https://github.com/screwdriver-cd/screwdriver/issues/1722)

From Yahoo! JAPAN:

- [Template/Command list screen shows wrong VERSION](https://github.com/screwdriver-cd/screwdriver/issues/1723)
- [More details on notification email](https://github.com/screwdriver-cd/screwdriver/issues/1668)
- [SD Local](https://github.com/screwdriver-cd/screwdriver/issues/1853)
- [Duplicate PR comments](https://github.com/screwdriver-cd/screwdriver/issues/1858)
- [DB Size is growing](https://github.com/screwdriver-cd/screwdriver/issues/1865)

## Discussion Notes

For [Template/Command list screen shows wrong VERSION](https://github.com/screwdriver-cd/screwdriver/issues/1723) current solution introduces [a bug](https://github.com/screwdriver-cd/screwdriver/issues/1857) with trusted templates. VMG has pinned `datastore-sequelize` to an older version, until this is fixed.

For [Disk Optimzation](https://github.com/screwdriver-cd/screwdriver/issues/1830), discussed workflow, `executor-k8s` to be worked up on after `exececutor-k8s-vm` flow is addressed.

For [Performance issue of webhook](https://github.com/screwdriver-cd/screwdriver/issues/1468), [prs](https://github.com/screwdriver-cd/screwdriver/pull/1850) have been merged, Yahoo! JAPAN team will get performance numbers next time.

For [DB Size is growing](https://github.com/screwdriver-cd/screwdriver/issues/1865) VMG has data retention policies with is a Lambda process cleaning up builds older than 1 year. Current database table structure should be analyzed to do normalization.

[Notification email](https://github.com/screwdriver-cd/screwdriver/issues/1668) feature was completed a while back, issue was closed.

For [Build timeout not reliable](https://github.com/screwdriver-cd/screwdriver/issues/1710) & [Updating dependencies](https://github.com/screwdriver-cd/screwdriver/issues/1722) VMG will proritize them for Q1 2020.
