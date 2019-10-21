# Stabilization Brigade Meeting started on 2019-10-15 07:02:00 -0700 PDT

## Attendance
- Aishwarya Rana
- Andy Bavier
- Chip Boling
- David Bainbridge
- Gilles Depatie
- Hardik Windlass (Infosys)
- Julie Lorentzen
- Kent Hagerman
- Matt Jeanneret
- Matteo Scandolo
- Mike Gasser (AT&T)
- Scott Baker
- Serkant Uluderya
- Zdravko Bozakov
- dineshbelwalkar
- knursimu

## Topic: Branching Change (2m25s)
- we are no longer going to be cherry-picking to Voltha 2.1 and development will continue on master
- may branch laters if required.

## Topic: Repository Disaggregation (2m48s)
- Voltha-go has disaggregated into multiple respositories
- this means we are moving to a one repository to container type model
- plan is to move most of voltha-go common to a library repository
- the library move may be a little disruptive as it is done in sort of a rolling update.

## Topic: From dep to mod (2m14s)
- voltha-go (I think) is last repo to move to mod
- need to make sure that any build documentation is updated

## Topic: Dashboard Review (5m42s)
- need more unit tests, below 80% target on most packages
- about 57 issues open and not in progress

# Meeting ended at 2019-10-15 07:17:41 -0700 PDT
