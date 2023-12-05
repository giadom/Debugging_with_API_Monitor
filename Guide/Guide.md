# Debugging with API Monitor
## Technique description
1. Start the chosen debugger with **administrative privileges**; for this tutorial I will use _x32dbg_
2. Start `API Monitor` with **administrative privileges** and
   1. load a filter that inspects the desired APIs and **has** a breakpoint[^1] on at least one API; I suggest to load `APIs-frequently_used_enhanced.xml` present in the "Filters" directory of this repository;
   2. start monitoring a **new** sample (i.e. a program not currently running).
3. At this point the program will break at the breakpoint specified in the XML filter file (for the `APIs_frequently_used_enhanced.xml` file it's the `` API).
4. Attach the debugger to the monitored sample.

[^1]: Read the caveat about the breakpoint on the `README.md` file in the "Filters" directory.
## Other notable use cases
### Analyse some anti-static-analysis techniques(?)
### Get the malicious payload injected in a victim process/thread

# FAQs
## Why not simply attach API Monitor to a debugged program?
Unfortunately API Monitor will fail in doing such operation: it will print an error message.  
![Alternative text: "API Monitor error while attaching to a debugged program"](./Images/.png)
## What about anti-debugging techniques?
This technique (as it is) can be detected by a sample looking for manually inspection traces.
