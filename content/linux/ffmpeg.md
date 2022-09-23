# ffmpeg

## add subtitles to video

adds english subtitles
```
ffmpeg -i input.mp4 -i sub-eng.srt -c copy -c:s mov_text -metadata:s:s:0 language=eng ouptut_english.mp4
```
