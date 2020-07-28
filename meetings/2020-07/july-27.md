# Meeting Notes - 2020-07-27

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Keisuke Kumada](https://github.com/kumada626)
- [Yoshika Shota](https://github.com/s-yoshika)
- [Hiroki Takatsuka](https://github.com/tk3fftk)
- [Supratik Das](https://github.com/supra08)
- Yahoo! JAPAN Team

## Agenda

#### From Yahoo! JAPAN:

Completed Work

1. sd-local support for long build logs. [PR#40](https://github.com/screwdriver-cd/sd-local/pull/40)

Work In Progress 

1. Updating browser tab favicon. [#1009](https://github.com/screwdriver-cd/screwdriver/issues/1009)
   1. Reviewing design from Chas. 
1. Drop-down values for Parameterized Builds. [#2092](https://github.com/screwdriver-cd/screwdriver/issues/2092)
   1.  Back-end work is complete . UI changes pending.
1. Functional test for remote-join feature. [PR#2159](https://github.com/screwdriver-cd/screwdriver/pull/2159)


Operational issues and feature requests

1. Remote Trigger is not working with Child Pipelines. [#2148](https://github.com/screwdriver-cd/screwdriver/issues/2148)

#### From Verizon Media:

Completed Work

1. UI fixes for Pipeline job-list view. [#2124](https://github.com/screwdriver-cd/screwdriver/issues/2124)

Work In Progress 

1. SonarQube Pull Request flow updates for supporting Enterprise Edition. [#2152](https://github.com/screwdriver-cd/screwdriver/issues/2152)
1. Support large build step logs. [#2068](https://github.com/screwdriver-cd/screwdriver/issues/2068)
1. Display namespace in Template drop down list. [#2140](https://github.com/screwdriver-cd/screwdriver/issues/2140)

Operational issues and feature requests

1. Template & Command Marketplace. [#2151](https://github.com/screwdriver-cd/screwdriver/issues/2151)
#### From GSoC Project:

Work in Progress

1. Notify SCM changes. [#1415](https://github.com/screwdriver-cd/screwdriver/issues/1415)

## Discussion Notes

1. Hapi.js has reversed EOL plans and will be maintained by a new Team. We should prioritize updating our dependencies. 
1. VZM faced more issues with Kata rollout. Will have to build a custom Kata kernel with all hardcoded tweaks. Will be opening an issue with details.
