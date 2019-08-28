# Stabilization Brigade started on 2019-08-27 07:02:00 -0700 PDT

## Attendance
- Aishwarya Rana
- Amit
- Andy Bavier
- Chip Boling
- David Bainbridge
- Divya(Infosys)
- Gilles Depatie
- Girish Kumar (Infosys)
- Hardik Windlass (Infosys)
- Julie Lorentzen
- Kailash
- Kent Hagerman
- Kyryll Sheychenko
- Mahir Gunyel(Netsia)
- Marcelo
- Scott Baker
- Vikas Arora
- jRvHVEOVcURcqRA56CRzynJvVlNh2/EFP5yoQ15UBaU=
- khenaidoo Nursimulu
- rakesh
- taskin_ucpinar
- teone
- zdw

## Topic: Action Item Review (1m20s)

## Topic: TP merge readout (1m41s)
- went pretty well
- thanks to Scott and Zack

## Topic: Event Format Status (3m25s)

### Actions
- Amit(9/3): follow up with Paul Devmalya and Matt about new event definition patchiest. Amit will follow up with email.

## Topic: Automated Testing (50m1s)
- presentation from Suchitra
- Automation Framework Proposal - https://docs.google.com/presentation/d/112xdckcM_a3OKs_ohfX9KZ3SwS3c6nkF2BlFrL0wW9c/edit
- goal is to automate majority of tests and a single framework for both bbsim and physical pods
- re-use/leverage work from SEBA
- want capability to diagnose (debug) when test fail
- Some hardware-based tests are hard to automate or require manual intervention (fiber pull) or special expensive hardware.
- Use of robot framework allows modularity and reuse of tests, integrates well with Jenkins, already have libraries used with SEBA
- developers will be able to run the tests locally via the Robot framework
- Robot framework was compared to other tools, such as Ansible and Robot framework was determined to be easier by the team
- Robot framework was used to test physical devices
- automation is done via python and Robot when testing physical devices
- deployment is done via Jenkins as a series of Helm charts
- tests are being run both on bbsim and physical PODs
- Ansible does not offer robust output as Robot as its focus is not testing
- there is a plan / roadmap for performance testing
- Voltha library uses voltha cli (ssh) to communicate to voltha
- the test sequence is based on the AT&T workflow today
- we may/should be including other workflows as well.
- the libraries have the capability to be used independent of the workflow
- The Robot framework library will wrap whatever interface (local CLI, remote CLI, REST, etc.) the component under test uses, so changing interfaces could be done at the library level.
- it is expected that all members of the brigade / community will contribute to testing scenarios
- documents exist that describe how to contribute to test cases
- voltha-system-tests repo: https://gerrit.opencord.org/gitweb?p=voltha-system-tests.git;a=tree
- please review the documentation about how to contribute to tests and if items that are desired are not covered we can update the documents with more details.
- testing docs: https://guide.opencord.org/cord-tester/
- The testing topology should be documented as part of the test setup
- physical lab setup guide: https://guide.opencord.org/profiles/seba/lab-setup.html
- there are deployment configuration files for each test from which topology can be implied
- Patchset verification builds a specific patchset
- Nightly test checks what have already been checked in.

### Actions
- Everyone(9/3): Review documentation that explains how tests are set up, how to integrate new tests, and how they'll be run.

# All Actions
- Amit(9/3): follow up with Paul Devmalya and Matt about new event definition patchiest. Amit will follow up with email.
- Everyone(9/3): Review documentation that explains how tests are set up, how to integrate new tests, and how they'll be run.

# Meeting ended at 2019-08-27 07:59:09 -0700 PDT
