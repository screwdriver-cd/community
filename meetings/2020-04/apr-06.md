# Meeting Notes - 2020-04-06

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Pritam Paul](https://github.com/pritamstyz4ever)
- [Keisuke Kumada](https://github.com/kumada626)
- Yahoo! JAPAN Team

## Agenda

From Yahoo! JAPAN:

Completed Work

1. SD Local mode updates. [#1314](https://github.com/screwdriver-cd/screwdriver/issues/1314).
    1. README updated with usage details.
    1. Refactoring config file to support multiple clusters. [#2050](https://github.com/screwdriver-cd/screwdriver/issues/2050)
1. Default collection UI work.[#1383](https://github.com/screwdriver-cd/screwdriver/issues/1383).

Operational issues and feature requests
1. UI needs proper handling of error conditions. [#2049](https://github.com/screwdriver-cd/screwdriver/issues/2049)
1. Validation errors on `settings` and `annotations` are not handled properly. [#2051](https://github.com/screwdriver-cd/screwdriver/issues/2051), [#2053](https://github.com/screwdriver-cd/screwdriver/issues/2053)
1. Child pipelines are not getting webhook added as part of parent pipeline setup. [#2056](https://github.com/screwdriver-cd/screwdriver/issues/2056)
1. Need ability to copy build parameters from another event. This will reduce user repetition when starting pipeline. [#2057](https://github.com/screwdriver-cd/screwdriver/issues/2057)


From Verizon Media:

1. [queue-service](https://github.com/screwdriver-cd/queue-service) deployed in OSSD. Guide and blog post is available.
    1. Faced an issue where periodic bulds stopped working. PRs open to address the problems.
1. [Kata container](https://github.com/screwdriver-cd/screwdriver/issues/818) working on bootstrapping k8s nodes to use Kata.
1. UI PR is open for new on-boarding UI. [#539](https://github.com/screwdriver-cd/ui/pull/539)

Operational issues and feature requests
1. queue service release had to be rolled back due to these [issues](https://github.com/screwdriver-cd/screwdriver/issues/1951#issuecomment-609938807).
1. UI logs need to support clickable [links](https://github.com/screwdriver-cd/screwdriver/issues/1826).
1. There is a need to [relax blocked by](https://github.com/screwdriver-cd/screwdriver/issues/1712) for same job, especially for parameterised builds where each run is different. 

## Discussion Notes

1. Jithin to work with Yahoo Japan on onboarding to Screwdriver Tumblr for posting SD local blog post.
1. Data schema changes caused downtime since it contained an alter data type for existing column.
1. Adding `stable` container  tags must be done when a blog post for release is published. If it's missing then it should be brought up in Slack and fixed.
