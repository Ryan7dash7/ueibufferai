# ueibufferai

MLDATA = UEIBUFFERAI(N,F,CH1,G1,W1,CH2,G2,W2,CH3,G3,W3,...) acquires N data points at a frequency of F Hz from the channels defined by the (CH,G,W) triples. The data are acquired by a UEI DNx-AI-201 layer installed in a PowerDNA Cube and saved to an N-by-C matrix, where C is the number of channels. CH is a string used to select which channels to use within a session. For example, the string '0:3' or '0,1,2,3' selects analog input lines 0, 1, 2, and 3. G specifies the gain applied on each channel and can be 1/10/100/1000 for the DNx-AI-201-16 or 1/2/5/10 for the DNx-AI-201-100/-801. W specifies how the inputs are wired and can be either 'SingleEnded' or 'Differential'.

Depending on what IP address the PowerDNA Cube is configured to use, you may need to edit the IP address in this function.

This function is based on bufferai_dotnet.m. See C:\Program Files (x86)\UEI\Framework\DotNet\matlab_examples for other examples.

Version 2017.03.23  
Copyright 2017 Ryan McGowan
