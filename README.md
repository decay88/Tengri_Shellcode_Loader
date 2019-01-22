# Tengri Shellcode Loader

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Tengri Shellcode Loader is a Cobalt Strike and x86 shellcode Loader builder for use on Red Team and Adversary Simulation engagements.

## Current Features:

  - Generate a loader from either DNS or HTTPS shellcode
  - Generate a loader that checks HTTPS connectivity and based on reponse either injects HTTPS or DNS shellcode into memory
  - Add Registry Entry to run loader on Start Up
  - AV Bypass - i've currently only test it with Symantec and one or two others, this needs further validation.

## Future Features:

  - Generate a loader that checks both HTTPS and DNS connectivity and if both fails runs EvilPostman SMTP agent
  - Generate an InstallUtil Function to evade application whitelisting
  - Add Sandbox detection techniques
  - Port to earlier versions of the .NET framework


## Requirements:

The loader and loader generator require .NET framework v4 to be installed on both the generator's and victim's machine.

You can download .NET framework v4 from [here](https://www.microsoft.com/en-gb/download/details.aspx?id=17851)

### GUI

It is a GUI application and fairly self explanatory. To run is just run the Tengri_SB.exe in the same folder as the rest of the repo.

The folder structure MUST be maintained for it to work and generated loaders are output into the FinishedLoader folder.

You will need to feed it either Metasploit and Cobalt Strike raw (.bin) x86 shellcode.

The GUI looks like this:

![Alt text](/images/loader_gui_prview.PNG)


## License 

This was developed by me on partly my own time and partly on KPMG's and while it does not contain any KPMG code currently, best not to share it with anyone outside the team. :)
