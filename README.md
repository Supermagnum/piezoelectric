The problem with piezo guitar pickups and piezoelectric crystals is that they are not well matched to typical audio inputs. By their nature they can generate a lot of signal, but they cannot drive a 50 kilohm typical line input. The pickup needs to work into a much higher impedance, typically 1 megohm or so.

So what to people do? They go and plug a piezoelectric disks output directly into the line input of their recorder, typical impedance 50k, or the plug-in-power mic input of their recorder, typical impedance about 7k, and they start to bitch and moan that this damn thing sounds tinny. Which is does ! But they don't understand why!

The reason why these devices often sound tinny is because the piezo sensor presents its signal through a series capacitance which is small, typically 15nF or less. When wired to a normal 50 kilohm line input this forms a high-pass filter, which eliminates the bass.

One of these can be used for a reverb plate, listening to the insides of a engine,recording the sound of vibrating things. 

Mechanics may even use one of these to discover trouble with bearings or other mechanisms not easily opened or stopped.

They should also work nice with hydrophones. PZT-5H tubes is best for that. 

In case of a hydrophone it's possible to have the hydrophone attached with a long cable and the amplifier/buffer circuit close to the piezoelectric elements. 
It's of course extremely important that the circuit board and connections are absolutely waterproof. 

PCB board for 48 volts phantom power, with balanced input and output using op amps, gain set with two resistors:
https://github.com/Supermagnum/double-gain

PCB board using ultra low self noise components, balanced input and output, 48 volt phantom power:
https://github.com/Supermagnum/piezo-balanced

PCB board for 9V battery, mono audio out and single input:
https://github.com/Supermagnum/piezo-9v

48 volt phantom power supply with mono headphone output:
https://github.com/Supermagnum/48power

Made with: http://www.kicad.org/

KiCad uses an integrated environment for all of the stages of the design process: Schematic capture, PCB layout, Gerber file generation/visualization, and library editing.

KiCad is a cross-platform program, and of curse free!
