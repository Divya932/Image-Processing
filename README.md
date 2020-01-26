# Image-Processing
### Ans 1. 
Channels are containers of a fixed type of objects or features that are extracted from image(s).

Ex: From a picture of many dogs, just the feature nose is used to extract out a part of the image. The collection of all these noses are a channel. 
Ex: Any picture or text in english can have at most 26 channels because we can separate it based on 26 different features called alphabets. 

A Kernel is also called a filter or an extractor which we use to extract features out of an image.

It is described as a small matrix (normally 3 X 3), which works as a filter on images to apply different effects like blurring, sharpening, outlining, etc., 

Ex: nose is a kernel in the above example.
Ex: An alphabet 'e' can also be considered as an extractor or a kernel in a text in English

 

### Ans 2. 
3X3 Kernels are an optimal choice because:

1. It has symmetry without which distortions across the layers can happen when using an even sized kernel.

2. Highly local features are extracted without much image overview.

3. It can capture small and complex features in the image.

4. If we want to use a 2X2 kernel we can simply substitute 0's at the edges of 3X3 matrix.

5. Two  3X3 kernels can be combined to give an effect of 5X5 kernels.

 

### Ans.3 

199X199 > 197X197 > 195X195 > 193X193>191X191 > 189X189 > 187X187 > 185X185 > 183X183 > 181X181 > 179X179 > 177X177 > 175X175 > 173X173>171X171 > 169X169 > 167X167 > 165X165 > 163X163 > 161X161 > 159X159 > 157X157 > 155X155 > 153X153>151X151 > 149X149 > 147X147 > 145X145 > 143X143 > 141X141 > 139X139 > 137X137 > 135X135 > 133X133>131X131 > 129X129 > 127X127 > 125X125 > 123X123 > 121X121 >
119X119 > 117X117 > 115X115 > 113X113>111X111 > 119X119 > 117X117 > 115X115 > 113X113 > 111X111 > 99X99 > 97X97 > 95X95 > 93X93>91X91 > 89X89 > 87X87 > 85X85 > 83X83 > 81X81 > 79X79 > 77X77 > 75X75 > 73X73>71X71 > 69X69 > 67X67 > 65X65 > 63X63 > 61X61 > 59X59 > 57X57 > 55X55 > 53X53>51X51 > 49X49 > 47X47 > 45X45 > 43X43 > 41X41 > 39X39 > 37X37 > 35X35 > 33X33>31X31 > 29X29 > 27X27 > 25X25 > 23X23 > 21X21 > 19X19 > 17X17 > 15X15 > 13X13>11X11 > 9X9 > 7X7 > 5X5 > 3X3 > 1X1

 
### Ans.4 

Kernels are initialized randomly. 

### Ans. 5

Training of a DNN means finding correct weights for each path(connections) between two layers.

An appropriate activation function is chosen(ex: sigmoid function), 

A certain number of middle or hidden layers(preferably large) are decided and kept,

Weights are initialized to the connections between layers,

And then the most important hyper parameter, learning rates are set.  Optimal choice is important else a smaller learning rate can take ages to converge, and larger learning rates can escalate the loss.

As a result of all these steps the kernel values we initialized randomly, are changed gradually based on the output received using previous kernel values, which improves accuracy consequently. When the model stops showing improvement in accuracy, the training is considered complete and the concurrent kernel values are the final values.

 
