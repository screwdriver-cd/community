# Meeting Notes - 2020-01-13

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Keisuke Kumada](https://github.com/kumada626)
- [Shota Yoshika](https://github.com/s-yoshika)
- Yahoo! JAPAN Team

## Agenda

From Verizon Media:

1. New user on-board flow work to start. UI mocks available at [#1922](https://github.com/screwdriver-cd/screwdriver/issues/1922)
2. PR open with fixes to pipeline token permission. [#1847](https://github.com/screwdriver-cd/screwdriver/issues/1847)
3. Working on custom test result link in UI. [#1718](https://github.com/screwdriver-cd/screwdriver/issues/1718)

From Yahoo! JAPAN:

1. Pipeline API token feature. Step definition to follow.
2. [DB refactoring #1865](https://github.com/screwdriver-cd/screwdriver/issues/1865) - PRs need to be reviewed
3. Internal user reported issues
    1. https://github.com/screwdriver-cd/screwdriver/issues/1912
        1. Can't update API because blocked on https://github.com/screwdriver-cd/hyperctl-image/pull/32
    2. https://github.com/screwdriver-cd/screwdriver/issues/1915
    3. https://github.com/screwdriver-cd/screwdriver/issues/1920
4. Next call is National holiday in Japan - National Foundation Day.


## Discussion Notes

1. Jithin to merge `hyperctl-image` PR to unblock API for Yahoo! Japan.
1. Newly reported issues to be reviewed and prioritized.
1. No meeting next week due to national holiday in Japan. Will sync on Slack.
1. Verizon Media seeing increased latency for network calls to Store and API end points. Yahoo! JAPAN not seeing this problem.
