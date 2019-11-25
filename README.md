# Stabilization Brigade Meeting started on 2019-11-12 07:02:00 -0800 PST

## Attendance
- Aishwarya Rana
- Chip Boling
- David Bainbridge
- George Munteanu
- Gilles Depatie
- Girish Kumar
- Kent Hagerman
- Larry Ho
- Matt Jeanneret
- Scott Baker
- Serkant Uluderya (netsia)
- knursimu
- zdw

## Topic: Unit Test Coverage (2m39s)
- @khen submitted two mocks in Voltha-lib: a Kafka mock and and embedded etcd
- these mocks can help flesh out unit tests for core
- @khen has some unit tests in the core that can be instructional on how to use them.

## Topic: JIRA Update (50s)

## Topic: Patchsets (2m7s)
- we need more focus on code review

## Topic: Attention Items (1m40s)

## Topic: VOL-2173 - may be a BCM bug waiting for response (13m11s)
- VOL-1977 works usually twice, fails on third time. Working working @teo
- VOL-1977 may be related to VOL-2201
- VOL-2223 - introduced on a commit Friday. There is a flow that is not pushed when custom profiles. Issue has been identified, should be a fix today or tomorrow. If not fixed today then current patch will be reverted around 1/2 p EST.
- VOL-2180 - will be discussed on VOLTHA community meeting
- VOL-1942 - ongoing issue. This is a known bug and being worked on the performance brigade.
- VOL-2201 - triage seems to indicate the openly adapter crashed
- VOL-2202 - @matt cannot reproduce on hardware
- waiting for response from assignee to understand test scenario better.
- VOL-1802 - waiting for feedback to see if @teo has verified the issue
- VOL-1914 - @dbainbri to verify
- VOL-2199 - @smbaker working to reproduce it today.

# Meeting ended at 2019-11-12 07:23:04 -0800 PST
