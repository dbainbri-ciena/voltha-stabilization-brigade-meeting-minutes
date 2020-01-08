# Stabilization Brigade Meeting started on 2020-01-07 07:02:00 -0800 PST

## Attendance
- Andy Bavier
- Chaitrashree G S
- David Bainbridge
- HARDIK WINDLASS (Infosys)
- Kent Hagerman
- Scott Baker
- Serkant Uluderya
- Vignesh Ethiraj (Infosys Ltd)
- Zack Williams
- knursimu
- taskin\_ucpinar
- HARDIK WINDLASS (Infosys)

## Topic: unit test coverage (52s)
- not much change

## Topic: jira and patch set (1m49s)
- need to reduce the patch set back log

## Topic: freezing tool version (41m46s)
- different tool version can cause different build differences.
- do we need to have a bundle of tools (based on version) and then repo use a specific set / bundle
- the auto build checks to see if the checked in code generated from the protobufs is by regenerating code and then comparing to checked in code. However if the developer is using a different version of the generator then this check can be a failed positive.
- how does a developer verify they have the correct version of the tools
- This should be a check/verify of tool versions, but not an automatic install of tooling, as there are platform/dev environment differences.
- a standard tool set can be accomplished with either Vagrant VMs or Docker builds
- a developers local file system can be mounted into a docker container
- a docker build may extend the build cycle time in certain situations
- Kent will attempt a docker build for the protos repo
- Need a BOM of versions in any case, created during release engineering process.
- Discussion of how to apply this BOM across multiple code repos.
- we will have a BOM repo at some point in the future that will be enforced via an implementation mechanism
- related Jira: https://jira.opencord.org/browse/VOL-2298

# Meeting ended at 2020-01-07 07:54:51 -0800 PST
