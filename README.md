# ClickToPhotonDebunked
Click to Photon - one of the most respected ways to measure latency for gaming. What if Click to Photon doesn't represent latency properly at all?

# Introduction
Click to Photon is one of the most respected ways to measure end-to-end latency. From tech YouTubers to multi-trillion dollar companies this method is used all over the tech industry. Click-To-Photon is the time between you clicking your mouse and seeing a response on the screen: ex, shooting in a game. Click to Photon can be measured by manually counting frames using a camera for each shot in game or using a Click-To-Photon device. Click-To-Photon devices typically use a photoresistor or a photodiode. According to TechTeamGB and google a photodiode is more precise. Typically you take at least 100 shots with a camera or a Click-To-Photon device.  There is also a huge range of frames per second these tools capture starting from 1000 fps from high-speed cameras, Nvidias LDAT with 8800 fps, OSLTT cs with 65,000 fps (The tool I'm using), and many more. Enough intro let's dig into the problem with Click-To-Photon. 

# Testing
I took 10 (100 sample tests) of both my everyday computer with no modifications except the best power mode in the Windows 11 settings and also took tests with my PC with virtually no power savers, events, Security mitigations, Static PC algorithms, etc. This should in theory reduce Jitter (The variance in latency) by having fewer settings changing on the whole PC.
Lets first start off by observing the so-called jitter visually with data across all stock and tweaked tests.

## Stock
![Test1Pic](https://github.com/user-attachments/assets/67e14b20-297a-40d9-8c98-0e311cbba116)

![Test2Pic](https://github.com/user-attachments/assets/bcb4fe32-4d0b-4eec-ae83-d692b270bcfb)

![Test3Pic](https://github.com/user-attachments/assets/4916f468-2099-4a42-b4ba-e5b47504c2fa)

![Test4Pic](https://github.com/user-attachments/assets/d6a76b01-d67d-4f2a-bea7-36a1b78f7422)

![Test5Pic](https://github.com/user-attachments/assets/854b6d1a-2e4c-42b8-a726-3f1c3ae3ab46)

![Test6Pic](https://github.com/user-attachments/assets/edb71648-12e1-4971-b2bb-3c8b2290389d)

![Test7Pic](https://github.com/user-attachments/assets/90954c2c-4c14-4dcd-87fe-f81c554fd6f0)

![Test8Pic](https://github.com/user-attachments/assets/0c98c19f-20d1-4207-ac92-2918eb7f762c)

![Test9Pic](https://github.com/user-attachments/assets/bfce425c-c5b3-4910-b644-20a50151b41e)

![Test10Pic](https://github.com/user-attachments/assets/6ad43c32-5c41-439f-8312-962e870e528e)

## Tweaked 

![Test1Pic](https://github.com/user-attachments/assets/1fb4265a-b500-402a-a0a9-8a7b419919af)

![Test2Pic](https://github.com/user-attachments/assets/4dc3f570-b15d-4c70-88af-aa8ff9da43a4)

![Test3Pic](https://github.com/user-attachments/assets/a2f863db-2cdb-48f0-afb3-ee087eae23e2)

![Test4Pic](https://github.com/user-attachments/assets/ac1dddb8-8ec2-4dc3-be0c-b3c1a2de030d)

![Test5Pic](https://github.com/user-attachments/assets/bd6181eb-95de-4853-a052-f5676d46b7c9)

![Test6Pic](https://github.com/user-attachments/assets/caf9cac5-2a98-4710-80d4-c72498572404)

![Test7Pic](https://github.com/user-attachments/assets/ef9a204e-2cc1-410f-880a-ba04bb245337)

![Test8Pic](https://github.com/user-attachments/assets/5aaa43a3-7572-4300-be78-11343394d231)

![Test9Pic](https://github.com/user-attachments/assets/0ebdafc8-fabd-4523-a356-146d3465a8a7)

![Test10Pic](https://github.com/user-attachments/assets/ac1a915d-2d3b-4aa5-9e99-66e1256e029c)



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
