# Meeting Notes - 2020-08-10

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Keisuke Kumada](https://github.com/kumada626)
- [Hiroki Takatsuka](https://github.com/tk3fftk)
- Yahoo! JAPAN Team

## Agenda

#### From Yahoo! JAPAN:

##### Completed Work

1. Should not use too common env PUSHGATEWAY_URL. [#2116](https://github.com/screwdriver-cd/screwdriver/issues/2116)
1. Remote trigger to child pipelines do not work. [#2148](https://github.com/screwdriver-cd/screwdriver/issues/2148)
1. Drop-down values in parameters. [#2092](https://github.com/screwdriver-cd/screwdriver/issues/2092)
    1. Thanks to [Alan](https://github.com/adong) for suggestions.
1. Validator does not recognize some annotations value. [#1684](https://github.com/screwdriver-cd/screwdriver/issues/1684)
    1. Upgraded Ember to 3.16 latest LTS.
1. Separated trigger functional tests into beta & prod. [PR#2166](https://github.com/screwdriver-cd/screwdriver/pull/2166)


##### Work In Progress 

1. Updating browser tab favicon. [#1009](https://github.com/screwdriver-cd/screwdriver/issues/1009)
   1. Awaiting icons from Chas. 
1. QUEUED notification is sent twice. [#2096](https://github.com/screwdriver-cd/screwdriver/issues/2096)
   1. Awaiting review from Jithin/Pritam 

#### From Verizon Media:

##### Completed Work

1. SonarQube Pull Request flow updates for supporting Enterprise Edition. [#2152](https://github.com/screwdriver-cd/screwdriver/issues/2152)
    1. Blog post pending
1. Display namespace in Template drop down list. [#2140](https://github.com/screwdriver-cd/screwdriver/issues/2140)

##### Work In Progress 

1. Support large build step logs. [#2068](https://github.com/screwdriver-cd/screwdriver/issues/2068)
1. Hapi.js upgrades. [#1958](https://github.com/screwdriver-cd/screwdriver/issues/1958)
1. Enable direct link to event in events list [#1802](https://github.com/screwdriver-cd/screwdriver/issues/1802)


##### Operational issues and feature requests

1. Upgrade octokit to v18. [#2173](https://github.com/screwdriver-cd/screwdriver/issues/2173)
1. Warn user if a build being restarted is not from the latest build [#2165](https://github.com/screwdriver-cd/screwdriver/issues/2165)

#### From GSoC Project:

##### Completed Work
1. Deploy Key Generation is turned on at [cd.screwdriver.cd](cd.screwdriver.cd/)

##### Work in Progress

1. Notify SCM changes. [#1415](https://github.com/screwdriver-cd/screwdriver/issues/1415)

## Discussion Notes

1. Remote trigger functional tests has been turned off in beta environment since it was blocking API pipeline. To be investigated on what is causing tests to fail on beta environment.
1. cdCon proposals for talks `CI/CD with Open Source Screwdriver` and `Case Study: How Yahoo! Japan Uses and Contributes to Screwdriver at Scale` has been accepted. 
