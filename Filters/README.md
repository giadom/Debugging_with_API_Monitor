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
- `APIs_frequently_used.xml` provides a filter with often abused Windows APIs (less than the first one); such APIs come out from:
  - suggestions from <https://malapi.io/> (which maps Windows APIs to common techniques used by malware);
  - suggestions from <https://www.sans.org/white-papers/33649/> (which is a white paper about abused APIs);

# Caveats and suggestions
- When putting a breakpoint in one API, be conscious that it will interrupt the sample every time it is called.
- Filtering too many APIs will slow down the program under inspection.
- Regardless to the filter chosen, I suggest to keep it update during your carreer (e.g. by adding those unfiltered APIs used by a brand-new malware).

# To do list
- [ ] Extend the APIs filterable by `API Monitor` (i.e. modify the inner XML files of `API Monitor` in order to provide more APIs filterable by the user).
