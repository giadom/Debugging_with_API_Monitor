# Table of contents
- `APIs_frequently_used_enhanced.xml` provides a filter with often abused Windows APIs and a _before call_ breakpoint at the `` API; such filterable APIs come out from:
  - samples that I personally analysed;
  - suggestions from <https://malapi.io/> (which maps Windows APIs to common techniques used by malware);
  - suggestions from <https://www.sans.org/white-papers/33649/> (which is a white paper about abused APIs);
  - personal refinement of the previous two points (i.e. I added APIs having similar functioning of cited ones).
- `All_APIs.xml` provides a filter containing all the APIs filterable.

# Caveats
- When putting a breakpoint in one API, be conscious that it will interrupt the sample every time it is called. For this reason in `APIs_frequently_used_enhanced.xml` there is only one breakpoint that is triggered right after the sample start and before its harmful behaviour. In particular `` is often called only at the beginning of a program.
- Filtering too many APIs will slow the program under inspection.
