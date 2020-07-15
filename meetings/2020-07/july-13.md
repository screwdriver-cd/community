# Meeting Notes - 2020-07-13

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

1. Improved UX for Pipeline Secret update/delete. [#1892](https://github.com/screwdriver-cd/screwdriver/issues/1892)
1. Made API call timeout configurable for launcher. [#2106](https://github.com/screwdriver-cd/screwdriver/issues/2106)
1. Added confirmation dialogue when deleting a Pipeline Secret. [#2117](https://github.com/screwdriver-cd/screwdriver/issues/2117)
1. Implemented a fix for build periodic configuration not getting cleared up. [#2138](https://github.com/screwdriver-cd/screwdriver/issues/2138)



Work In Progress 

1. Updating browser tab favicon. [#1009](https://github.com/screwdriver-cd/screwdriver/issues/1009)
   1. Will discuss in the Github issue on design. 
1. Application Metrics. [#2115](https://github.com/screwdriver-cd/screwdriver/issues/2115)
   1. VZM is using AWS Cloudwatch search for rudimentary metrics. Need a comprehensive solution.



Operational issues and feature requests

1. Template namespace is missing in Create pipeline page. [#2140](https://github.com/screwdriver-cd/screwdriver/issues/2140)

#### From Verizon Media:


Work In Progress 

1. Fix for multiple join jobs due to a race condition. [#2071](https://github.com/screwdriver-cd/screwdriver/issues/2071)
1. Enhancements to pipeline job list view. [#2124](https://github.com/screwdriver-cd/screwdriver/issues/2124)



## Discussion Notes

1. [#2106](https://github.com/screwdriver-cd/screwdriver/issues/2106) still cannot be used since `executors` need to be modified to pass in this value. VZM team to take a look into this. Created [#2150](https://github.com/screwdriver-cd/screwdriver/issues/2150) to track
1. VZM tried upgrade of Sonarqube from 6.x to 7.x and upgrade ran for over 4 days and had to roll back. Updated plan is to upgrade without carrying over data.
1. Supratik gave a demo of his GSoC project of Deploy Key generation as part of a new pipeline creation. Demo went well, and primary use-cases works as expected.
1. VZM team to start looking into [denali-ember](https://github.com/denali-design/denali-ember) for UI components. Screwdriver UI design ie heavily influenced by Denali and is create by same same Design team behind Screwdriver UI.
1. Need a replacement for Hapi.js since it's on EOL path. 

