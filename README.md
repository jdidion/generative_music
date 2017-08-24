This repository contains projects associated with computer-generated music.

# Projects

## Neural network-generated video game music

This project starts from the biaxial rnn for music composition created by Daniel Johnson (https://github.com/hexahedria/biaxial-rnn-music-composition).

The first part of the project involves:

1. Getting the neural network running on a local cluster with GPUs
2. Training the network on [video game music](http://vgmusic.com)
3. Generating some pieces and seeing if they're any good

Next steps are:

1. Classify pieces according to mood. There are several classification systems; this [paper](http://hpac.rwth-aachen.de/teaching/sem-mus-15/reports/Napiorkowski.pdf) provides a good review. I am most attracted to Hevner's adjective cycle, which defines 8 moods that are described by different sets of adjectives. Reasonable labels for these sets are:
    1. Sacred/spiritual
    2. Sad/dark
    3. Dreamy/sentimental
    4. Tranquil/soothing
    5. Light/playful
    6. Happy/joyful
    7. Dramatic/passionate
    8. Majestic/martial
2. Train the network separately on the sets of music belonging to each mood category; score the results (using either a binary or continuous scale). Initially, this will be a subjective scoring done by hand, but it would be interesting to crowd-source this.

# Software

* python library for generating music algorithmically https://github.com/ideoforms/isobar
* bytebeats: http://royal-paw.com/2012/01/bytebeats-in-c-and-python-generative-symphonies-from-extremely-small-programs/

# Music

* Video game music: http://www.vgmusic.com/

# See also

* https://deepmind.com/blog/wavenet-generative-model-raw-audio/
* https://aiexperiments.withgoogle.com/ai-duet
* DeepBach: https://arxiv.org/abs/1612.01010
* https://highnoongmt.wordpress.com/2015/05/22/lisls-stis-recurrent-neural-networks-for-folk-music-generation/
