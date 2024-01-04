![Alternative text: "Azure Grotto, Naples by Ivan Konstantinovich Aivazovsky (1841)"](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c7/%D0%9B%D0%B0%D0%B7%D0%BE%D1%80%D0%B5%D0%B2%D1%8B%D0%B9_%D0%B3%D1%80%D0%BE%D1%82._%D0%9D%D0%B5%D0%B0%D0%BF%D0%BE%D0%BB%D1%8C.jpg/640px-%D0%9B%D0%B0%D0%B7%D0%BE%D1%80%D0%B5%D0%B2%D1%8B%D0%B9_%D0%B3%D1%80%D0%BE%D1%82._%D0%9D%D0%B5%D0%B0%D0%BF%D0%BE%D0%BB%D1%8C.jpg "Azure Grotto, Naples by Ivan Konstantinovich Aivazovsky (1841)")

# Topic of this guide
The technique illustrated in this guide is oriented **for Windows** and allows to debug a sample (i.e. an instance of a malware) using **also** _API Monitor_ (available at <http://www.rohitab.com/apimonitor>).  
This technique has sped up my malware analysis on several occasions and to use it you just need:
- your favourite debugger;
- `API Monitor`.

In a nutshell, you will:
1. debug a sample (including the possibility to **move its Instruction Pointer** as you whish);
2. track via `API Monitor` the APIs used by the sample (which is **still** under debugging).

# Table of contents
At:
- "Guide" you will find the tutorial for this technique.
- "Filters" you will find some suggested filters to be feeded to `API Monitor`.

# Acknowledgements
I would like to thank professor D. C. D'Elia for the clarifications and suggestions about this guide.
