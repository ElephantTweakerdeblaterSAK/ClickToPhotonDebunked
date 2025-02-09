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

These pictures contain about 36 tests each, when we carefully look at these pictures we see tons of jitter, between all of these tests, across both stock and tweaked. This showcases how inconsistent latency really is. Now that you visually see this variance we can now question if each full 100 sample tests translates to consistent stdevs across all tests (spoiler it is absolutely inconsistent). Starting with Stock




# Test1 Reported avgs
 Click Time (ms) : 0.522  avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 12.487 avg
Total System Input Lag (ms) : 13.009 avg


# Test1 calculated my self
Total System Input Lag (ms) : 2.39924300037501  stdev
Display Latency (ms) : 2.3625156756254  stdev
Click Time (ms) : 0.296819635571176 stdev


# Test2 Reported avgs
Click Time (ms) : 0.491  avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 12.409 avg
Total System Input Lag (ms) : 12.9 avg


# Test2 calculated my self
Total System Input Lag (ms) : 2.34485888744295  stdev
Display Latency (ms) : 2.33775105333603  stdev
Click Time (ms) : 0.282524670416478  stdev


# Test3 Reported avgs
Click Time (ms) : 0.52 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 11.907 avg
Total System Input Lag (ms) : 12.427 avg


# Test3 calculated my self
Total System Input Lag (ms) : 2.1827280773603  stdev
Display Latency (ms) : 2.18330055536349  stdev
Click Time (ms) : 0.295324786797468   stdev


# Test4 Reported avgs
Click Time (ms) : 0.476 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 12.503 avg
Total System Input Lag (ms) : 12.979 avg


# Test4 calculated my self
Total System Input Lag (ms) : 2.25558437911623  stdev
Display Latency (ms) : 2.25556672051772  stdev
Click Time (ms) : 0.283919998690768  stdev

> [!NOTE]
> I will explain the results of test 5 and why it looks different then the rest.


# Test5 Reported avgs
Click Time (ms) : 0.499 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 12.384 avg
Total System Input Lag (ms) : 12.882 avg



# Test5 calculated my self
Total System Input Lag (ms) : 3.04697581912349  stdev
Display Latency (ms) : 3.04594792389012  stdev
Click Time (ms) : 0.259466134883755 stdev


# Test6 Reported avgs
Click Time (ms) : 0.494 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 12.225 avg
Total System Input Lag (ms) : 12.719 avg


# Test6 calculated my self
Total System Input Lag (ms) : 2.20516061787029 stdev
Display Latency (ms) : 2.14360938888623 stdev
Click Time (ms) : 0.283025089190183 stdev


# Test7 Reported avgs
Click Time (ms) : 0.535 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 11.898 avg
Total System Input Lag (ms) : 12.433 avg


# Test7 calculated my self
Total System Input Lag (ms) : 2.38427259159059  stdev
Display Latency (ms) : 2.31404052318219  stdev
Click Time (ms) : 0.295918780830965  stdev


# Test8 Reported avgs
Click Time (ms) : 0.531 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 11.988 avg
Total System Input Lag (ms) : 12.519 avg


# Test8 calculated my self
Total System Input Lag (ms) : 2.44709452538344  stdev
Display Latency (ms) : 2.42831618770595 stdev
Click Time (ms) : 0.289217908131288  stdev


# Test9 Reported avgs
Click Time (ms) : 0.532 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 12.089 avg
Total System Input Lag (ms) : 12.621 avg


# Test9 calculated my self
Total System Input Lag (ms) : 2.33591655489106 stdev
Display Latency (ms) : 2.38349832552443  stdev
Click Time (ms) : 0.291661149038719  stdev


# Test10 Reported avgs
Click Time (ms) : 0.517 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 12.058 avg
Total System Input Lag (ms) : 12.575 avg


# Test10 calculated my self
Total System Input Lag (ms) : 2.31509553305511  stdev
Display Latency (ms) : 2.26721878683416  stdev
Click Time (ms) : 0.285038919192705 stdev


when we look at the data just for example lets compare test 1 to test 2. Specifically we will compare the standard devation differences in microseconds of The total system Input Lag (End-2-End). But first lets quickly explain standard deviation simply. The Standard deviation allows us to compare variance in a set of data while still keeping it in MS. We see a 54.3841129 µs difference in consistency. But wait the number is so small why does it matter. Well... test 1 vs test 3 has a difference of 216.514923 microseconds 😏 Now what just happened, When we look at test 1 vs test 2 we see the difference between them is 54.3841129 µs. Why when I compared test 1 to 3 we saw a 216.514923 µs difference. Its clear that your pc is consistently adapting , sending events, changing frequencies, running background apps, etc. Do you think they are consistently causing a specific amount of jitter? Heck no, think of a computer as a human, things are always going on internally which like a computer is not static. This explains why jitter is not the same every single test in fact no test is even close to the same. Still don't believe me okay let's compare test 2 to test 3. It has a 162.13081 µs difference. You see it is consistently changing and you see it's not because the first test is different because you just started the game for the first time. (knew you were thinking about that) Now let's talk about test 5 as I noted above something was strange about it. Test 5 had a much bigger difference than all the tests. Test 2 vs 5 had a 702.116932 µs difference. Unlike the other tests, it had a higher max latency in the CSV file (you can find this in the repo). First I need to explain how and why I point this out. During the tweaked testing there was an outlier of 62.118 ms I thought it was an issue with me putting on the tool to my display and me accidently moving the CIP Device when putting it on as it was the second test that had the outlier. I also thought that because no number got even close to let alone 20 in the test. But then I looked at Stock on test 6 It was far down in the test and not one of the first. This time was it a 30.642 ms value which is closer to the other values. After all the tests I looked at I concluded that latency is just that strange because of the natural dynamics of the computer. In my final conclusion with all the tests I both of those in a section where I exclude it. So if you believe it's not good or ruins the test, you can find them removed. But it seems to ruin the data when removed and give lower values in variance then all tests (we compared above) which leads me to believe it's just a part of the data. Heres pictures of the outlier in the sets.



![30outlierFragementStock](https://github.com/user-attachments/assets/15d356ea-140d-413a-bac5-055351f57188)


![60outlierFragementTweaked](https://github.com/user-attachments/assets/2ed248e8-e908-4162-8eaf-bccabe1d957c)


Now I will show Tweaked data

# Test1 Reported avgs
Click Time (ms) : 0.484 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 11.929 avg
Total System Input Lag (ms) : 12.413 avg


# Test1 calculated my self
Total System Input Lag (ms) : 2.25142271381068 stdev
Display Latency (ms) : 2.27954781853106 stdev
Click Time (ms) : 0.279979486081146  stdev


> [!NOTE]
> Heres the test with that huge outlier of 62.118.

# Test2 Reported avgs
Click Time (ms) : 0.534  avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 12.282  avg
Total System Input Lag (ms) : 12.816 avg


# Test2 calculated my self
Total System Input Lag (ms) : 5.54903155786683  stdev
Display Latency (ms) : 5.54122592482016 stdev
Click Time (ms) : 0.282391066867323 stdev



# Test3 Reported avgs
Click Time (ms) : 0.535  avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 11.996  avg
Total System Input Lag (ms) : 12.532 avg


# Test3 calculated my self
Total System Input Lag (ms) : 2.24737288208057   stdev
Display Latency (ms) : 2.26210387538466  stdev
Click Time (ms) : 0.298888081482894 stdev


# Test4 Reported avgs
Click Time (ms) : 0.532 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 11.854  avg
Total System Input Lag (ms) : 12.386 avg


# Test4 calculated my self
Total System Input Lag (ms) : 2.36293977598869  stdev
Display Latency (ms) : 2.39052156990093  stdev
Click Time (ms) : 0.286543986962991  stdev


# Test5 Reported avgs
Click Time (ms) : 0.482 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 12.074  avg
Total System Input Lag (ms) : 12.555 avg


# Test5 calculated my self
Total System Input Lag (ms) : 2.32263219532225  stdev
Display Latency (ms) : 2.26883118968176  stdev
Click Time (ms) : 0.322384658099262  stdev


# Test6 Reported avgs
Click Time (ms) : 0.521 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 11.866  avg
Total System Input Lag (ms) : 12.388 avg


# Test6 calculated my self
Total System Input Lag (ms) : 2.55132784991926 stdev
Display Latency (ms) : 2.53142688261958 stdev
Click Time (ms) : 0.298759214474389  stdev




# Test7 Reported avgs
Click Time (ms) : 0.554 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 12.516  avg
Total System Input Lag (ms) : 13.07 avg


# Test7 calculated my self
Total System Input Lag (ms) : 2.6837088605288  stdev
Display Latency (ms) : 2.64562063719642 stdev
Click Time (ms) : 0.295337984093623 stdev



# Test8 Reported avgs
Click Time (ms) : 0.495  avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 11.504  avg
Total System Input Lag (ms) : 11.999 avg


# Test8 calculated my self
Total System Input Lag (ms) : 2.11541848616678  stdev
Display Latency (ms) : 2.14749891979136  stdev
Click Time (ms) : 0.29695309206824  stdev


# Test9 Reported avgs
Click Time (ms) : 0.498 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 11.547  avg
Total System Input Lag (ms) : 12.045 avg


# Test9 calculated my self
Total System Input Lag (ms) : 2.08570316653374  stdev
Display Latency (ms) : 2.05843741177181  stdev
Click Time (ms) : 0.291981275171037 stdev


# Test10 Reported avgs
Click Time (ms) : 0.479 avg
Processing latency (ms) : 0 avg
Display Latency (ms) : 11.931  avg
Total System Input Lag (ms) : 12.41 avg


# Test10 calculated my self
Total System Input Lag (ms) : 2.26193839335945  stdev
Display Latency (ms) : 2.25823394615251  stdev
Click Time (ms) : 0.256073451426056 stdev


You know the routine let's start with test 1 vs 3 as test 2 is one with a very different result causing a big jump. Test 1 vs 3 results in a difference of 4.04983173 μs already looks like a much lower variance but as we said latency jitter is really inconsistent even tweaked as you will see. Here is test 1 vs 4 with 111.517062 μs. As you can see this data is extremely unreliable. Okay now tests do 3 vs 4 this gives us 115.566894 μs difference. As you can see if you were to compare 2 test it can both appear inconsistent and consistent because of jitter. Let me show the huge difference of test 1 vs 2 due to one of the tests being 62.118. The difference ends up being 3297.60884 μs which is 3.29760884405615 ms difference !!! You see with the outlier its even huger.


So after all of this, I surely hope you are starting to get an idea of the problem here.
The main problems summarized.
1. Jitter is inconsistent
2. When testing tweaks that make a microsecond difference they will easily blend in because of jitter. The inconsistent amount of jitter means that even a millisecond could not be tested.
3. When comparing stock to tweaked it would be inaccurate due to the jitter always changing.



Lets show 999 samples vs 999 samples now (honestly an individual 100 better showcases the variance) I will show 998 vs 998 to show if you exclude both outliers from stock and tweaked configurations. I put this in a file to ensure the samples were exactly 999 or 998. I deleted the end of the datasets each time instead of deleting random parts to remain consistent.

Stock vs Tweaked 

# 999 samples tweaked
Total System Input Lag (ms) : 12.4615045045045 avg
Total System Input Lag (ms) : 2.82409992856889 stdev
Display Latency (ms) : 11.9500940940941 avg
Display Latency (ms) : 2.81719078142625 stdev
Click Time (ms) : 0.511408408408408 avg
Click Time (ms) : 0.291183204678331 stdev


---------------------------------------------------
# 998 samples Tweaked (excluding 62.118 outlier)
Total System Input Lag (ms) : 12.411748496994 avg
Total System Input Lag (ms) : 2.34688617021802 stdev
Display Latency (ms) : 11.9005561122244 avg
Display Latency (ms) : 2.34318325652919 stdev
Click Time (ms) : 0.511190380761523 avg
Click Time (ms) : 0.291247601404074 stdev



------------------------------------------
# 999 samples Stock
Total System Input Lag (ms) : 12.709015015015 avg
Total System Input Lag (ms) : 2.40129656167851 stdev
Display Latency (ms) : 12.1976936936937 avg
Display Latency (ms) : 2.38361185708595 stdev
Click Time (ms) : 0.511408408408408 avg
Click Time (ms) : 0.291183204678331 stdev



------------------------------------------
# 998 samples Stock Excluding outlier
Total System Input Lag (ms) : 12.6910460921844 avg
Total System Input Lag (ms) : 2.33433629060439 stdev
Display Latency (ms) : 12.1792845691383 avg
Display Latency (ms) : 2.31266245701846 stdev
Click Time (ms) : 0.511761523046092 avg
Click Time (ms) : 0.285610141102494 stdev

You can always compare the other latency types. I just look at the total. If you were to look closely at the outlier pictures on top they don't affect the click latency. Im not fully sure what click latency means as its auto firing. Im not the one clicking. Id ask Andrew the creator of the OSLTT CS to understand what it is.
By the way I dont use 1000 samples because test 6 for stock was missing a sample (most likely a bug). If you look at these you can conclude that the tweaked configuration is way better even excluding the outlier. I'm simply going to let you calculate this because it doesn't really matter because we know how inconsistent the data is.

Now heres the stock data

# 5 tests 500 samples
Total System Input Lag (ms) : 12.839446 avg
Total System Input Lag (ms) : 2.46461056346496 stdev
Display Latency (ms) : 2.4568279754688 stdev
Display Latency (ms) : 12.337934 avg
Click Time (ms) : 0.501512 avg 
Click Time (ms) : 0.283325531093014 stdev
-----------------------------------------------
# Another 5 Tests 500 samples
Total System Input Lag (ms) : 12.573468 avg
Total System Input Lag (ms) : 2.33148066368698 stdev
Display Latency (ms) : 2.3005500830503 stdev                         
Display Latency (ms) : 12.050748502994 avg
Click Time (ms) : 0.521758 avg
Click Time (ms) : 0.288250356412519 stdev

------------------------------------------------

# 5 tests (30 outlier excluded) 499 samples
Total System Input Lag (ms) : 12.8229879227053 avg 
Total System Input Lag (ms) : 2.32109805615671 stdev
Display Latency (ms) : 12.3194782608696 avg
Display Latency (ms) : 2.30972798064244 stdev
Click Time (ms) : 0.503509661835749 avg
Click Time (ms) : 0.289133578642597 stdev
-----------------------------------------------------------


# Another 5 Tests 499 samples (for the outlier excluded test to get an accurate stdev)
Total System Input Lag (ms) : 12.0571723446894  avg
Total System Input Lag (ms) :  2.30181933333831 stdev
Display Latency (ms) : 2.30181933333831 stdev                         
Display Latency (ms) : 12.0571723446894 avg
Click Time (ms) : 0.521150300601202 avg
Click Time (ms) : 0.288218826279961 stdev


and heres the tweaked data

# 5 vs 5 tests  

# 499 samples 

Total System Input Lag (ms) : 12.5463386773547  avg
Total System Input Lag (ms) : 3.21268410838166 stdev
Display Latency (ms) : 3.21294184309526 stdev                         
Display Latency (ms) : 12.031993987976 avg
Click Time (ms) : 0.514342685370742 avg
Click Time (ms) : 0.293859166336808 stdev

# Another 499 samples 

Total System Input Lag (ms) : 12.37684  avg
Total System Input Lag (ms) : 2.37403588835519 stdev
Display Latency (ms) : 2.35741767747001 stdev                         
Display Latency (ms) : 11.868358 avg
Click Time (ms) : 0.50848 avg
Click Time (ms) : 0.288752415600338 stdev


# 498 samples (outlier excluded)

Total System Input Lag (ms) : 12.446797188755  avg
Total System Input Lag (ms) : 2.32116621824211 stdev
Display Latency (ms) : 2.33072635514022 stdev                         
Display Latency (ms) : 11.9328835341365 avg
Click Time (ms) : 0.513439759036145 avg
Click Time (ms) : 0.293460929749222 stdev


# Another 498 samples 

Total System Input Lag (ms) : 12.3889578313253  avg
Total System Input Lag (ms) : 2.37103620477101 stdev
Display Latency (ms) : 2.35239021771009 stdev                         
Display Latency (ms) : 11.8818995983936 avg
Click Time (ms) : 0.507377510040161 avg
Click Time (ms) : 0.288872139073017 stdev



Hope this helps you learn about latency. If you liked this information consider following.



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


# Game

## Counter strike 2
## Lowest Settings 1440p
## controlled testing environment 
## Latency flash was used


