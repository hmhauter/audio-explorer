# Sound scene classifier for hearing aids
### Audio Explorers challenge 2023

##### Introduction
Modern hearing aids utilize many different algorithms for improving hearing comprehension and reducing ambient noise. In many situations, modern hearing aids are capable not only to attenuate unwanted noise but also sounds which could be of benefit for the hearing aid user. Often the amount of noise reduction, which is needed, will depend on the current sound environment. For example, babble background noise may prevent a hearing-impaired user from following a conversation. Another example is traffic noise. Even though traffic noise is annoying, it is important for the hearing-impaired listener to hear a vehicle approaching from behind in order navigate safely. It would thus be highly attractive to have the hearing aid automatically detect the nature of the sound environment and adjust the settings accordingly.

##### Challenge
Given a provided dataset, sound snippets should be classified into 5 different classes:
- 0: Other 
- 1: Music
- 2: Human voice
- 3: Engine sound
- 4: Alarm

The provided audio is transformed into the frequency domain using a Short-time Fourier transform (STFT) and is the converted into mel-frequency scale.
The dimensions of the dataset is (52890 x 32 x 96) corresponding to 52890 sound samples with 96 time frames each containing 32 frequency bands.

The limited memory and computational power of a hearing aid has to be taen into account. For example should the Machine Learning model have less than 500000 parameters. 