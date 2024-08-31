# plugdata guitar effects module

![image](https://github.com/user-attachments/assets/8e3b02c6-a629-4e8e-a50b-e8f1c44d0cfb)

How to use:
- Download the eguitar folder
- open module.pd using plug data
- use the sample audio to test it

Context:
The motivation for this project is to create modular effects to replace an old electric guitar pedalboard and with a laptop digital effects unit.

This is also an exercise for me to develop some experience in puredata,so the methodology may not result in the best/cleanest patches. My primary goal is to get something working first, then work on refinements for each module as I go. 

Effects
- audio input handler/gain
- compressor/limiter
- violin
- parametric eq
- overdrive
- chorus
- phaser
- delay (with modulated and time signature parameters)
- spectral delay 
- reverb
- convolution reverb
- output volume

Signal flow: guitar -> audio interface -> plugdata (laptop) -> mixer

Some of the features planned:
- DONE presets for each effect module (stored as individual text files)
- TODO Scene presets which trigger different combinations of module presets
- TODO Global Tap tempo delay with note value selection
- TODO Implement mobmuplat on an android phone mounted on a guitar to trigger effects live.

Acknowledgements:
The patches were made in plugdata, primarily using the following externals: ELSE and Audiolab, however any extra modules can be downloaded via the externals library.

Most effect modules are the patches of other pure data creators, with some subpatches copied over (e.g. the preset module from audiolabs is used in all modules with some modifications). 
Others are based on tutorials (e.g. maxmsp). In the future I hope to make a list of the works which I have learnt from as they have been invaluable.

It should work as long as you have a pc with PlugData, some externals and an USB audio interface. It can also work in Puredata vanilla, but some GUI elements wont scale to the same size. Sample rate and latency still needs to be tweak for individual setups.
