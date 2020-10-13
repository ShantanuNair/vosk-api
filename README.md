# About

Vosk is an offline open source speech recognition toolkit. It enables
speech recognition models for 16 languages and dialects - English, Indian
English, German, French, Spanish, Portuguese, Chinese, Russian, Turkish,
Vietnamese, Italian, Dutch, Catalan, Arabic, Greek, Farsi.

Vosk models are small (50 Mb) but provide continuous large vocabulary
transcription, zero-latency response with streaming API, reconfigurable
vocabulary and speaker identification.

Speech recognition bindings implemented for various programming languages
like Python, Java, Node.JS, C#, C++ and others.

Vosk supplies speech recognition for chatbots, smart home appliances,
virtual assistants. It can also create subtitles for movies,
transcription for lectures and interviews.

Vosk scales from small devices like Raspberry Pi or Android smartphone to
big clusters.

# Documentation

For installation instructions, examples and documentation visit [Vosk
Website](https://alphacephei.com/vosk).

# Setup

Docker (Vosk Websocket/GRPC Server)
- ```docker run -d -p 2700:2700 alphacep/kaldi-en```

Vosk Server
- Clone https://github.com/alphacep/vosk-server
- ```cd vosk-server && pip install -r requirements.txt```
- ```cd websocket```
- To transcribe a .wav
    - Start Docker Container
    - ```python3 ./test.py test.wav```
- To transcribe via ffmpeg
    - Start Docker Container
    - ```python3 ./test_ffmpeg.py test.mp4```

Vosk Api
- Clone https://github.com/ShantanuNair/vosk-api
- ```cd python/example```
- To transcribe via ffmpeg to simple transcription
    - ```python3 test_ffmpeg_to_text.py test.mp4```
