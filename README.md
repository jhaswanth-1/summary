# IITISOC 2025 MEETING NOTES GENERATOR

# Automatic Meeting Notes Generator 📝

->Easily turn your meeting audio into clear, useful notes in just a few steps.

  ## Overview

-> Streamlit app that lets you:
->Transcribes meeting audio into text.
->Diarize speakers (show who spoke and when).
->Summarize meetings in humanize way .
->Translate summaries into popular Indian languages.
->Save summaries as neat PDFs.
->Use a UI with dark theme and guiding emojis.


## Features

- 🎤 Accurate speech-to-text using Whisper/WhisperX.
- 🗣️ Speaker diarization for identifying speakers and timestamps.
- 📝 Professional, human-like meeting summaries powered by LLaMA-3 model.
- 🔄 Translation into Hindi, Telugu, Tamil, Kannada, Marathi, Bengali, or English.
- 📄 One-click PDF download of summaries.
- ✨ Modern dark theme UI with smooth gradients and emojis.

## Demo

- Add a screenshot or GIF here to show your app in action.

## How It Works

1. Upload your meeting audio file (`.mp3`, `.wav`, `.m4a`).
2. Transcription with noise reduction runs automatically.
3. Speakers are diarized (who spoke what, and when).
4. A Humanizied, structured meeting summary is generated.
5. Optional translation to your favourite language.
6. Download your summary as a structured,formated PDF.

## Installation & Setup

-> **Clone the repo:**

-> **Requirements include:**
  -> Python 3.8+ and  less than 3.11 as other models are not available with that version python 
  -> streamlit, librosa, noisereduce, numpy, soundfile
  -> whisper, whisperx, pyannote.audio, fpdf, openai, deep-translator
  -> torch (with CUDA/cuDNN for GPU users) others it will run on cpu
  -> ffmpeg as a package
  ->or you can download directly the requirements.txt
    

- **Set up API keys in** .streamlit/secrets.toml file:

- **Run the app:**
  streamlit run app.py

## Configuration

-> it  Uses " medium " WhisperX model by default (good accuracy and moderate resource use).
-> Diarization batch sizes are reduced to avoid memory errors.
-> UI uses modern CSS styles for clarity and ease of use.

## Customization Options

-> UI colors and fonts = Edit the CSS block in "app.py".
->  PDF appearance    =  Modify the " PDF " class in the code for headers, footers, or logos.
-> Translation languages = Change options in the language dropdown.
-> Model choice =Swap WhisperX models via " load_whisperx_model() " (e.g., "small" , " large-v2 ").

## Troubleshooting Tips
- **GPU issues:**
  - Verify PyTorch installation and CUDA compatibility.
  - If no GPU, use CPU with slower speeds.

- **Missing API keys:**
  - Ensure both tokens are set in .streamlit/secrets.toml.

## Future Work / Planned Features 🚧

-> Mobile-friendly UI for phones and tablets.
-> Multiple audio file uploads and merging.
-> Meeting analytics (speaker talk time, keyword highlights).
-> User login and history management.
-> Support for more translation languages.
-> Sync summaries and action items with Google Calendar.

## License

-> MIT License.

## Credits

-> OpenAI Whisper & WhisperX
-> pyannote.audio
-> Streamlit
-> LLaMA-3 via Together API
-> All open-source libraries used


**Make your meeting notes quick, simple, and shareable — never miss an important point! 🚀**

