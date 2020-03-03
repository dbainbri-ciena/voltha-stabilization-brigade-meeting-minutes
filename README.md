# Stabilization Brigade Meeting started on 2020-02-25 09:02:00 -0800 PST

## Attendance
- Andy Bavier
- Chaitrashree G S
- David Bainbridge
- Girish Kumar
- Hardik Windlass (Infosys)
- Julie Lorentzen
- Kent Hagerman
- Matt Jeanneret
- Neha Sharma
- ONF Zoom-3
- Scott Baker
- Serkant Uluderya
- Zack
- khenaidoo Nursimulu
- sauravdas
- taskin_ucpinar

## Topic: Test Coverage review (4m26s)
- test coverage flat
- after bugs are fixed we might be able to put more focus on quality unit tests
- when you add a new function first thing should be to write a new unit test
- no plan to adopt a new testing framework
- JIRA and patch sets

### Actions
- dbainbri(N/A): drop sim adapters from code coverage list

## Topic: jira and patch sets (1m47s)

## Topic: jia walk (49m20s)
- since the point release last week there have been nightly failures
- mostly the restart tests that are failing
- authentication failing after core restart.
- @suchitra to send links to the failures
- VOL-2657 passed 8/8 functional tests on hardware
- VOL-2631 almost ready, one nit left
- VOL-2344 currently not reproducable
- VOL-2106 cannot restart one adapter
- VOL-1383 depends on state update implementation
- device state patch set: https://gerrit.opencord.org/#/c/16569/
- VOL-1383 depends on VOL-21257 and patchset https://gerrit.opencord.org/#/c/16569/
- patch set https://gerrit.opencord.org/#/c/16569/ to remove WIP label
- VOL-2156 needs to be pulled into stabilization brigade
-  mark  VOL-2641 as unassigned need to find someone to pick up
- when testing connectivity to etcd and Kafka the tests should be about network partitioning to the service and not the service going down
- VOL-2658 requires API semantic changes to support server side filtering, sorting, and paging.
- VOL-2658 might be slit to multiple JIRAs one to move voltctl to unlimited timeout the other is the longer term fix.

### Actions
- dbainbri(n/a): move VOL-2156 into stabilization
- dbainbri(n/a): to split vol-2658
- dbainbri(n/a): to look for timeout jira for of agent and if not create one

### Decisions
- move the state changes post 2.3 and get started on reboot issues

# All Actions
- dbainbri(N/A): drop sim adapters from code coverage list
- dbainbri(n/a): move VOL-2156 into stabilization
- dbainbri(n/a): to split vol-2658
- dbainbri(n/a): to look for timeout jira for of agent and if not create one

# All Decisions
- move the state changes post 2.3 and get started on reboot issues

# Meeting ended at 2020-02-25 10:05:49 -0800 PST
