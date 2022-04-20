# downloading vimeo vods

0. get a vimeo account (duh)
1. buy/rent your vod
2. export cookies for vimeo.com (use a browser extension)
3. use youtube-dlp like this: 
```sh
yt-dlp --cookies cookies.txt VIMEO_VOD_URL
```
4. get the subtitles: open devtools and go to the network tab, search for `vtt` and download the files for the language you want
5. enjoy the content you purchased in a better video player ;)

