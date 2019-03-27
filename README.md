This project was made for Dr. Mark Albert's Computational Neuroscience class

The project creates varying receptive fields and analyzes how manipulation of properties of these filters can affect depth perception.


V1 Cortical Cells in the Occipital Lobe each contain their own receptive field (a visual stimulus that stimulates said neuron).
Receptive fields vary greatly from one another and often serve for different computational functions.
In this case, we're looking at a receptive fields ability to detect depth and thus percieve it.

A receptive field can be mathematically represented by a 2D Gabor Wavelet (A Gaussian Kernel Function modulated by a Sinusoidal Plane Wave)

Utilizing python, a 2D Gabor wavelet can be generated given paramaters for each eye.

The two filters can then be double convolved upon an autostereogram (a picture that has been filtered to have depth at 3 circular areas).

The result is an image showing where on the autostereogram the receptive fields were "stimulated"

Each pair of gabor wavelets (receptive fields) is then scored based on it's ability to detect depth in the CORRECT areas of the autostereogram.
(A filter would be discounted points for detecting depth where it shouldnt)

