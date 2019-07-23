# Stabilization Meeting started on 2019-07-23 07:00:00 -0700 PDT

## Attendance
- David Bainbridge
- zdw
- Kent Hagerman
- Scott Baker
- Andy Bavier
- kailashkhalasi
- Girish GC
- khenaidoo Nursimulu
- Kyryll Sheychenko
- Shaun Missett (Radisys)
- aghosh
- teone
- Aishwarya Rana
- Gilles Depatie
- Marcelo
- jzhang
- George Munteanu (Furukawa)
- sauravdas

## Topic: intro (2m55s)
- time conflict SEBA tiger team meeting, Saurav recommend that SEBA meeting gets resceduled

## Topic: agenda bashing (12s)
- no changes

## Topic: Goal and Scope (24m31s)
- brigade will focus on VOLTHA only, but as VOLTHA is not standalone ONOS apps required will have to be included
- NEM layer makes activate subscriber call, this will have to be a manual step without SEBA/NEM
- Matt proposed a plan to come up with a couple of stable releases and a plan to introduce new features and maintain stability.
- the final user of VOLTHA is the operator and thus the result has to meet their expectations.
- need a way for new features to be introduced while maintaining stability.
- reviews raised for tech profiles for v 2.x
- MVP from previous meeting really features for stability release
- the list of stability features from previous meetings needs more clarification, example for HA
- plan would be to settle on minimal feature set to stabilize and then come up with a viable way to introduce new features.
- include numbers of OLT/ONUs as well as what adapters and end devices
- action item should include how VOLTHA is going to be tested as well as what is going to be tested.
- suggested that each release of VOLTHA should include a test suite

### Actions
- dbainbri(7/30): clarify minimal set of feature for stabilization

## Topic: Branch and release strategy (30m40s)
- strategy is similar to what is being used in SEBA, individual component and brought together into a solution.
- meant to be suitable for stabilization as well as on going releases and feature introduction
- doesn’t address lifecycle issues such as how many releases to support.
- suggestion is to develop fix on master when possible and then move it to the stabile release branch
- changes that go into helm charts are atomic across the solution
- do we have a HEAD test cases that will run against the latest of everything, but it may fail at times
- the helm chart needs to be up versioned when any of the components it uses has a new tag
- when a feature is submitted, end to end testing is submitted as well.

### Actions
- zdw(7/30): update document to include example of cross repo patchset update

### Decisions
- will use patchiest and not feature branches
- sanity tests are single repo focused
- cross repo tests are when helm chart version is bumped

# All Actions
- dbainbri(7/30): clarify minimal set of feature for stabilization
- zdw(7/30): update document to include example of cross repo patchset update

# All Decisions
- will use patchiest and not feature branches
- sanity tests are single repo focused
- cross repo tests are when helm chart version is bumped

# Meeting ended at 2019-07-23 08:08:41 -0700 PDT
