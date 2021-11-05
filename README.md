# scores-chimeres

**PUREDATA GENERATIVE SCORES V1 FOR CHIMERES ORCHESTRA.**

See data/params-generator-readme.txt for infos

**1 - HOW TO**

 1 open [install].pd patch
 2 from [install].pd,  click toggle "compozer" to open compozer patch
 3 click open [pd SAFRAN-5x6-JAM]
 4 pressing once "Start" toggle should launch a new gig

**2 - CLOCK AUTO**

check "clock" box from [install].pd on should launch a new gig every 15mn

**3 - ALIEN-EVENTS OSC-COMMANDS**
OSC listening to port 10000

use any other free OSC app or import the file data/Chimeres-Orchestra-v1.tosc on any remote pc/tab/smartphone with touchOSC app > https://hexler.net/touchosc). cf. data/Chimeres-O-touchOSC.gif

// prefixe messages :
/btn1 	Start
/btn2	Stop
/btn3 	Alien shot
/btn4 	Alien pingpong
/btn5	Replay same preset
//
/f1 	Alien length
/f2 	Alien speed
/f3 	Alien velocity
/f4 	LFO to Alien velocity (only works when a preset is playing)
//
see [osc-remote 10000].pd from install].pd patch if needed
//
**4 - AUDIO-SIMULATOR**

Open [robots-simulation.pd] from /abs folder.
This patch launch as much [synth-arm].pd as define in the conf.txt infos file (NB_ARMS * BN_CHIMERES)
[synth-arm].pd listen to [r CHIMERES] emitted frome [install].pd.
[robots-simulation.pd] play straigth to the pd dac~ main output.

reso-nance.org 2021 | contact@reso-nance.org 
 
