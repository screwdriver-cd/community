# Meeting Notes - 2020-11-19

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Keisuke Kumada](https://github.com/kumada626)
- Mansoor Chengat
- Yahoo! JAPAN Team

## Agenda

### From Yahoo! JAPAN:

#### Completed Work

1. [Fix](https://github.com/screwdriver-cd/sd-local/pull/49) for `sd-local` where large step lines was breaking the execution. 


#### Work In Progress 


1. `sd-local` environment variables with spaces [don't work](https://github.com/screwdriver-cd/screwdriver/issues/2280).
2. Started work on feature to [prevent certain jobs](https://github.com/screwdriver-cd/screwdriver/issues/1901) from being restarted.
3. [Enhancement to default build cluster selection](https://github.com/screwdriver-cd/screwdriver/issues/2258) logic to prevent auto selecting a cluster.


#### New Issues


### From Verizon Media:

#### Completed Work

1. Supporting container pull [configurations](https://github.com/screwdriver-cd/screwdriver/issues/2265) in `executor-k8s`
2. [Downtime view](https://github.com/screwdriver-cd/screwdriver/issues/2199) metrics on Build Metrics page. 

#### Work In Progress 

1. Collections end point performance fix. [#2267](https://github.com/screwdriver-cd/screwdriver/issues/2267)
   1.   API work completed. UI work on lazy loading pending.
2. Bookends to run on aborted builds.
   1. work is done and available in open source SD. Feature [verification](https://github.com/screwdriver-cd/screwdriver/issues/1125) pending.



#### Operational issues and feature requests

1. Job display name feature [bugs](https://github.com/screwdriver-cd/screwdriver/issues/2273).
2. notifications settings bugs [#2276](https://github.com/screwdriver-cd/screwdriver/issues/2276) & [#2275](https://github.com/screwdriver-cd/screwdriver/issues/2275).
3. [Stale metadata](https://github.com/screwdriver-cd/screwdriver/issues/2278) on remote-join.
4. Create pipeline flow [not listing](https://github.com/screwdriver-cd/screwdriver/issues/2282) all available templates.
 
### Discussion Notes

1. Kata container setup in Yahoo! JAPAN is not working as expected.
   1. VZM notes
        1. VZM don’t have docker in our setup, uses containerd storage setup
        2. We use containerd + devmapper, no overlay fs
        3. We use k8s runtime to route builds to kata nodes
        4. We will move further discussion to slack channel

