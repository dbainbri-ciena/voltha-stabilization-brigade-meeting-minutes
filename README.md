# Stabilization Meeting started on 2019-08-06 07:02:00 -0700 PDT

## Attendance
- Andy Bavier
- Bjoern
- David Bainbridge
- George Munteanu (Furukawa)
- Girish
- Kent Hagerman
- Stéphane Barbarie
- aghosh
- bill
- kailashkhalasi
- sauravdas
- teone

## Topic: Action Item Review (18m27s)

## Topic: patchiest updates (1m44s)
- patchset 1623 undergoing load testing and then will talk to the core team to set if it can be merged

## Topic: testing (27m56s)
- automated testings for Volta 2.x using kind-voltha
- test suite not complete but is a starting point
- tests are with bbsim
- jobs has been running for a couple days on ec2, stable since yesterday
- robot test framework is being used
- using voltctl as the cli utility tool
- bbsim onu activation test, enable active and reachable.
- at some point we need an automated test suite that uses physical devices
- tests suites use REST to ONOS to validate information in that system
- the test suite communicates with the RADIUS server to verify authentication
- seeing some inconsistency in the DHCP test case
- both addition and removal test cases covered
- test cases can be associated with JIRA items so that a test can be marked as a known failure until the JIRA is closed
- logs for all the pods are captured with the test to help with diag
- going to start running the tests on the “master” as opposed to the pinned 2.0.0 version specified in the charts
- also want to get the test to be able to run on each patchset
- running the equivalent tests on the hardware, such as nightly, will be important as well.
- the tests are in the repo voltha-system-tests
- for SEBA full test suite run nightly and a minimal subset run on each patchset, which may make sense to do for VOLTHA as well
- bulk of time spent downloading images
- when using physical devices it may take more time for test setup
- as an example using a physical set up a single test case is known to take 49h including physical device image updates
- the repo contains information on how to set up a test environment and how to contribute
- the goal should be to contribute a test when you submit a bug fix to help prevent regresstion
- when reporting a bug providing steps to reproduce the bug is important
- people should submit unit tests and e2e tests as then add feature code as well.
- discussion of code coverage, and trying to find what the "hot" parts of the codebase are (flame graphs), and deadlock detection.

### Actions
- Kailash(to): review the test case spreadsheet, recommend others look at the test framework.

# All Actions
- Kailash(to): review the test case spreadsheet, recommend others look at the test framework.

# Meeting ended at 2019-08-06 07:56:46 -0700 PDT
