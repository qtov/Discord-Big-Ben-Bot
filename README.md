# Discord-Big-Ben_Bot
A bot that will join a set voice channel and play the sound of big ben's bong for every hour it is.

## Setup
```
# Setup the env:
echo DISCORD_TOKEN=<yourdiscordtoken> > .env
echo VOICE_CHANNEL_NAME=<channel_to_join> >> .env
echo TIMEZONE=Europe/Bucharest >> .env
echo WAV_PATH=big_ben_bell.wav >> .env

python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python3 Code.py
```

## Function
The bot will join a pre-defined (In environment/env.var) voice channel at the start of every hour xx:00. It will then play the wav file once for every hour it is (1am one play, 11pm, 23 plays etc).
It will only join the channel if there are users in it.
