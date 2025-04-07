# attachment_emo_clf
This is the code used to train the emotion-based attachment classifier described in the paper [**Emotion Recognition for Multimodal Recognition of Attachment in School-Age Children**](https://dl.acm.org/doi/10.1145/3678957.3685747).

There are 4 files used to train the attachment classifiers that are based on audio, text, multimodal combination 1 (MC1) and multimodal combination 2 (MC2).

There are also 2 files used to extract emotions from both audio and text: **Attachment Emotion Cleaned Audio Extractor** and **Attachment Emotion Cleaned Text Extractor**. These files extract embeddings representing emotions from both modalities and store them in separate files. These files are then used as input to the attachment classifiers.

Two emotion classifiers were used, one for [text](https://huggingface.co/bhadresh-savani/bert-base-uncased-emotion) and the other for [audio](https://huggingface.co/AreejB/wav2vec2-xlsr-english-speech-emotion-recognition).

The "Attachment_NN_Audio_Emo_Cleaned.ipynb" file has additional comments to explain the code.

The trained model weights have been uploaded. As each experiment was repeated 10 times, there are 10 versions available for each model: Audio-based, Text-based, MC1, and MC2. Due to size limitations, some files have been divided into multiple parts.
