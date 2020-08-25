# Meeting Notes - 2020-08-24

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Keisuke Kumada](https://github.com/kumada626)
- [Hiroki Takatsuka](https://github.com/tk3fftk)
- [Supratik Das](https://github.com/supra08)
- Yahoo! JAPAN Team

## Agenda

#### From Yahoo! JAPAN:

##### Completed Work

1. Sync webhook when Pipeline repo is updated [#1954](https://github.com/screwdriver-cd/screwdriver/issues/1954)

##### Work In Progress 

1. Display Pipeline Description. [#2007](https://github.com/screwdriver-cd/screwdriver/issues/2007)
   1. Will request Chas to review.
1. Functional tests for Remote-Join is working as expected locally. [PR #2166](https://github.com/screwdriver-cd/screwdriver/pull/2166)
   1. Need to debug in SD Beta environment.
1. Application Metrics is blocked on Hapi v19 work. [#2115](https://github.com/screwdriver-cd/screwdriver/issues/2115)

##### New Issues

1. Modify response code for pipeline with no admin. [#2189](https://github.com/screwdriver-cd/screwdriver/issues/2189)

#### From Verizon Media:

##### Completed Work

1. Pipeline creation for Github SCM will default to repository branch rather than being hardcoded to `master` branch. [#2185](https://github.com/screwdriver-cd/screwdriver/issues/2185)
1. Pull Request Checkout process has been changed to support Sonarqube PR analysis [Changes](https://github.com/screwdriver-cd/scm-github/compare/v10.3.1...v10.3.3#diff-168726dbe96b3ce427e7fedce31bb0bcL677)
    1. Rather than doing a `merge` into the checked out pipeline branch, PR is now a separate detached branch.
1. UI - Permalinks for job builds were broken. [#2184](https://github.com/screwdriver-cd/screwdriver/issues/2184)
1. UI - Pipeline list view scroll was not working for pipelines with large number of jobs. [#2181](https://github.com/screwdriver-cd/screwdriver/issues/2181)
1. Allow aborting builds with Pipeline Token. [PR#2191](https://github.com/screwdriver-cd/screwdriver/pull/2191)


##### Work In Progress 

1. Support large build step logs. [#2068](https://github.com/screwdriver-cd/screwdriver/issues/2068)
1. Hapi.js upgrades. [#1958](https://github.com/screwdriver-cd/screwdriver/issues/1958)
1. Enable direct link to event in events list [#1802](https://github.com/screwdriver-cd/screwdriver/issues/1802)


##### Operational issues and feature requests

1. Build periodically setting not getting reenabled if a job gets archived somehow. 
1. Setup SonarQull Pull Request Decoration automatically for new Sonar Projects.
1. Invalid trigger in `requires` breaks collection. [#2192](https://github.com/screwdriver-cd/screwdriver/issues/2192)

#### From GSoC Project:

##### Work in Progress

1. Notify SCM changes. [#1415](https://github.com/screwdriver-cd/screwdriver/issues/1415)
   1. Pull Requests open, pending review.
