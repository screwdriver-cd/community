# Meeting Notes - 2020-12-03

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Keisuke Kumada](https://github.com/kumada626)
- [Tiffany Kyi](https://github.com/tkyi)
- Yahoo! JAPAN Team

## Agenda

### From Yahoo! JAPAN:

#### Completed Work

1. Ability to [mount ssh socket](https://github.com/screwdriver-cd/sd-local/pull/50) in sd-local interactive mode.
2. Job display name [bug fixes](https://github.com/screwdriver-cd/screwdriver/issues/2273). 


#### Work In Progress 

1. [Validation](https://github.com/screwdriver-cd/screwdriver/issues/2051) for settings.
2. [UI to highlight](https://github.com/screwdriver-cd/screwdriver/issues/2168#issuecomment-721522525) latest commit in events tab.


#### New Issues
1. `sd-local`  [ability to mount](https://github.com/screwdriver-cd/screwdriver/issues/2294) custom volumes.


### From Verizon Media:

#### Completed Work

1. `sd-local` to work with non-sudo user containers.
2. K8S pod [label support](https://github.com/screwdriver-cd/screwdriver/issues/2265).
3. [Run teardown](https://github.com/screwdriver-cd/screwdriver/issues/1125) steps for aborted builds.
4. [SonarQube integration ](https://github.com/screwdriver-cd/screwdriver/issues/2288)for all Screwdriver projects.

#### Work In Progress 

1. Collections end point performance fix. [#2267](https://github.com/screwdriver-cd/screwdriver/issues/2267)
   1.   API work completed. UI work on lazy loading pending.
2. [Stale metadata](https://github.com/screwdriver-cd/screwdriver/issues/2278) on remote-join.
3. [UI fixes](https://github.com/screwdriver-cd/screwdriver/issues/2124) to pipeline list view.
4. [Clickable URLs](https://github.com/screwdriver-cd/screwdriver/issues/1826) in log viewer


#### Operational issues and feature requests

1. Pipeline creation flow [should ask SCM permissions](https://github.com/screwdriver-cd/screwdriver/issues/2289) if not available.
2. Build cluster worker has [no functional tests](https://github.com/screwdriver-cd/screwdriver/issues/2281).
 
### Discussion Notes

