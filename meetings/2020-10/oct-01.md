# Meeting Notes - 2020-10-01

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Tiffany K](https://github.com/tkyi)
- [Renaud Lepage](https://github.com/renaud-vmg)
- [Keisuke Kumada](https://github.com/kumada626)
- Yahoo! JAPAN Team

## Agenda

### From Yahoo! JAPAN:

#### Completed Work

1. Fix noisy github logs [PR#179](https://github.com/screwdriver-cd/scm-github/pull/179)
1. Enable Kata runtime with configuration in queue service so that kata can be used without buildcluster worker. [PR#22](https://github.com/screwdriver-cd/queue-service/pull/22#pullrequestreview-491210768)

#### Work In Progress 

1. Display Pipeline Description. [#2007](https://github.com/screwdriver-cd/screwdriver/issues/2007)
   1. Feature work done. One issue remaining wrt UI. [#2235](https://github.com/screwdriver-cd/screwdriver/issues/2235)

#### New Issues

1. Templates page is broken with latest sequalize version. [#2212](https://github.com/screwdriver-cd/screwdriver/issues/2212)
1. Performance issue with new API. [#2216](https://github.com/screwdriver-cd/screwdriver/issues/2216)

### From Verizon Media:

#### Completed Work

1. Fix for performance issue wrt API after hapi.js v20 upgrade. [#2216](https://github.com/screwdriver-cd/screwdriver/issues/2216)
1. New performance test suite for Screwdriver API. [#2233](https://github.com/screwdriver-cd/screwdriver/issues/2233)


#### Work In Progress 

1. Support large build step logs. [#2068](https://github.com/screwdriver-cd/screwdriver/issues/2068)
1. Build metrics - Display Pipeline downtime information. [#2199](https://github.com/screwdriver-cd/screwdriver/issues/2199)
1. Build steps are not in order. [#2232](https://github.com/screwdriver-cd/screwdriver/issues/2232)
   1. Likely an issue with build node. Time in build k8s pod drifted. Have a PR to make sure that UI displays steps in order.

#### Operational issues and feature requests
1. Limit number of parallel builds in a pipeline. [#2225](https://github.com/screwdriver-cd/screwdriver/issues/2225)
   1. We had an issue where a single pipeine took down build cluster by running over 100 parallel builds using TURBO resources.
1. Build in Bare metal nodes using executor-ssh [#2224](https://github.com/screwdriver-cd/screwdriver/issues/2224)
   1. There is a need for building on bare metal for OS images, since containers can't satisfy the build requireemnts. 
1. UX for builds in `CREATED` status is confusing. [#2225](https://github.com/screwdriver-cd/screwdriver/issues/2225)
1. Source Paths exclusions doesn't support blanket paths. [#1044](https://github.com/screwdriver-cd/screwdriver/issues/1044#issuecomment-702462653)
1. Enhancement to Secrets in PR builds so that they can be safely exposed in PRs for writers. [#2221](https://github.com/screwdriver-cd/screwdriver/issues/2221)

### Discussion Notes

1. Performance fixes were verified using the new performance test suite using `artillery`
1. VZM moved to blue-green deployment model using Kubernetes Canary ingress flow.
1. cdCon conference registration is now free. Screwdriver has [3 talks](https://blog.screwdriver.cd/post/630726409431760896/explore-screwdriver-at-cdcon-2020). 
1. No meetup next week since we skipped a week due to Google Meet outage. Next meeting will be on October 22nd.

