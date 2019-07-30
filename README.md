# Stabilization Meeting started on 2019-07-30 07:03:00 -0700 PDT

## Attendance
- Aishwarya Rana
- Chip Boling
- David Bainbridge
- Gilles Depatie
- Julie Lorentzen
- Kent Hagerman
- Kyryll Sheychenko
- Matt Jeanneret
- Scott Baker
- aghosh
- kailashkhalasi
- khenaidoo Nursimulu
- teone
- zdw

## Topic: Agenda bashing (42s)

## Topic: action item review (15m9s)
- features list in spreadsheet
- sheet that covers components of voltha
- should some components be in their own repo
- when do we deprecated python adapter and remove it to its own repository.
- 1.6 doesn’t depend on the containerized adapters
- @zdw updated his branching document to cover multiple project updates

### Decisions
- continue to differentiate python and go version of adapter by tag for now
- change the default tag (master) to reference the go version
- while it make sense to split some projects into their own repo we will get the code working first, i.e. it is low priority

## Topic: of agent versions (6m19s)
- version in voltha-go started with 2.x, using GRPC for 2.x
- had to work with api server which required some logic changes
- of agent in voltha only works with 1.x grpc
- features from 1.x version have been mostly ported to 2.x
- there are additional libraries from 1.x needs to be ported to 2.x (pyvoltha, open omci)
- can we freeze the 1.x code to prevent the continues need to port form 1.x to 2.x

### Actions
- @dbainbri(8/6): to talk to someone about 1.x futures

## Topic: branch and freeze (26m32s)
- master version work today with older version of Onos and not tech profile to get a bbsim one up
- these patchsets will cause churn as things get settled.
- also needs to be tested on bbsim and hardware
- a few more hands to help out on writing unit tests for the golang adapter
- Existing team will write example tests for the golang adapter and then create tasks that others can take on
- no ETA for unit test passing at this time, but will be more than a couple of days.
- there other patches required to be feature complete, such a reconciliation.
- we can tag and branch repos independently and don’t have to be done all at once.

### Actions
- all(8/6): please identify all patchsets that are required before branch and freeze
- all(8/6): forward any JIRAs required for feature to @dbainbri

### Decisions
- no patchset will be merged unless we can prove that the e2e story works.

## Topic: CI/CD pipeline (1m45s)
- diagram depicts items that have been under discussion in terms of flow of development and gates to pass before merges

## Topic: post-release support (5m8s)
- need to make decisions around post-release support
- how many versions to support (example)
- may need to be raised to TST level
- policy should be defined / written about post-release
- seba has a policy of supporting 1 release behind
- need to define policy in terms of LTS release
- Release support needs to be informed by upgrade cycle of service providers.

# All Actions
- @dbainbri(8/6): to talk to someone about 1.x futures
- all(8/6): please identify all patchsets that are required before branch and freeze
- all(8/6): forward any JIRAs required for feature to @dbainbri

# All Decisions
- continue to differentiate python and go version of adapter by tag for now
- change the default tag (master) to reference the go version
- while it make sense to split some projects into their own repo we will get the code working first, i.e. it is low priority
- no patchset will be merged unless we can prove that the e2e story works.

# Meeting ended at 2019-07-30 08:04:23 -0700 PDT
