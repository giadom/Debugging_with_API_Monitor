# Table of contents
- `APIs_frequently_used_enhanced.xml` provides a filter with often abused Windows APIs; such APIs come out from:
  - samples that I personally analysed;
  - suggestions from <https://malapi.io/> (which maps Windows APIs to common techniques used by malware);
  - suggestions from <https://www.sans.org/white-papers/33649/> (which is a white paper about abused APIs);
  - personal refinement of the previous two points (i.e. I added APIs having similar functioning of cited ones).
- `Kernel32_Ntdll.xml` provides a filter that:
  - filters all the APIs present in _Kernel32.dll_ and _Ntdll.dll_;
  - breaks the execution **before** any call of them.
- `All_APIs.xml` provides a filter containing all the APIs filterable.

# Caveats
- When putting a breakpoint in one API, be conscious that it will interrupt the sample every time it is called.
- Filtering too many APIs will slow the program under inspection.
