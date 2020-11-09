# Meeting Notes - 2020-11-05

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Keisuke Kumada](https://github.com/kumada626)
- [Hiroki Takatsuka](https://github.com/tk3fftk)
- Mansoor Chengat
- Yahoo! JAPAN Team

## Agenda

### From Yahoo! JAPAN:

#### Completed Work

1. Shared steps can be merged into a job’s steps when using Templates. [#2174](https://github.com/screwdriver-cd/screwdriver/issues/2174)
1. `sd-local` interactive mode. [#2238](https://github.com/screwdriver-cd/screwdriver/issues/2238#issuecomment-708948452)
1. Incorrect `cache` config should not break pipelines. [#2211](https://github.com/screwdriver-cd/screwdriver/issues/2211)

#### Work In Progress 

1. Build cluster is getting enabled even when configuration is disabled. [#2240](https://github.com/screwdriver-cd/screwdriver/issues/2240)

#### New Issues

1. Display event label in build detail page. [#2261](https://github.com/screwdriver-cd/screwdriver/issues/2261)
1. Ability to sync periodic job's configuration in queue. [#2264](https://github.com/screwdriver-cd/screwdriver/issues/2264)
1. Homebrew support for `sd-local`. [#2270](https://github.com/screwdriver-cd/screwdriver/issues/2270)

### From Verizon Media:

#### Completed Work

1. UI permalink for jobs view. [#PR621](https://github.com/screwdriver-cd/ui/pull/621)
1. UI fix for invalid workflow graph when enabling triggers. [#PR626](https://github.com/screwdriver-cd/ui/pull/626)
1. UI fix for flickering workflow graph by fixing job display order. [#PR623](https://github.com/screwdriver-cd/ui/pull/623)

#### Work In Progress 

1. Build metrics - Display Pipeline downtime information. [#2199](https://github.com/screwdriver-cd/screwdriver/issues/2199)
1. Running teardown steps on aborted builds. [#1125](https://github.com/screwdriver-cd/screwdriver/issues/1125)
1. Collections end point performance fix. [#2267](https://github.com/screwdriver-cd/screwdriver/issues/2267)


#### Operational issues and feature requests

 
### Discussion Notes

1. Open Source Screwdriver was down because of an issue with underlying Kubernetes cluster when new nodes were added. KOPS went out of state and we had to rebuild the entire cluster.
1. Verizon Media Open source projects are onboarding to Screwdriver from Travis CI.


