# Meeting Notes - 2020-02-24

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Keisuke Kumada](https://github.com/kumada626)
- [Shota Yoshika](https://github.com/s-yoshika)
- [DJ Erraballi](https://github.com/djerraballi)
- Yahoo! JAPAN Team

## Agenda

From Verizon Media:

1. Completed [#1091](https://github.com/screwdriver-cd/screwdriver/issues/1091) for displaying usage stats of Templates. Commands popularity is not straightforward and hence deprioritized.
2. New `queue-service` implementation in progress. This removes `node-resque` out of API into a separate micro service. [#1951](https://github.com/screwdriver-cd/screwdriver/issues/1951)
3. Parallel fork join for remote jobs, is feature complete. Working on validating existing flows and fixing a bug when `chainPR` is used. [#1710](https://github.com/screwdriver-cd/screwdriver/issues/1710). Feature is behind an environment variable `EXTERNAL_JOIN` and introduces new logic on how next jobs are triggered after a build is completed.
4. Working on a script to setup build cluster using AWS. [#1955](https://github.com/screwdriver-cd/screwdriver/issues/1955)
5. [DB refactoring #1865](https://github.com/screwdriver-cd/screwdriver/issues/1865) release caused an incident. Should strive to make DB schema change release separate from application release.


From Yahoo! JAPAN:

1. Live demo of SD Local mode [#1314](https://github.com/screwdriver-cd/screwdriver/issues/1314).
1. Fixed usability when logged in SCM is different [#1937](https://github.com/screwdriver-cd/screwdriver/issues/1937).
1. Fixes for supporting SCM branch names with `#` sign [#1925](https://github.com/screwdriver-cd/screwdriver/issues/1925).
1. Added meaningful page titles for Templates & Commands. [#1920](https://github.com/screwdriver-cd/screwdriver/issues/1920).
1. Fix for addressing restart scenario of jobs across events. [#1785](https://github.com/screwdriver-cd/screwdriver/issues/1785).
1. Fix for displaying proper GIT_BRANCH on Pull Requests. [#965](https://github.com/screwdriver-cd/screwdriver/issues/965).
1. [DB refactoring #1865](https://github.com/screwdriver-cd/screwdriver/issues/1865) feature complete.
1. Internal user reported issues
    1. Cache bookend error when using symlinks. [#1970](https://github.com/screwdriver-cd/screwdriver/issues/1970)


## Discussion Notes

1. Screwdriver joins CDF as inbuation project. [Media release](https://cd.foundation/blog/2020/02/19/screwdriver-joins-cd-foundation-as-its-first-incubation-project-treating-continuous-delivery-as-a-first-class-citizen-in-the-build-pipeline/) by CD Foundation happened on 02/19/2020. Verizon Media CEO Guru gave shout outs on social media.
1. DJ Errabali has been using Screwdriver in his health care startup for over an year. Likes the interface over Travis.
    1. Would like an overview on various executor and queue choices. Differences between `executor-k8s` & `executor-k8s-vm` are not clear.
    1. Would like to publish a blog post on Screwdriver setup and compare with other production setups.
1. Verizon Media team continues refactoring to enhance API performance.
