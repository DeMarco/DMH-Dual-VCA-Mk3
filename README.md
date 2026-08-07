# DMH-Dual-VCA-Mk3
Version 3 of my stereo VCA in Kosmo format, now including voltage controlled panning and optional clipping and distortion!

<img width="651" height="869" alt="image" src="https://github.com/user-attachments/assets/8861be07-b561-4f47-b6e3-411e85839587" />

<img width="651" height="869" alt="image" src="https://github.com/user-attachments/assets/fed7a587-f414-4081-9bb1-c6e01b596919" />

<img width="651" height="869" alt="image" src="https://github.com/user-attachments/assets/5eecec60-ba61-4f71-9d5c-39fdc59ac0e1" />

## Features

- 2 channels, A and B
- 2 CV inputs per channel, each one with its own attenuverter knob
- Unipolar control voltage: 0V means VCA is fully closed (gain = 0), +10V means completely open (gain = 1)
- 1 offset knob per channel, useful to bias bipolar CV signals like those from LFOs
- The offset setting and attenuverted CV inputs of each channel are summed
- Toggle switches to select between pan/balanced/tremolo mode, and clipping/distortion
- Pan mode: output volue of both channels is halved. Pan CV signal will increase one channel's volume and decrease the other's simultaneously.
- Balanced mode: same as Pan mode, but both channels volume are biased with half the Pan CV signal amplitude, which preserves overall volume during panning.
- Tremolo mode: both channels duck in response to Pan CV.
- The Pan knob can be used to manually change panning when no Pan CV is plugged in. It becomes an attenuverter when Pan CV is used.
- Clip mode: 4v7 Zener diode pairs are applied to both channel outputs, effectively limiting output to about +/-5V.
- Distorted mode: 3v0 Zener diode pairs and 2x gain is applied to both channels output, effectively distorting and limiting output to +/-5V.
- LEDs indicate when the output levels pre-clipping/distortion peak above 5V, so you know that Clip mode is clipping the output when engaged.

Demo video: https://www.instagram.com/reel/DbrHDk0sg0o/?utm_source=ig_web_copy_link&igsh=MzRlODBiNWFlZA==

## Schematic and Gerbers

https://github.com/DeMarco/DMH-Dual-VCA-Mk3/blob/main/Schematic.pdf

https://github.com/DeMarco/DMH-Dual-VCA-Mk3/tree/main/Gerbers

https://github.com/DeMarco/DMH-Dual-VCA-Mk3/blob/main/DMH_Output_BoM.csv

Please note the plug-in VCA submodules are part of another Repo. You need to make 4 of these to assemble the complete module:

https://github.com/DeMarco/DMH-Submodules/tree/main/DMH_Submodule_VCA/Gerbers

## Assembly instructions

Use 11mm long pin headers on the Main PCB to ensure connection with the pin sockets on the Controls PCB.
Other than that, nothing special.
I recommend soldering components in order of height: start with resistors and diodes, then move on to IC sockets, capacitors, transistors and connectors.

### Main PCB

<img width="426" height="696" alt="image" src="https://github.com/user-attachments/assets/1e165583-19a7-46e5-913c-8396688c8d91" />
<img width="412" height="696" alt="image" src="https://github.com/user-attachments/assets/3ca2b1aa-054a-49d1-8ed9-beba8802cf90" />

### Controls PCB

<img width="527" height="797" alt="image" src="https://github.com/user-attachments/assets/e8e82e0c-a9f6-4f56-a9cb-09d3904c6845" />
<img width="515" height="756" alt="image" src="https://github.com/user-attachments/assets/e16723be-c8fe-4bd9-9e01-461693c154dd" />


### VCA Submodule Mk1

<img width="577" height="667" alt="image" src="https://github.com/user-attachments/assets/36cc7be1-583c-42f3-91a5-03bc689d66e7" />
<img width="542" height="657" alt="image" src="https://github.com/user-attachments/assets/5855f88c-2905-4e38-b24a-7be18a07f569" />


## Calibration

### Attenuverters pot center

t.b.w.

### VCAs symmetry

t.b.w

## Current consumption

+12V --> 38mA

-12V --> 38mA

## Dimensions

Height: 20cm

Width: 5cm

Depth: t.b.c.

## Font

For viewing/customizing in KiCad, I recommend downloading and installing the Nulshock font from Typodermic: https://typodermicfonts.com/nulshock/
