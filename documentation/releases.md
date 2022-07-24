# Releases

All Video Trimmer releases can be downloaded from [GitHub](https://github.com/rendeer-pl/VideoTrimmer/releases/latest/download/VideoTrimmer.exe):

* [**Click here to download the latest version of Video Trimmer**](https://github.com/rendeer-pl/VideoTrimmer/releases/latest/download/VideoTrimmer.exe),
* Previous releases can be downloaded from the [Releases](https://github.com/rendeer-pl/VideoTrimmer/releases/) page on GitHub.

## Change Logs

### 1.1.2.220724
* The position of range markers will now properly update when resizing the window,
* The position of range markers will now properly update when opening a file through start argument ("Open with..."),
* Fixed a bug with flickering taskbar progress indicator on Windows 11,
* Visual improvements.

### 1.1.1.220620
* If the required FFmpeg executable is not found, the app will now suggest downloading it automatically,
* The timeline now includes markers representing the start and end timecode. Both the markers and the timeline thumb can now be dragged to adjust the range,
* Added basic keyboard shortcuts and improved keyboard navigation,
* Additional visual improvements and bugfixes.

### 1.1.0.220605
* Enabled support for MKV files,
* Fixed positioning of UI elements, which makes it possible to resize the main window. The default size has been increased to properly accommodate 16:9 videos,
* The visuals of the timeline have been reworked, and now it includes a preview of the trim range,
* There's a new "About" button which opens a separate window with details of the version, license, links to the website and a button to check for updates,
* Small bugfixes and visual improvements.

### 1.0.0.211026
* Refreshed UI,
* New icon,
* Fixed timeline behavior on video end,
* Added the possibility to remove focus from text inputs by clicking on the window background,
* Fixed FFMPEG download link,
* Under the hood improvements.

### 0.2.8.200218
* Added a video player with visual timecode picker,
* "Handler_name" metadata is now cleared in each trimmed file,
* Fixed a bug that caused trimming to fail if calculated bitrate contained a decimal point,
* Fixed a bug where dragging an unsupported file didn't make the window's background red,
* Added protection for unexpected FFmpeg output.

### 0.2.7.200218
* Fixed a bug that caused trimming to fail in some cases when the file was opened through Windows context menus.

### 0.2.6.200217
* UI readability improvements,
* Added support for taskbar progress indicator,
* Added support for opening files through Windows context menus ("Open with...").

### 0.2.5.200210
* Improvements to window position management.

### 0.2.4.200209
* When recompressing videos, the progress bar now displays actual progress,
* Add option to make the file size fit under a certain MB limit,
* Fixed a bug that caused the app to crash if user tried to drag and drop anything other than a file.

### 0.2.3.200101
* Added support for .avi files,
* Fixed a bug that caused filenames to include the extension twice,
* Fixed a bug that caused the file selection to be cleared when cancelling the File Picker dialog.

### 0.2.2.190530
* Fixed a crash that occured when trying to copy console command after trimming,
* Aborting an operation now actually closes the underlying FFmpeg process,
* Audio file duration is now properly formatted in the "End" input field,
* New app icon for improved readability on Windows taskbar.

### 0.2.1.190529
* Added option to recompress video, allowing for greater precision when trimming videos with low keyframe density,
* Added new progress window,
* Added new button to copy the FFmpeg command to clipboard,
* Added support for more video and audio formats.

### 0.2.0.190518
* Added notification when trimming fails,
* Notification waits for trimming to end, so the explorer window should always point to right file,
* Added option to remove sound from trimmed video.

### 0.1.3.190516
* Added support for dropping files from explorer.

### 0.1.2.190512
* Blocked input fields when a file has not been picked up yet,
* Added input validation on changing focus.

### 0.1.1.190511
* Initial functionality.