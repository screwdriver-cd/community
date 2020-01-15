# Meeting Notes - 2020-01-13

## Attendees

- [Jithin Emmanuel](https://github.com/jithine)
- [Keisuke Kumada](https://github.com/kumada626)
- [Shota Yoshika](https://github.com/s-yoshika)
- Yahoo! JAPAN Team

## Agenda

From Verizon Media:

- Screwdriver team to start POC on `Kata` containers for replacing `executor-k8s-vm` which uses `hyperd`
- Current features in progres, Parallel workflow & making build timeout robust.
- Screwdriver being accepted as an incubation project at CD Foundation.

From Yahoo! JAPAN:

- Fixes for Templates and command showing wrong version has been released.
- Launcher & log service updated to support SD Local mode. Team to start working on rest of implementaion.
- Filed new issues affecting usability.

## Discussion Notes

[Build timeout fix](https://github.com/screwdriver-cd/screwdriver/issues/1710) implementataion has a bug which can cause builds to timeout earlier. Pull Requests are already open with fix.

[Templates & Commands can return wrong version](https://github.com/screwdriver-cd/screwdriver/issues/1891) if major or minor version alone is sepcifed. This is different from the fixes for DB query and needs to be fixed at application layer.

For [DB Size is growing](https://github.com/screwdriver-cd/screwdriver/issues/1865) PRs are open to reduce `step` information stored in `build` record.

New usability issues reported. These are to be reviewed with Design team at Verizon Media.
  * https://github.com/screwdriver-cd/screwdriver/issues/1903
  * https://github.com/screwdriver-cd/screwdriver/issues/1900
  * https://github.com/screwdriver-cd/screwdriver/issues/1892

New workflow feature request
  * https://github.com/screwdriver-cd/screwdriver/issues/1900
