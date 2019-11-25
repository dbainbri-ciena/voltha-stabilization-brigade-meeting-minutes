# Stabilization Brigade Meeting started on 2019-11-19 07:02:00 -0800 PST

## Attendance
- Amit
- Andy Bavier
- Chip Boling
- Chris Busch
- David Bainbridge
- Girish Kumar
- HARDIK WINDLASS (Infosys)
- Kent Hagerman
- Scott Baker
- knursimu
- taskin_ucpinar

## Topic: Unit Test Coverage (13m20s)
- good bump on lab-go, other not so much
- unit tests need to verify function behavior
- can gerrit check and report or -1 when coverage goes lower on code commit
- using interfaces in the code over structs and bound functions helps with unit testing because it allows the definition of mocks.
- as we define interfaces we need to make sure that we check that structs continue to implement the interfaces.
- need to think about restructuring voltha-go repo

## Topic: JIRA Update (8m27s)
- unresolved JIRAs and patchiest counts are related
- please take time to review patchsets
- as repos can pass the SCA tests we can add an sca Makefile target to the lint dependencies.
- need a default sca configuration as to what is required to pass
- python 3 conversion is going well

# Meeting ended at 2019-11-19 07:25:03 -0800 PST
