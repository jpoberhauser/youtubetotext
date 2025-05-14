# Youtube Video to Text

Tool that enables converting videos from a variety of sources, for example youtube, into text using Whisper. Mostly as an option to analyze videos through its transcribed audio instead of going multi-modal. 


Use this tool to:

    * feed videos as text into context of your LLM project

    * generate a library of text on latest youtube videos to populate your vector DB for RAG.

    * so sentiment analysis or any other kind of text modeling on top of audio from videos. 

This tool uses the [Faster Whisper Library ](https://github.com/SYSTRAN/faster-whisper) to achieve up to 4 times faster transcription than openai whisper. 

Also, based on [YT-DLP ](https://github.com/yt-dlp/yt-dlp).

"yt-dlp is a feature-rich command-line audio/video downloader with support for thousands of sites. The project is a fork of youtube-dl based on the now inactive youtube-dlc."

## Setup

```bash
pip install faster-whisper
pip install yt-dlp  
```

## Usage

```bash
python engine.py --url https://youtube.com/watch?v=abc123 --model-size small
```