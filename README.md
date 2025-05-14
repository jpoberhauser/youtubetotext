# Youtube Video to Text

Tool that enables converting videos from a variety of sources, for example youtube, into text using Whisper. Mostly as an option to analyze videos through its transcribed audio instead of going multi-modal. 


Use this tool to:

    * feed videos as text into context of your LLM project

    * generate a library of text on latest youtube videos to populate your vector DB for RAG.

    * do sentiment analysis or any other kind of text modeling on top of audio from videos. 


| YouTube Clip Duration | Whisper Model | Transcription Time |
|-----------------------|----------------|---------------------|
| 24 minutes            | medium         | ~13 minutes         |
| 24 minutes            | small          | ~5 minutes          |

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


## Now, you have the entire text transcribed as a .txt like:

 Luis Robert, trade rumors are real.
 Bob Nightingale has reported that Luis Robert Jr.
 and the New York Mets have been linked in possible trades.
 The White Sox are looking at Mets prospects.
 We're gonna talk about everything that there is
 to possibly talk about with these Luis Robert trade rumors
 in today's YouTube video and podcast episode.
 Make sure you are subscribed to the Mets on Podcast,
 YouTube channel, so don't miss out on any of the content
 coming at you, videos after every single series,
 and a third bonus episode every single week.
 So you're gonna want to stick around and see that.
 And if you are listening to us on Apple,
 podcast, Spotify, Google, whatever it is,
 drop us a reading, drop us a review,
 download and subscribe.
 We really do appreciate it.
 James, when I saw this news,
 I know we've talked about this off camera many a times.
 Luis Robert would be awesome on this team.
 He'd be fantastic to have.
 He'd be kind of perfect,
 because when you look up and down
 this Mets roster right now,
 there's, they're really strong and deep,
 basically every single position of the starting nine.
 I guess of the starting eight,
 really beside center field.
 I know that we love Tyrone Taylor.
 He's become a bit of a cult hero for Mets fans.
 He walks up to Ice Cube.
 He was really clutching the playoffs last year.
 Really good defensive center fielder.
 He's a solid ball player.
 Jose Seria is out.
 He will be back at some point.
 But again, if you look at this team up and down,
 you're like, what position is the one
 of the guys on the field
 that would be the most worth upgrading?
 And of the lineup,
 it's very clearly center field.
 Luis Robert Jr.'s that spot right now
 where he has two years of team options left
 on his White Sox contract,
 $20 million each for the next two seasons
 and both totally voluntary money.
 So the White Sox can just get rid of him
 from the end of the season if they don't want to 