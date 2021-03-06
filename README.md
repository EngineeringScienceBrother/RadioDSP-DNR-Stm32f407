# RadioDSP-DNR-Stm32f407

 THE RADIO DSP - DNR - PROJECT - Giuseppe Callipo - IK8YFW
 
This is an open source project that define a simple platform to make an
Audio DSP Processor for shortwave radio receiver with Digital Noise Reduction capabilities based on Spectral Subtraction. 

The system uses the good performances offered by the stm32f4 processor based on the CortexM4 specification, thanks to DSP extensions it is possible to process 256-element FFT real time (bin) ensuring a good response on the DNR functionalities, filtering and visualization of the audio signal.
Four filter elements have been implemented, currently fixed and implemented with Fir, with the following characteristics:
 
 * Filter 0: passes through (> 16kHz)
 * Filter 1: low pass for AM (<6kHz)
 * Filter 2: low pass for SSB (<3kHz)
 * Filter 3: bandpass for CW (500 Hz)
 
The display of the spectrum of the signal received in 8kHz and one is also implemented
secondary display to Waterfall with 3kHz zoom.

First Commit 31.12.2018
*********************************************************************************************************************
Update 25.01.2019
First version completed, final functions:

 * DNR with two stage (Spectral Subtraction + Adaptative Lms filters)
 * BPF / LPF filters (12, 6, 3, 0.5 kHz)
 * Spectrum and Waterfall signal realtime display
 * Morse CW decoder
 
 Added simple schematic (temporary hand writted) and the Help document to upload the firmware. 

**********************************************************************************************************************
Some videos of working prototipe:

Link1:(40 mt ssb)
https://youtu.be/YvctFP2eqpk

Link2:(40 mt ssb)
https://youtu.be/HLHY--rRiw8

Link3:(40 mt AM broadcasting)
https://youtu.be/vCnF3_ZGBCg

Link4:(20 mt ssb)
https://youtu.be/6EdBPZAnyo4

Link5:(waterfall)
https://youtu.be/ByIudrHRiHA

Link6: (Radio china int. AM)
https://youtu.be/mXqoe8ZU1xU

Link7: (Test decoder CW)
https://youtu.be/tha96osoO_M

************************************************************************************************************
Update 23.03.2019
A box for this project could be download from thingieverse as 3d Printed project.
Look here: https://www.thingiverse.com/thing:3506317

************************************************************************************************************


The project is work in progress and may be subject to change without notice.

  The RadioDSP openSource software is released under the license:
             Common Creative - Attribution 3.0
            
Vy 73 de Giuseppe Callipo - IK8YFW
