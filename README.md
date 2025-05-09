## 🌍 Multilingual Emotion Detection in Voice

This project combines **speech transcription** and **emotion recognition** from audio files using Python libraries such as `whisper`, `librosa`, and `scikit-learn`.

### 🧩 Key Components

* 🎤 **Speech Recognition**: Using OpenAI Whisper to transcribe voice from `.mp4` audio files
* 😃 **Emotion Detection**: Extracting audio features (MFCC + pitch) and classifying emotions using a Support Vector Machine (SVM)
* 🌐 **Multilingual Support**: Whisper automatically detects the spoken language

### 📦 Dependencies

Install the required packages:

```bash
pip install openai-whisper librosa scikit-learn moviepy
```

### 🛠️ How It Works

1. **Convert Audio**: Convert `.mp4` files to `.wav` using `moviepy`
2. **Transcribe Speech**: Transcribe speech using OpenAI's Whisper model
3. **Extract Features**: Use `librosa` to extract MFCC and pitch features
4. **Classify Emotion**: Predict emotional tone using an SVM classifier
5. **Output**: Print transcription, detected language, and detected emotion

### 🧪 Sample Code Usage

```python
emotion_classifier, label_encoder = train_emotion_classifier()
emotion_aware_speech_recognition("/content/happy voice.mp4")
```

### 🎯 Example Output

```
Transcription: Hello, how are you today?
Language Detected: en
Detected Emotion: happy
```

### 📁 File Format

* Input: `.mp4` audio file
* Internal conversion to `.wav` for processing

### 📌 Notes

* The emotion classifier is trained on synthetic/random data for demonstration. Replace with real labeled emotion datasets for production use.
* Whisper model used: `"base"` (can be changed to `tiny`, `small`, `medium`, or `large`)

### 📜 License

MIT License

