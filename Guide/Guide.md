# Debugging with API Monitor
## Technique description
1. Start `API Monitor` with administrative privileges.
2. Load a filter that inspects the desired APIs and having a breakpoint on at least one API; I suggest to load `APIs-frequently_used_enhanced.xml` present in the "Filters" directory of this repository.
## Other notable use cases
### Analyse some anti-static-analysis techniques(?)
### Get the malicious payload injected in a victim process/thread

# FAQs
## Why not simply attach API Monitor to a debugged program?
Unfortunately API Monitor will fail in doing such operation: it will print an error message.
## What about anti-debugging techniques?
This technique (as it is) can be detected by a sample looking for manually inspection traces.
