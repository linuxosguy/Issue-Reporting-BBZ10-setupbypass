# Issue-Reporting-BBZ10-setupbypass
The GitHub Issue Reporting page and Setup Guide for bypassing the Blackberry Z10 Setup on STL100-1 Z10 Devices.
<br> Based on OS Version: 10.3.02.2813

# Setup Guide
First, download the required files from the MEGA link, or you can click [here](https://mega.nz/folder/UI1jVYqA#n405DxKsOhgpazCgu9wwYQ), 
<br>The latest release is v1.0.
<br>You will also need [cfp.exe](https://mega.nz/file/cI8gkYaC#yACNSnrVI3aA6K7xkg6pY9Bw8Te5KagepWfJAp5X0AA), if you don't already have it.

## Step 1
Open a Command Prompt in the directory of where the files are stored.

## Step 2
**INFO: You will need [Blackberry Link.](https://mega.nz/file/BE9FwQYD#WwlrI75lKqsYiwhzgPWKLaTr3XBukg3r6Nj_kZXlBog)**
<br>Run command:
```batch
cfp load os.Signed
```
Then, once you see "Connecting to bootrom..."
<br> Connect your Z10 to your computer.
<br> Wait until the process has finished.

## Step 3
You might see:
```text
Writing  0x0002C8E2 [############## 100 ##############]
Error: Failed to load images.
Error: Security error.
```
This is normal, and expected.
<br> After you have gotten this error, run this command:
```batch
cfp load radio.signed
```
<br> Wait for the process to complete.
<br> This clears the software error flag and allows the system to boot properly.

## Step 4
After this, your Z10 should boot into a normal state. Instead of booting straight into setup, it will boot straight to the App Menu, and you will get no Complete Setup notification, and it will be in a fully-setup state.


## Credits
### Pablo Ferreira 
[Reddit: u/Confident-Guess2914](https://www.reddit.com/u/Confident-Guess2914)
<br>[Github: FerrieraPablo](https://github.com/FerreiraPablo)
<br> Code editor
<br> De-bloated image

### OS Guy
[GitHub: linuxosguy](https://github.com/linuxosguy)
<br>Code tester




