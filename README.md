﻿# BDSTL Bringing Dead Switches to Life
A Seattle VR Hackathon Project, September 16-18, 2016

## Inspiration
The Museum of Flight in Seattle has a few "sit in cockpit" exhibits. You can climb into an actual jet cockpit, settle into the seat, grab the stick, turn some knobs ..... and nothing happens.  What if you wore an AR headset that could "paint over" the gauges and make them come to life?  What i you could paint over the windshield to render the simulated world running past you, pitching and rolling as yank and bank on the stick?  What if this could be done without making any physical changes to the exhibit?

And what if this technology where available to every exhibitor for every museum and tradeshow?

## Operating Concept
An AR System would track hand/finger position, and render graphics to guages, windshields, portholes, etc; to show how the (simulated) vehicle reacts to the switches and wheel. Sounds would include engine noise, wind/water/ground effects, etc.

Perhaps an AI/Machine Learning system could watch your hands and be ‘trained’ on how to react to manipulations of the physical switches.  Imagine climbing into a real airplane, grabbing the stick and moving it forward and back.  At the same time, someone is operating a USB joystick in unison with your motions.  The AI/Machine Learning System watches (with a couple strategically placed webcams) and learns that “This Motion” means “That USB axis”  Simlar with switches.  “This physical switch” means “that keyboard press”  Hit the switch and keyboard in unison until the AI gets it.  With an AI like that, BDSTL could be "trained" to work with any exhibit, control panel, or vehicle anywhere.

## What Has Been Built So Far
The first iteration consists of a Microsoft HoloLens App, a physticals slider switch, and "holographic twin" of the slider switch, rendered in glowing wireframe.  The user begins by placing the phystical slider switch on a work surface such as a desk.  The next step is to launch the HoloLens App, which will render the holograpic twin floating in the air, about a meter away from the user. The user grabs the slider with the standard HoloLens "pinch" gesture, then places it over its phystical twin so that they correleate. The slider button is a seprate object, which must also be placed to correlate with its physical twin.  I was hoping the button could be configured to follow the users hand/fingers rather than gaze. In practice, this doesn't work very well, and the user needs to stare at the slide button while moving it.

which interacts with a simple slider switch.  The slider siwtch has a "physical twin" which can be placed on any surface.  When the App is started, the "holgraphic twin" is floating in the air, about a meter away from the user. 

## How I built it
This project is built on the Holgrams 101e tutorial materials at [https://developer.microsoft.com/en-us/windows/holographic/holograms_101e] . That's why the project is called Origami and lives under a folder called HolographicAcademy-Holograms-101
