PushToOSC (via MAX)

This Max patch can be used to control your own OSC receiving software from your Ableton Push controller. If you want to use
it for visual programs, individual drum pads can for example activate different effects, the after touch can be used to
control any parameter of the effects. The way the after touch relates to the chosen parameter can be controlled by changing
the Wekinator learning algorithms.

Requirements:
Download the external objects for Max/MSP from CNMAT at:
http://cnmat.berkeley.edu/downloads

Run the Max patch:

Set the MIDI device name to Ableton Push User. PushToOSC sends by default to localhost, port 6448.

Open Wekinator or WekiInputHelper until the setup page. Press <Start listening> on port 6448 and hit the initialize button on
the max patch, this updates all input names for you inside Wekinator or WekiInputHelper to easily distinguish between them.
This step also sets the input number automatically to 129.

Wekinator is now receiving OSC data from all Drum Pads. On/Off information and aftertouch. Also Pitchbend information is sent
Multitouch is also supported.

input 1 - 64 drum pads on off
input 65 -128 AT drum pads (Aftertouch Information)
129 pitchbend information
