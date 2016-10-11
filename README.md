# mfcc_extractor
A Max based mfcc extractor to be used with wekinator

Sends to Wekinator using /wek/inputs on port 6448

Description:

A simple MFCC extractor that can be used to differentiate between different voices.


Requires:

* OpenSoundControl Max object in Max/MSP folder.
* Zsa.descriptors - http://www.e--j.com/index.php/download-zsa/


To run:

1) Open the patch in max and turn the sound on.
2) Select sound source.
3) Select the number of Mel Band(s). The default is 24.
4) Run Wekinator with 24 inputs. This will change depending on the number of Mel Band(s) you are working with.

This patch can take sound input from either the adc~ object (“microphone” i.e. whatever your input device may be) or from a sound file.

You may want to experiment with the number of Mel Band(s), but remember this will also change the number of inputs sent to Wekinator.
