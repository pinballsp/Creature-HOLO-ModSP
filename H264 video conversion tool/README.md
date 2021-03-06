
Convert video file to Raw H264
==============================

Download tool from this link:
https://mega.nz/#!pVdAxAza!3zsAmpZDwePizIyIggnU7Osevn-5LmAVQH7KPE_7ePw

HOLO ModSP work with video animations in Raw H264 format, so can not use directly any standard video/audio files.
At any rate, with ffmpeg tool, you will may convert easily any video file to h264.

ffmpeg is a command line tool so you'll need to open a terminal on your computer and navigate to the 
directory that contains your video.  Then run a command like this:

ffmpeg -i video.mp4 -vcodec copy -an -bsf:v h264_mp4toannexb video.h264

Where video.mp4 is the name of your video to convert (don't worry ffmpeg supports almost all video 
formats, so you can send it a .avi, .mov, .mkv, .mp4, m4v, etc.) and video.h264 is the name of the 
output file (raw h264 format).  

Make sure to keep the .h264 extension on the output file as it's required when using Creature HOLO ModSP.
After ffmpeg finishes running (usually the operation is quite fast since it's just extracting the 
H.264 stream) copy (and rename if need) the output .h264 file to the USB Pendrive of your HOLO ModSP.

Remember you must configure your HOLO ModSP to trigger any new video according with status of playfield 
switches, lamps, bumpers flashers, etc... Check User Manual for full instructions.

![alt text](http://i.imgur.com/YQ2eRFv.jpg)


