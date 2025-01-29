# ClickToPhotonDebunked
Click to Photon - one of the most respected ways to measure latency for gaming. What if Click to Photon doesn't represent latency properly at all?

# Introduction
Click to Photon is one of the most respected ways to measure end-to-end latency. From tech YouTubers to multi-trillion dollar companies this method is used all over the tech industry. Click-To-Photon is the time between you clicking your mouse and seeing a response on the screen: ex, shooting in a game. Click to Photon can be measured by manually counting frames using a camera for each shot or using a Click-To-Photon device. Photon devices typically use a photoresistor or a photodiode. Typically you take at least 100 shots with a camera or a Click-To-Photon device. According to TechTeamGB and google a photodiode is more precise. There is also a huge range of frames per second these tools capture starting from 1000 fps from high-speed cameras, Nvidias LDAT with 8800 fps, OSLTT cs with 65,000 fps (The tool I'm using), and many more. Enough intro let's dig into the problem with Click-To-Photon. 





# Bios Settings for Tweaked Configuration

> [!NOTE] 
> All related settings have been disabled such as  ASPM, LTR, OBFF, PowerDown settings, Memory power savers, Power saving states, Power gating, Clock gating, Dynamic Intel technologies, (excluding turbo boost and Speedstep), Mitigations, All power management settings, MachineCheck and MonitorMWait, Integrated GPU, event producing settings and watchdog settings.
> All related settings have been enabled or changed such as PCI delay Optimization, Legacy IO Latency, Interrupt redirection mode selection was set to [fixed priority], automatic overclock, AP threads Idle manner was set to [Run Loop] and FCLK frequency for Early Power On was set to [1Ghz]
> 

> Though turbo boost 3.0 was disabled. A few other settings were changed


# Bios were set back to defaults after tweaked configuration (Settings were checked to make sure they reverted)


### Latency Tool
https://www.osrtt.com/osltt

65ksps 
