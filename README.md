# VoxCeleb v2 With Mel Spectrogram Features

## Summary
The aim of the project is to explore the effectiveness of Mel Spectrogram features in the Kaldi VoxCeleb v2 recipe. Mel Spectrogram features may show more success given the DNN architecture of the v2 recipe. 
After running the experiments, the MFCC model outperformed the Mel Spectrogram model, with an EER of 7.69% versus 12.79%.

Background on the recipe: https://youtu.be/UKMG8N40CiM

Summarization of the project: https://youtu.be/rsV9lbM1KXI

Results: [MFCCvsSpec.pdf](MFCCvsSpec.pdf)

## Tools Used
The [Kaldi Speech Recognition Toolkit](https://github.com/kaldi-asr/kaldi) was used for training and evaluating the models. All scripts were adapted from the Kaldi VoxCeleb v2 [run.sh](https://github.com/kaldi-asr/kaldi/blob/master/egs/voxceleb/v2/run.sh) file.

## Scripts
Both scripts train a lighter version of the VoxCeleb v2 recipe.

[run_mfcc.sh](run_mfcc.sh) trains and evaluates a model with MFCC features.

[run_spec.sh](run_spec.sh) trains and evaluates a model with Mel Spectrogram features.

## Data
The VoxCeleb1 data was obtained from https://mm.kaist.ac.kr/datasets/voxceleb/ 

The MUSAN data was obtained from https://www.openslr.org/17/ 

The RIR Noises data was obtained from https://www.openslr.org/28/ 

## How to Run
Clone and set up the Kaldi toolkit. Then, run either script in the `kaldi/egs/voxceleb/v2/` directory.

## Future Work

Future work includes training a model with a combination of MFCC and Spectrogram features.


