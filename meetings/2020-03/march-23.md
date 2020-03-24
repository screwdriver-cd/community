# Meeting Notes - 2020-03-23

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Keisuke Kumada](https://github.com/kumada626)
- Yahoo! JAPAN Team

## Agenda

From Yahoo! JAPAN:

Completed Work

1. SD Local mode is feature complete. [#1314](https://github.com/screwdriver-cd/screwdriver/issues/1314).
    1. Added `sudo` option
    1. Updated user guide.
    1. Added `LICENSE`.
1. Fixed build step [ordering](https://github.com/screwdriver-cd/models/pull/442).
1. Template owners can now delete template. [#1977](https://github.com/screwdriver-cd/screwdriver/issues/1977)

Operational issues and feature requests
1. Noticing performance issues on API. Suspect it's when updating pipelines with large number of jobs.
1. Chain PR not resuming pipeline on restart case. [#2029](https://github.com/screwdriver-cd/screwdriver/issues/2029)
1. Ability to show docker container digest. [#2028](https://github.com/screwdriver-cd/screwdriver/issues/2028)
1. Will look into [#2036](https://github.com/screwdriver-cd/screwdriver/issues/2036) for making build logs available in build container.


From Verizon Media:

1. [queue-service](https://github.com/screwdriver-cd/queue-service) code complete. Working on deployment aspects in OSSD.
    1. Current API doesn't work with [queue-worker](https://github.com/screwdriver-cd/queue-worker) and must be replaced with `queue service` for newer API deployments.
    1. Will share example configs.
1. [Kata container](https://github.com/screwdriver-cd/screwdriver/issues/818) work getting completed. Bulk of work is in installing Kata in build cluster and configuring kubernetes.
1. Inder who was interning with us has returned back to Canada due to Corona Virus situation. Work on Aggregate view of pipeline which he was driving is on hold for now.
1. Screwdriver is participating in Google Summer of Code via CD Foundation. We have a slack channel `#soc` with details.


## Discussion Notes

1. For performance problems, we need to evaluate logic when bulk update is done using `Promise.all`. Also new [queue-service](https://github.com/screwdriver-cd/qkueue-service) will help, since it will make API light weight.
1. Worth implementing container digest for executors docker & k8s only. Since k8s-vm will soon be retired when `kata` is operational.
1. `LICENSE` copyright name on newer repositories to be evaluated.
