# Text-to-video-generation-model
Damo-vilab Text-to-Videos model leverages a sophisticated multi-stage diffusion architecture to transform textual descriptions into corresponding video sequences. 

Exclusively designed for English input, the model comprises three integral sub-networks:<br>
1. Text feature extraction model
2. Text feature-to-video latent space diffusion model
3. Video latent space to video visual space model

The model employs a UNet3D structure for its diffusion process, generating videos iteratively through denoising from pure Gaussian noise video.
Also finds application across diverse scenarios, offering the ability to reason and generate videos based on arbitrary English text descriptions.

The generated output is made accessible through the provision of a save path for the resulting video file. Playback is facilitated through VLC media player, with the output saved in an MP4 format. Note that while VLC seamlessly supports playback, some other media players may not exhibit optimal performance for viewing the generated content. 

TEXT FEATURE EXTRACTION MODEL<br>
The initial stage employs advanced natural language processing (NLP) techniques to meticulously extract nuanced features from the input text, laying a robust foundation for subsequent video generation

LATENT SPACE DIFFFUSION MODEL<br>
The model's core strength lies in its multi-stage diffusion process, a unique approach that iteratively transforms text features into videos by denoising from pure Gaussian noise video. The incorporation of a UNet3D structure adds an extra layer of efficiency to this diffusion process.

VIDEO VISUAL SPACING MODEL<br>
The final stage elegantly translates the refined latent space into the video visual space, resulting in a coherent and visually compelling output that faithfully reflects the essence of the input text.<br>

GENERATION FROM VIDEOS TO TEXT<br>
The model tackles the intricate task of describing videos by proposing a multi-step approach that synergizes Natural Language Processing (NLP) and Computer Vision (CV) components, exemplifying a holistic understanding of both domains.
1. NLP PART: The user-provided text undergoes a meticulous journey, including segmentation into sentences, entity extraction, and engagement with a Named Entity Module, showcasing a nuanced understanding of textual nuances.
2. CV PART: The Computer Vision (CV) part encompasses the complete spectrum, from collecting text for video generation to model selection (e.g., CRAFT, TFGAN, GODIVA), dataset division, training, testing, and optimization. This approach ensures meaningful and contextually rich video creation.

![process](https://github.com/apekkshaa/text-to-video-generation-model/blob/main/Images/process.png)
