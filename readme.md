#Nanomite - Graphical Debugger for x64 and x86 on Windows

## Features
- Debugging x86 and x64 (+ WOW64) processes
- Breakpoints
    - Software
	- Memory
	- Hardware
- Step In
- Step Over
- Step Out
- Step back to user code
- Attaching
- Detaching
- Single Step Tracing
- Supporting child processes
- Supporting multithreading
- Display source code
- Detailed view of:
	- disassembly
	- windows
	- handles
	- debug strings
	- threads
	- (child)processes
	- exceptions
	- process privileges
	- loaded modules
	- strings
	- callstack
	- stack
	- memory
	- heap
	- cpu registers
	- functions
	- pe header

## Changelog
###Version 0.1 beta 13
+ fixed some crashs related to the qt /MT build, see note for more details
+ fixed some bugs in the patch manager
+ fixed the symbol display in the trace view
+ added colors to the state bar
+ added missing edi/rdi register
+ added option break on tls callback
+ added possibility to show registers of a thread in detailview
+ added possibility to show TEB/TBI of a thread in detailview
+ added possibility to show PEB/PBI of a process in detailview
+ added possibility to set Nanomite as default JIT
+ updated PE-Editor layout
+ updated Options to include more options, easier config 

####Notes:
	- Needed to compile Qt with /MD because of issues with the cruntime. If you want to use the
	  debugger you have to install the visual c++ runtime 2010. 
	- You can save an exception to the list in the Options window. The debugger then knows how to handle it. 
		- 0 = break
		- 1 = pass to application
		- 2 = ignore

###For the full changelog click [here](https://github.com/zer0fl4g/Nanomite/blob/master/changelog.md)