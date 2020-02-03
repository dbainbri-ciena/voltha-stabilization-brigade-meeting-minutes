# Stabilization Brigade started on 2020-01-28 07:02:00 -0800 PST

## Attendance
- Andy Bavier
- Chaitrashree G S
- Chip Boling
- David Bainbridge
- Girish Kumar
- Hardik Windlass (Infosys)
- Julie Lorentzen
- Kent Hagerman
- Mike Emmendorfer
- ONF Zoom-2
- Scott Baker
- khenaidoo Nursimulu
- taskin_ucpinar
- zdw

## Topic: test coverage (47s)
- no change in coverage from last time

### Actions
- dbainbri(2/4): check py tests to see if they are being recorded correctly

## Topic: jira and patch update (16m51s)
- 52 open patch set need reviewed and merge
- what is the reason for there long patch set life
- people need to shepherd their patch set until it is reviewed and merged.
- if you have a patch set that needs to be talked about to see if it should go forward, raise its visibility on the slack channel or in this meeting
- because of some large changes recently many changes need to be manually rebased, which slows the process
- we need a suite a test that covers restarting scenarios
- if the strictness of the review process goes up then the queue of the patch sets increasersd
- there are more robot tests available for various scenarios than what is used for sanity.
- developers can run all the robot tests manually
- can we know when a patch last had a comment

### Actions
- dbainbri(2/4): find our how many require a rebase
- dbainbri(2/4): post patchset report to slack channel

## Topic: docker and ci tools (15m16s)
- the tools have been containerized and are in their own repo but not being used for the auto builds
- needs to be looked over once and merged into each repo
- merging into a repo means convert the makefile in each repo to use the containerized tool
- tools make photos, listing, etc. docker builds are not changerd
- each file for golang has to go through protobuf compiling individually which slows down the process a bit when using containerized tools
- request for reviews on the code later today
- once a repo is converted to use these tools using the containerized tools will be required.
- so Docker would be required to test.
- This would improve consistency.  Having the option of using local tools may be useful for advanced developers, but shouldn't be the default tools.
- about a 3sec (avg on linux) time increase when running make test using containers
- the standard “go test” will still be a viable use case

## Topic: logging guidelines (10m21s)
- https://docs.google.com/document/d/1oXkhBPTA3fW35d--OcZTORgIBInixkTiMLLL0K5Ry_4/edit?usp=sharing
- logger var is a package global
- log level names need to be consistent with work in jira

### Actions
- dbainbri(2/4): break up fatal and error
- dbainbri(2/4): limit levels based on lira discussion

# All Actions
- dbainbri(2/4): check py tests to see if they are being recorded correctly
- dbainbri(2/4): find our how many require a rebase
- dbainbri(2/4): post patchset report to slack channel
- dbainbri(2/4): break up fatal and error
- dbainbri(2/4): limit levels based on lira discussion

# Meeting ended at 2020-01-28 07:46:38 -0800 PST
