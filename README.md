# Stabilization Meeting started on 2019-08-20 07:02:00 -0700 PDT

## Attendance
- Aishwarya Rana
- Amit
- Andy Bavier
- Chip Boling
- David Bainbridge
- George Munteanu (Furukawa)
- Gilles Depatie
- Julie Lorentzen
- Kailash
- Kent Hagerman
- Khen
- Kyryll Sheychenko
- Marcelo
- Matt Jeanneret
- Open Networking Foundation
- Saurav
- Scott Baker
- taskin_ucpinar
- teone
- zdw

## Topic: Action item review (1m0s)
- Matt posted docker images with TP patches for testing

## Topic: tech profile status (8m26s)
- lots of testing TP patchiest last week
- is it time to merge TP patches
- content to merge
- tag before merge
- David to work with Zack on tagging
- for openlt agent it is thought that version 1.7 should be used
- not all hardware has TP support yet.
- Shawn to check with Girish about openlt compatibility with 2.x

### Actions
- Khen,(David,): Matt will work to merge patchset today.
- Zdw(will): tag before merge

## Topic: repo versioning (5m54s)
- do version numbers stay in sync?
- or does every component have their own life cycle?
- versioning is done on a per-repo basis
- helm charts unify version of multiple (different version) components
- will move forward to have repos versioned independently
- splitting up components in the voltha-go repo (rw_core, affinity router, etc.) into their own repos
- Not sure how long this would take or the priority
- splitting will be proposed after brigade

### Actions
- David(will): create JIRA to split repo

## Topic: proposed stabilization roadmap (25m39s)
- proposal includes some of the existing proposals of the brigade in terms of bug fix and cherry pick flows
- the proposal includes date milestones on the process to help focus the effort
- should get an inventory of improvements to date to help understand what work is left.
- mechanics of versions/branches?  Process not defined quite yet.
- changes applied to either/both branches on a per-patchset level
- blue arrows are patchset fixes (cherry picked or reworked to the other branch)
- testing framework and integration tests should be applied to both master and stabilization branch
- code and process standards developed under the stabilization branch will also apply to master
- stabilization brigade needs to define it goals a little more clearly
- when the brigade has reached its goals the brigade goes away as does the branch
- patchsets should be cherry picked from stabilization branch to master after they have been merged into the stabilization branch.
- the plan is to propose processes and guidlelines for testing and commit standards. The plan is to create working groups (smaller than entire community) to develop and then socialize to community for comment and change.

## Topic: outstanding issues before branch (10m40s)
- TP and event model patchset needed before branch
- need openonu testing to verify the event model patchset

### Actions
- Taskin(to): get the patch tested
- Matt(will): get the patchset numbers to Taskin

## Topic: Testing after the branch (4m51s)
- we need more people with hardware to test, i.e. more people should purchase hardware
- can we get an open hardware test bed?
- carry over topic to next meeting

# All Actions
- Khen,(David,): Matt will work to merge patchset today.
- Zdw(will): tag before merge
- David(will): create JIRA to split repo
- Taskin(to): get the patch tested
- Matt(will): get the patchset numbers to Taskin

# Meeting ended at 2019-08-20 07:59:39 -0700 PDT
