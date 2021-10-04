# Introduction

## Overview
Video Trimmer is a standalone Graphical user interface (GUI) for [FFmpeg](https://ffmpeg.org) meant to facilitate trimming down and reducing the size of videos. 

## Requirements
* Video Trimmer requires Windows 10 or newer with support for .net applications.
* In order to run properly, Video Trimmer requries `FFmpeg.exe` to be placed in the same directory as `VideoTrimmer.exe`. If you don't have `FFmpeg.exe`, you can download it from https://ffmpeg.org.

## Downloads
The most recent release can be downloaded from [GitHub](https://github.com/rendeer-pl/VideoTrimmer/releases/latest/download/VideoTrimmer.exe). Please see the [Releases](https://github.com/rendeer-pl/VideoTrimmer/releases/) page to access previous versions.

## Feature List
* Opening videos with a visual preview,
* Ability to select in and out points via timeline handle manipulation,
* Ability to specify in and out points via manual textbox entry,
* Option to remove autio from a video,
* Trimming videos in two ways:
    * **Without reencoding**, which preserves 100% of the quality of the source video, at the expense of not being able to precisely adjust the In and Out points (the video will be trimmed at previous keyframes). This is the fastest option, as the duration of the trimming is only limited by read and write speeds of the hard drive. As a result, processing most videos takes mere seconds.
    * **With reencoding**, which allows precise adjustment of In and Out points, but leads to some loss of quality. However, the user is given an additional option to keep the file size of the final video under a certain limit expressed in MB.

### Trimming Modes Breakdown
|   | Trimming without reencoding  | Trimming with reencoding  |
|---|---|---|
| Speed | Most videos will be trimmed in seconds | Dependant on CPU |
| Trim precision | In and Out points are adjusted to previous keyframe | In and Out points can be adjusted with frame-accuracy |
| Quality | Lossless | Reduces quality |
| Option to keep the file size under X MB | ❌ No |  ✔️ Yes |
| Option to remove audio | ✔️ Yes |  ✔️ Yes |


## Source code
The entire source (written in C# .net WPF) can be accessed, downloaded or forked on [GitHub](https://github.com/rendeer-pl/VideoTrimmer). Feel free to modify the code and contribute your changes.
