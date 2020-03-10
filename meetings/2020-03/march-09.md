# Meeting Notes - 2020-03-09

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Keisuke Kumada](https://github.com/kumada626)
- [Shota Yoshika](https://github.com/s-yoshika)
- Yahoo! JAPAN Team

## Agenda

From Verizon Media:

1. Remote-Join feature has been released.
2. Ran node.js profiling in production to trace performance problems, but not seeing any issues.
3. GHE 2.19.8 and above introduces SSH CA for an org, but it's breaking Webhook signature validations.
4. Working on fixing restart scenarios across mutiple events. [#1785](https://github.com/screwdriver-cd/screwdriver/issues/1785)

From Yahoo! JAPAN:

1. SD Local mode is feature complete. [#1314](https://github.com/screwdriver-cd/screwdriver/issues/1314).
    1. Blog post pending. Verizon Media team can collaborate on blog.
    1. Need to tag docker containers as `stable`.
1. New environment variable for PR branch name is now available. [#965](https://github.com/screwdriver-cd/screwdriver/issues/965)
1. Fixed template/command data when semver versions are used. [#1891](https://github.com/screwdriver-cd/screwdriver/issues/1891) 
1. Correctly handle ignore commits. [PR 2009](https://github.com/screwdriver-cd/screwdriver/pull/2009)
1. Fixes for supporting SCM branch names with `#` sign [#1925](https://github.com/screwdriver-cd/screwdriver/issues/1925).
1. PR Open for granting users ability to delete templates and commands. [#1977](https://github.com/screwdriver-cd/screwdriver/issues/1977)
1. Internal user reported issues
    1. New feature request to handle template deprecation. [#1989](https://github.com/screwdriver-cd/screwdriver/issues/1989)


## Discussion Notes

1. Need formal process for tagging docker containers as stable. We should be doing this after a major feature work and a blog post is available for the fature. 
1. Verizon Media team can collaborate on blog post for sd-local.
