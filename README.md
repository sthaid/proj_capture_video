# Automatic Dog Feeder Webcam

This project provides a script to capture a short video from a webcam,
and upload this video to Google Drive.

The following steps are performed by the capture_video script, which is
run by a cron job on a Raspberry Pi (Architecture armv7l, 4 CPUs).
* Turn on Tplink Smartplug, turns on lamp
* Run ffmpeg to capture a 600 second video, including audio.
* Turn off Tplink Smartplug, turns off lamp
* Delete last weeks video file from Google Drive
* Upload the new video file to Google Drive.

See NOTES file for additional details.
