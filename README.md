# Tunefish Synthesizer

Tunefish v4 was developed as a smaller replacement of Tunefish v3 with roughly the same power. It was developed for our intro Turtles all the way down which forced us to rethink how to most effectively produce music in very tight machine code. Read more about it here. The result was totally worth it and some might argue it is even more powerful. To open it up to a broader range of people, it was also ported over to Linux and MacOS and it was given a new polished UI.

Check our website at https://tunefish-synth.com

## Screenshot

![Screenshot](https://github.com/paynebc/tunefish/blob/master/media/tunefish4.jpg)

### Compiling on Windows

TODO

### Compiling on Mac OS X

Install CMake and CLI C++ build tools, then run the following commands:
```
cmake -B .build
cmake --build .build
```

This should build a vst3 instrument plugin, and the "player" which has been modified to output a .wav file since realtime playback is implemented for Windows only.

### Compiling on Linux

TODO

The following additional packages are needed on Ubuntu 20.04 to compile:

* libgl1-mesa-dev
* libfreetype6-dev
* libasound2-dev
* libxrandr-dev
* libxinerama-dev
* libxcursor-dev
* libcurl4-openssl-dev

Install them using:

```
sudo apt-get install libgl1-mesa-dev libfreetype6-dev libasound2-dev libxrandr-dev libxinerama-dev libxcursor-dev libcurl4-openssl-dev
```

run make in directory
/src/tunefish4/Builds/LinuxMakefile

### Running

Copy the tunefish4.dll/.so/.component/vst (depending on platform) to your desired plugins directory. Run your sequencer.
