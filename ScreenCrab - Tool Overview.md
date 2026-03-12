# Screen Crab - Tool Overview

- This document holds a discription of the tool `Screen`, its uses, and what the tool does.

## Overview 

The Screen Crab is a stealthy wideo man-in-the-middle implant. It sits between HDMI devices such as a computer or monitor to quietly capture screenshots. This is a hardware based tool, meaning unlike software-based screen recorders it cannot be detected by task manager or antivirius. 

## How it Works: The Hardware

The Screen Crab sits physically between a source device and a monitor 
- Physical Setup: You plug the HDMI cabe from the computer into the "Input" port of the Screen Crab, and then run another HDMI cable from the "Output" port to the monitor.
- Passthrough: It provides a lag-free, 1080p video signal to the monitor, so the user has no idea thier feed is being viewed.
- The Data Collection: While passing the signal through, it silently cpatures screenshots or video and saves them to an onboard microSD card or streams them over Wi-Fi. 
