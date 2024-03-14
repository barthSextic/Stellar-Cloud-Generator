# Stellar Cloud Generator

A new firmware hack for the Qu-Bit Nebulae V2

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)

## Installation

Simply download the .instr file and place in the root folder of the flash drive you boot the Nebulae with.

Make sure to have some audio files in there!

## Usage

There are three main components. A looper, a reverb, and a filter.

Note: Both the inputs, and the sample are simultaneously sent through the system. Density_Alt controls the volume of the inputs, and Start_Alt controls the sample volume. 

If you run into trouble, Source mutes everything.


__Looper__

Start       - Sample Start
Size        - Sample End
Pitch       - Sample Pitch
Speed       - Sample Speed

Start_Alt   - Sample Volume

__Reverb__

Density     - Feedback
Overlap     - Dry / Wet

__Filter__

Blend       - Filter Cutoff
Window      - Filter Resonance

The Reset / Freeze Buttons are for selecting filter types

Reset, Freeze   -> 00 - Low Pass
                -> 01 - Band Pass
                -> 10 - High Pass
                -> 11 - Phaser

Note: the resonance control for the phaser is in the range (-1, 1), while all other types are (0, 1).

Record      -   'Off'   -> Filtering is applied before the delay
                'On'    -> Filtering is applied after the delay

Record_Alt  -   'Off'   -> Filtering is not applied to the dry signal
                'On'    -> Filtering is apllied to dry signal