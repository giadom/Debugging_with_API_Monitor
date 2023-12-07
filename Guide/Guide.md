# Debugging with API Monitor
## Technique description
1. Start the chosen debugger with **administrative privileges**; for this tutorial I will use _x32dbg_.
2. Start `API Monitor` with **administrative privileges** and
   1. load a filter that blocks as soon as possible the sample to be analysed; I suggest to use the [Kernel32_Ntdll.xml](https://github.com/giadom/Debugging_with_API_Monitor/tree/main/Filters/) file present in the "Filters" directory of this repository;  
      ![Alternative text: ""](./Images/.png)
   2. start monitoring a new sample (i.e. a program **not currently running**).
3. As you can see the program has stopped immediatly thanks to `API Monitor` (if you used the suggested filter, this interruption happened because every program calls immediatly an API of `Kernel32.dll` or `Ntdll.dll`); do not press the _Continue_ or _Break_ buttons for now.
4. **Attach** the debugger chosen to the sample.
5. Put a **breakpoint** (a software one will be fine) to the entry point of the sample.
6. Press the button to continue the execution(?) (you will not move the Instruction Pointer because `API Monitor` is blocking it).
7. **Clear** the API filters.
8. Load a filter that filters/inspects the **desired APIs**; I suggest to load `APIs-frequently_used_enhanced.xml` present in the "Filters" directory.
9. 

[^1]: Read the caveat about the breakpoint on the `README.md` file in the "Filters" directory.
## Other notable use cases
### Analyse some anti-static-analysis techniques(?)
### Get the malicious payload injected in a victim process/thread

# FAQs
## Why do not simply attach API Monitor to a debugged program?
Unfortunately API Monitor will fail in doing such operation: it will print an error message.  
![Alternative text: "API Monitor error while attaching to a debugged program"](./Images/.png)

## What about anti-debugging techniques used by samples?
This technique (as it is) can be detected by a sample looking for manually inspection traces.

# To do list
- [ ] Explain why this technique works.
