⚠️ *Warning: This website may not function properly on Safari. For the best experience, please use Google Chrome.*

[`arXiv`](https://arxiv.org/abs/2407.14358): Stable Audio Open paper

[`HuggingFace`](https://huggingface.co/stabilityai/stable-audio-open-1.0): model weights

[`stable-audio-tools`](https://github.com/Stability-AI/stable-audio-tools): code to reproduce Stable Audio

[`stable-audio-metrics`](https://github.com/Stability-AI/stable-audio-metrics): code to evaluate Stable Audio

Stable Audio Open generates variable-length (up to 47s) stereo audio at 44.1kHz from text prompts. It comprises three components: an autoencoder that compresses waveforms into a manageable sequence length, a T5-based text embedding for text conditioning, and a transformer-based diffusion (DiT) model that operates in the latent space of the autoencoder.

## Autoencoder reconstructions

This comparison is useful to evaluate the audio fidelity capabilities of the autoencoder. On the left, we have the ground truth recording. On the right, we take the ground truth recording and end pass it through the any of those autoencoders or neural audio codecs. 

| Ground truth | Stable Audio Open | Stable Audio 2.0 | DAC | 
| ------------ | ----------------- | ---------------- | --- |
| <audio controls preload=False><source src="audio/3112.mp3" type="audio/mpeg">Audio not supported by your browser.</audio> | <audio controls preload=False><source src="audio/3112_sdd_sao.mp3" type="audio/mpeg">Audio not supported by your browser.</audio> | <audio controls preload=False><source src="audio/3112_sdd_sa2.mp3" type="audio/mpeg">Audio not supported by your browser.</audio> | <audio controls preload=False><source src="audio/3112_sdd_dac.mp3" type="audio/mpeg">Audio not supported by your browser.</audio> |
| <audio controls preload=False><source src="audio/4883.mp3" type="audio/mpeg">Audio not supported by your browser.</audio> | <audio controls preload=False><source src="audio/4883_sdd_sao.mp3" type="audio/mpeg">Audio not supported by your browser.</audio> | <audio controls preload=False><source src="audio/4883_sdd_sa2.mp3" type="audio/mpeg">Audio not supported by your browser.</audio> | <audio controls preload=False><source src="audio/4883_sdd_dac.mp3" type="audio/mpeg">Audio not supported by your browser.</audio> |
