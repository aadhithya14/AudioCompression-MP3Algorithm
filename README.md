# AudioCompression-MP3Algorithm

This Project contains a MATLAB demo that demonstrates the compression of an input audio signal in a stage wise manner as in MP3 algorithm. The MDCT gets applied to the blocked audio signal via polyphase decomposition matrices. The resulting coefficients get quantized by computing the auditory masking threshold and scaling such that the quantization error stays below. The quantized coefficients get then stored using Huffman coding, resulting in a binary file that can be decoded using the Huffman table and inverse scaling coefficients. The size of the original wave file  is about 7 times the compressed signal. This shows that compression of 7 times has occurred.

The main script `audio_coder_demo.m` calls all successive steps on an example file and produces the decoded output wave. Original and decoded wave files can be found in './data'.

An example masking threshold for one spectral frame and an example of original and decoded waveforms are added in the images folder.


