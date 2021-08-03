The problem with piezo guitar pickups and piezoelectric crystals is that they are not well matched to typical audio inputs. By their nature they can generate a lot of signal, but they cannot drive a 50 kilohm typical line input. The pickup needs to work into a much higher impedance, typically 1 megohm or so.

So what to people do? They go and plug a piezoelectric disks output directly into the line input of their recorder, typical impedance 50k, or the plug-in-power mic input of their recorder, typical impedance about 7k, and they start to bitch and moan that this damn thing sounds tinny. Which is does ! But they don't understand why!

The reason why these devices often sound tinny is because the piezo sensor presents its signal through a series capacitance which is small, typically 15nF or less. When wired to a normal 50 kilohm line input this forms a high-pass filter, which eliminates the bass.

One of these can be used for a reverb plate, listening to the insides of a engine,recording the sound of vibrating things. 

Mechanics may even use one of these to discover trouble with bearings or other mechanisms not easily opened or stopped.
That includes engine Knocking (also knock, detonation, spark knock, pinging or pinking) in spark ignition internal combustion engines. 

They should also work nice with hydrophones. PZT-5H tubes is best for that. 

In case of a hydrophone it's possible to have the hydrophone attached with a long cable and the amplifier/buffer circuit close to the piezoelectric elements. 
It's of course extremely important that the circuit board and connections are absolutely waterproof. 

Commercial ones uses kerosene oil, so olive oil or sunflower oil is a great alternative as it will not pollute the environment if any leaks occurs.
Plant based oils is actually possible to use in high voltage transformers:
https://pdfs.semanticscholar.org/56b6/36870fac68b1bb6e343eee914002195b8a61.pdf
Silicone rubber, dielectric grease, epoxy is also useable if it is not harmful to the environment.

All PCB boards and components are easy to solder, one just needs basic skills and knowledge of the right direction to put in the diodes.

There may be components that has lower self noise,better common mode noise rejection and so on,
-but finding the best choice of components that handles from 0 to 48 volts DC power range, uses maximum 10 milliamperes total, minimum self noise, has 8 or 14 pins DIP package is not a easy task!
I think that these are ok SMD alternatives: LT6234,LT6231,
THT: NJM2122D

If you know components that is superior in regard to the intended voltage range, please fork the relevant GitHub page and make the changes you want.

Some PCB boards has SMD components, but Aisler and other companies offers SMD assembly.

PCB board for 48 volts phantom power, with balanced input and output using op amps, gain set with two resistors. It's the easiest to solder because it has no SMD components:
https://github.com/Supermagnum/double-gain

SMD adapter with LT6234 :
https://aisler.net/p/IXOHRKHO

With switches to set the gain:
https://github.com/Supermagnum/double-dip

SMD version, gain set with switches:
https://github.com/Supermagnum/balanced-smd

PCB board using ultra low self noise components, balanced input and output, 48 volt phantom power. It's a little harder to solder, because some of the solder points are quite close together:
https://github.com/Supermagnum/piezo-balanced

PCB board for 9V battery, mono audio out and single input. Easy to solder:
https://github.com/Supermagnum/piezo-9v

48 volt phantom power supply with mono headphone output. Has one SMD component:
https://github.com/Supermagnum/48power

All these links has links to Aisler, that offers PCB boards and components:
Just register and import the 
PCB and part list.

Made with: http://www.kicad.org/

KiCad uses an integrated environment for all of the stages of the design process: Schematic capture, PCB layout, Gerber file generation/visualization, and library editing.

KiCad is a cross-platform program, and of curse free!
