# Whisper

This repo contains the files that are created as a result of running OpenAI's
Whisper project on a video's audio ([Ben Holmes' interview with Dan Abramov about React Server components](https://www.twitch.tv/videos/1779925131)).
Below are instructions on how to use Whisper.

## Setup

### Python
1. [Install `pyenv`](https://github.com/pyenv/pyenv#installation)
1. [Install `pyenv-virtualenv`](https://github.com/pyenv/pyenv-virtualenv#installation)
1. Install Python 3.10.9: `pyenv install 3.10.9`
1. Setup a virtual envirnment for this project: `pyenv virtualenv 3.10.9 whisper`
1. use this virutalenv for this folder: `cd` to this directory and run `pyenv local whisper` you should now see `(whisper)` before your command prompt

### Dependencies
1. Install ffmpeg
   | Operating System | Installation Instructions |
   | --- | --- |
   | macOS | [Install Homebrew](https://brew.sh/#install) then run: `brew install ffmpeg` in a terminal |
   | Linux (Debian) | Run `sudo apt update && sudo apt install ffmpeg` in a terminal |
   | Windows | [Install Chocolatey](https://chocolatey.org/install) then run: `choco install ffmpeg` in a terminal |
1. Install the whisper python library: `pip install git+https://github.com/openai/whisper.git`


## Running
1. run `whisper PATH/TO/audio.wav`


## Other

### Convert mp4 to wav

`ffmpeg -i <infile> -ac 2 -f wav <outfile>`

### Links
* https://mattcarrollcode.com/blog/transcribing-audio-with-openai-whisper
* https://www.assemblyai.com/blog/how-to-run-openais-whisper-speech-recognition-model/
* https://github.com/openai/whisper

