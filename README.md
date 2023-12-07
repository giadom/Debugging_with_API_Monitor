![Alternative text: "Azure Grotto, Naples by Ivan Konstantinovich Aivazovsky (1841)"](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c7/%D0%9B%D0%B0%D0%B7%D0%BE%D1%80%D0%B5%D0%B2%D1%8B%D0%B9_%D0%B3%D1%80%D0%BE%D1%82._%D0%9D%D0%B5%D0%B0%D0%BF%D0%BE%D0%BB%D1%8C.jpg/640px-%D0%9B%D0%B0%D0%B7%D0%BE%D1%80%D0%B5%D0%B2%D1%8B%D0%B9_%D0%B3%D1%80%D0%BE%D1%82._%D0%9D%D0%B5%D0%B0%D0%BF%D0%BE%D0%BB%D1%8C.jpg "Azure Grotto, Naples by Ivan Konstantinovich Aivazovsky (1841)")

# Topic of this guide
The technique illustrated in this guide is oriented **for Windows** and allows to debug a sample (i.e. an instance of a malware) using **also** _API Monitor_ (by Rohitab).  
This technique has sped up my malware analysis on several occasions and to use it you just need:
- your favourite debugger;
- `API Monitor`.

I will not explain in detail the functioning of this latter tool (for which I kindly redirect you to <http://www.rohitab.com/apimonitor>), but by the way I will explain something about it.

# Table of contents
At:
- "Guide" you will find the tutorial for this technique.
- "Filters" you will find some suggested filters to be feeded to `API Monitor`.

# To do list
- [ ] Explain why this work.
- [ ] Extend the APIs filterable by `API Monitor`.
