# sleep-sounds-detector-server
Program that detects sounds during your sleep (talking, snoring, lunatism etc). 

### high-level architecture

1. Server receives a chunk of sound data with timestamp and deviceId (ex. 10 minutes of recording)

2. Program analyses a data chunk if there's any non-background sounds

3. Program extracts parts of data where the sound is detected and returns those parts to the caller together with timestamp where it was found.

### how-to-run
To run it you'll need to have docker and docker-compose installed on your machine.
Then in root directory run:

```
docker-compose up
```

### technologies used

* Python 3.7

* PyAudio

https://github.com/gmaslov/apnea

https://github.com/skjerns/AutoSleepScorer

https://github.com/lakshmanmallidi/SleepApneaDetection

https://github.com/faroit/awesome-python-scientific-audio

https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3877189/

https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4148548/

https://github.com/xSparfuchs/clap-detection

https://stackoverflow.com/questions/2668442/detect-and-record-a-sound-with-python

https://stackoverflow.com/questions/892199/detect-record-audio-in-python/892293#892293

https://medium.com/@almeidneto/sound-pattern-recognition-with-python-9aff69edce5d

https://www.researchgate.net/figure/Example-of-a-26-s-excerpt-of-a-snoring-sound-signal-from-a-subject-in-our-database-The_fig1_221693467

https://pdfs.semanticscholar.org/ec98/15d8c632e9b02f1817daf57192f88e6c2687.pdf
