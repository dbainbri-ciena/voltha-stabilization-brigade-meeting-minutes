# Stabilization Meeting started on 2019-08-13 07:02:00 -0700 PDT

## Attendance
- Aishwarya Rana
- Andy Bavier
- David Bainbridge
- Gilles Depatie
- Girish
- Julie Lorentzen
- Kent Hagerman
- Kyryll Sheychenko
- Matt Jeanneret
- Open Networking Foundation
- Scott Baker
- Vikas Arora
- kailashkhalasi
- khenaidoo Nursimulu
- sbarbari
- taskin_ucpinar
- teone
- zdw

## Topic: action item review (50s)
- Kailash did review the spreadsheet and working on ironing out auth issues to be consistent

## Topic: tech profile status (34m32s)
- Matt has tested on hardware and had to tweak SADIS settings and ONOS is not adding first EPOL flows
- Matt has seen success 1 out of 4 times, seems to be a timing issue
- Matt has patch set out for bbsim, which sees tech profile work with auth and DHCP
- two main issues, a BAL timing issue and the Onos app AAA patch
- please test the BBSIM with TP if you can to get multiple people working on it.
- ONF will try to test V2.x with h/w later this week.
- do we merge patchiest now before everything is working consistantly.
- actually working 3 out of 4
- applying patchiest across repos can be difficult
- master branch is stalled until the brigade branches
- Voltha-go, oprenolt, bbsim, and new versions of Onos patches are needed
- guide with SADIS options https://guide.opencord.org
- can we formalize what has been tested and against what
- automated testing is the correct direction, but we are not there yet.
- TT will test against hardware once the patched images are pushed to docker hub
- edge core will be testing on hardware
- edgecore will work with the community and DT and set up test labs, createa a CI/CD environment, and continuously test the branch(es) 
- repo will be tagged before TP patchset it merged

### Actions
- Matt(8/14): to push built images with TP patchiest to dockerhub

## Topic: stabilization branch (17m33s)
- when are we ready cut branch and free master
- issues or existing bugs will not prevent the stabilization branch creation
- event patch is significant
- event patch may not be complete
- event patch at https://gerrit.opencord.org/#/c/14866/
- and the cooresponding patch for the onu adapter:  https://gerrit.opencord.org/#/c/14865/
- need to create JIRAs for the outstanding items around event patchsets
- gating patchiest for branch are TP and event
- 4 or 5 minor patches outstanding.

### Decisions
- event patchset will be added before branch, but test cases are required
- will create 2.0.1 ag right before TP or events are merged
- wed 8/14 at noon PDT is the minor patchset merge deadline

# All Actions
- Matt(8/14): to push built images with TP patchiest to dockerhub

# All Decisions
- event patchset will be added before branch, but test cases are required
- will create 2.0.1 ag right before TP or events are merged
- wed 8/14 at noon PDT is the minor patchset merge deadline

# Meeting ended at 2019-08-13 08:03:20 -0700 PDT
