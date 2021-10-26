# Using the App

## Prerequisites
In order to run the app, the `FFmpeg.exe` file needs to be placed in the same directory as `VideoTrimmer.exe`. If you don't have `FFmpeg.exe`, you can download it from https://ffmpeg.org.

## Opening Video Files
You can open a video file in three ways:
1. By right-clicking on a video file, selecting "Open With" and chosing Video Trimmer,
1. By drag-and-dropping a video file onto the Video Trimmer window,
1. By clicking the "Select video" button in the top left corner of the Video Trimmer window and picking your file through the system file picking dialog.

## Selecting Trim Range
With a file loaded, you can either click on the **Start** and **End** timecodes to modify them manually. Alternatively, you use the video player to navigate the timeline to the desired Start and End points and then click on the triangle buttons next to the timecodes to use the current position of the video player as Start or End:
![Setting Start and End positions](https://soft.rendeer.pl/VideoTrimmer/documentation/assets/VideoTrimmer-Start-End.png)

If you don't want to trim the file, you can leave the timecodes at their defaults: the Start is 00:00:00 and End is equal to the file's original duration.

## Additional Options
Video Trimmer has three additional options:

### Removing Audio
Will remove the audio track from the file. This is especially useful to remove undesired music or voice over (e.g. microphone sound on gameplay, in-car conversations in dashcam footage, etc.).

### Recompressing File
Video Trimmer allows trimming files either with or without recompressing them. Please use this guide to decide if you want to recompress your file or not:

| Don't recompress the file if... | Recompress the file if... |
| --- | --- |
| You want the output file to have loseless quality | You accept some level of quality degradation |
| You want the file trimmed as quickly as possible | You don't care about the duration of the trimming process |
| You don't care about the file size | You want to reduce the file size |
| You accept that the file might not be trimmed precisely at Start and End points | You need the trim to happen with high precision |

Please note this setting does not affect the possibility to remove the audio track.

### Keeping the File Size Below a Limit
If you chose to recompress the file, you can specify a limit (in MB) which will be used to calculate the video's target bitrate. Setting this to too low a value can lead to significant quality loss, but can be very helpful if the service you use to upload your file to (e.g. JIRA) has a strictly enforced file size limit.

Please note that setting this to 0 will disable the option and a default bitrate will be used instead.

## Trimming the File
Once you are happy with the settings, you can click **TRIM VIDEO** to start the trimming process. A new window will be displayed showing current progress:
![Progress window](https://soft.rendeer.pl/VideoTrimmer/documentation/assets/VideoTrimmer-Progress.png)

Please note an exact progress will only be displayed if you chose to recompress the file.

After the process will be done, a new Explorer window will be opened to show the new file location. On top of that, the progress window will contain a button to copy the full FFmpeg command which was used to perform the trim:

![Progress window after a trim has been completed](https://soft.rendeer.pl/VideoTrimmer/documentation/assets/VideoTrimmer-Progress-Finished.png)