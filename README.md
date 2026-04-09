# Low-Noise Instrumentation PCB for Data Acquisition

## Overview
Designed and fabricated a PCB for a data acquisition system used in hardware-in-the-loop (HIL) testing. The goal was to improve signal integrity and measurement accuracy in sensor validation workflows.

## The Design Challenge
Mixed-signal systems often suffer from noise coupling between digital switching and sensitive analog measurements. Early prototypes showed inconsistent readings due to noise interference.

## Key Design Insight
Instead of adding more filtering components, I focused on solving the problem at the layout level.

I implemented a grounding and decoupling strategy that:

- Separated analog and digital return paths
- Minimized loop areas for sensitive signals
- Placed decoupling capacitors directly at IC power pins
- Controlled current return paths to reduce ground bounce

## Why This is Interesting
Most designs attempt to fix noise after it appears using filtering. This design prevents noise at the source through layout decisions, reducing complexity and cost.

## Results
- Reduced measured noise by ~15 dB  
- Achieved ±1% system accuracy  
- Improved repeatability in calibration and testing workflows  

## Visuals
(Add images here)

- PCB Layout (Top Layer)
- Ground Plane / Bottom Layer
- Schematic (Power + Analog Section)

## Takeaway
Small layout decisions in PCB design can have large system-level impacts. Thoughtful grounding and component placement can outperform more complex circuit-level fixes.
