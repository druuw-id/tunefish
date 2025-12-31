cmake_minimum_required(VERSION 3.22)
project(TUNEFISH_PLAYER VERSION 0.0.1)

add_executable(TuneFish4Player
    ../tunefish4/Source/runtime/array.cpp
    ../tunefish4/Source/runtime/random.cpp
    ../tunefish4/Source/runtime/runtime.cpp
    ../tunefish4/Source/runtime/simd.cpp

    ../tunefish4/Source/synth/tf4.cpp
    ../tunefish4/Source/synth/tf4fx.cpp
    # ../tunefish4/Source/synth/tfrecorder.cpp

    datastream.cpp
    main.cpp
    # tf4dx.cpp
    tf4player.cpp
    # threading.cpp
)
