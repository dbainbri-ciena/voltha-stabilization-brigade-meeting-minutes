# Stabilization Brigade Meeting started on 2019-10-08 07:02:00 -0700 PDT

## Attendance
- Abhilash S L
- Aishwarya Rana
- Andy Bavier
- Chip Boling
- David Bainbridge
- Gilles Depatie
- HARDIK WINDLASS (Infosys)
- Julie Lorentzen
- Kent Hagerman
- Mahir Gunyel(Netsia)
- Marcelo
- Matt Jeanneret
- Matteo Scandolo
- Scott Baker
- Serkant Uluderya
- dineshbelwalkar
- jRvHVEOVcURcqRA56CRzynJvVlNh2/EFP5yoQ15UBaU=
- knursimu
- taskin_ucpinar
- zdw

## Topic: Repository and Releases (3m50s)
- components desegregated from Voltha-go
- have cut releases for repos
- If you get a tag collision error, see here: https://guide.opencord.org/developer/test_release_software.html#tag-collision-job-tag-collision
- release tags back to -dev version not complete

## Topic: dep to mod (1m19s)
- not all repos moved to go mod yet

## Topic: outstanding patchsets (7m21s)
- no patchiest waiting for cherry pick
- branches nearly identical
- need to add new repos to daily nag report tables
- ready to merge is missing some pyvoltha issues
- please review patchsets

## Topic: dashboard review (18m7s)
- still below where we need to be for unit tests
- "Needs Attention" on dashboard are items with `verify` (unsure if relevant, not stale) or `triage` (need help identifying the problem)
- To get the dashboard, go here: https://jira.opencord.org/secure/ConfigurePortalPages!default.jspa?view=search , click "Search" then click the Star next to `VOL - Brigade - Stabilization`, and it will show up in the Dashboard section in the top menu.
- what is the expected behavior of disable/enable for OLTs and ONUs (VOL-1802)
- we need to defined expectations around enable/disable for devices
- Khen working on document about device state which will (or should) cover issues about disable/enable
- for any issue with the new BBSIM please reach out to @teone on slack
- there is now slack channel for kind-voltha
- might be ready to bring kind-voltha into gerrit

### Actions
- zdw(N/A): to look why not all repos repos reporting coverage in jenkins

# All Actions
- zdw(N/A): to look why not all repos repos reporting coverage in jenkins

# Meeting ended at 2019-10-08 07:33:44 -0700 PDT
