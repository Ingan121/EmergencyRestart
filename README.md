# EmergencyRestart
(Almost) immediately reboot a Windows computer. If something goes wrong on your remote PC and you feel like it'll completely freeze soon, just run this to regain access to your PC.
This is accomplished by calling two functions inside NTDLL.DLL that are normally ran at the end of the normal shutdown process, [NtShutdownSystem](http://undocumented.ntinternals.net/index.html?page=UserMode%2FUndocumented%20Functions%2FHardware%2FNtShutdownSystem.html) and NtSetSystemPowerState.  

# Warning!  
Running this program will immediately shut down your computer, all unsaved data will be lost.  
Loss of data or data corruption could also be caused by the sudden shutdown (just like it could if you were to unplug your PC from power!)  
I'm not responsable for any loss of data caused by the usage of this program.  
I do not condone the usage of this program to cause damage to other people's hardware, software or data.  

# Requirements
Precompiled builds support Windows XP and onwards (compiled using the v141_xp build tools).  
Requires [Microsoft Visual C++ Redistributable for VS2015](https://docs.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170) or newer to be installed

# Usage  
Just open the executable.  

This is a fork of [PullThePlug](https://github.com/derivativeoflog7/PullThePlug), but it reboots the PC instead of shutting down.
Most of the original work done by [hxhl95](https://www.codeproject.com/Articles/34194/Performing-emergency-shutdowns), I just reimplemented part of their code.
