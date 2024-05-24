# FFMPEG

## h264 encode

`ffmpeg -i video.mp4 -c:v libx264 video.compressed.mp4`

## h265 (HVEC) encode
`ffmpeg -i video.mp4 -c:v libx265 video.compressed.mp4`

## Compress to bitrate

`ffmpeg -i video.mp4 -c:v libx264 -b:v 1000k video.compressed.mp4`

