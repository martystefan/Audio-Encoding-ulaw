# Audio-Encoding-ulaw
## Audio Encoding ulaw High Quality

### Standardanwendung

µ-law (auch u-law oder PCMU) ist ein Kompandierungsverfahren im Sprachcodec ITU-T G.711 für die digitale Telefonie und VoIP. Es komprimiert lineare PCM-Abtastwerte logarithmisch auf 8 Bit pro Sample bei einer Abtastrate von 8 kHz. µ-law kann den Container .au verwenden.

### Anwendung für High Quality Stereo Audio

Man kann bei ulaw auch höhere Abtastraten encodieren. Wie bei CD Qualität kann man eine Abtastrate von 44.1 khz verwenden. Damit bleiben die Höhen erhalten bei Musikstücken. Es werden dabei Abtastwerte von 8 bit logarithmisch verwendet. Das bedeutet das im vergleich zum Standard CD PCM 16bit, 44.1khz eine Halbierung der Dateigrösse resultiert. CD Bitrate 1,411kbps, ulaw 705kbps.

### Erfahrung Hörerlebnis.

Beim normalen hören sind kaum negative Effekte feststellbar gewesen. Der Hörgenuss ist praktisch nicht eingeschränkt. Meine ABX Tests haben praktisch keine Unterscheidbarkeit gezeigt. 

Fragen, Feedback und Ergebnisse von Hörtests sind willkommen! Erstelle bei Bedarf gerne ein Issue.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Standard Application

µ-law (also written as u-law or PCMU) is a companding method used in the ITU-T G.711 speech codec for digital telephony and VoIP. It logarithmically compresses linear PCM samples down to 8 bits per sample, using a sampling rate of 8 kHz. µ-law can use the .au container.

### Application for High-Quality Stereo Audio

It is also possible to encode at higher sampling rates using µ-law—for instance, a sampling rate of 44.1 kHz, which is equivalent to CD quality. This preserves the high-frequency content in musical tracks. The process employs 8-bit logarithmic sampling, which results in a file size half that of standard 16-bit, 44.1 kHz CD-quality PCM. (CD bitrate: 1,411 kbps; µ-law: 705 kbps.)

### Listening Experience

During standard listening, virtually no negative effects were perceptible. The listening experience remains essentially unimpaired; my ABX tests have shown that the formats are practically indistinguishable.

Questions, feedback, and listening test results are welcome! Feel free to open an issue.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Encoding with FFmpeg

```ffmpeg -i "input.wav" -c:a pcm_mulaw -ar 44100 -ac 2  "output.au"```

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Supported Players

footbar2000<br>
VLC<br>
Windows Media Player<br>

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

martystefan, 18.11.2026


