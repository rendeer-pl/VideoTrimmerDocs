# Feature List

* Opening videos with a visual preview,
* Ability to specify in and out points via manual textbox entry,
* Option to remove autio from a video,
* Trimming videos in two ways:
    * **Without reencoding**, which preserves 100% of the quality of the source video, at the expense of not being able to precisely adjust the In and Out points (the video will be trimmed at previous keyframes). This is the fastest option, as the duration of the trimming is only limited by read and write speeds of the hard drive. As a result, processing most videos takes mere seconds.
    * **With reencoding**, which allows precise adjustment of In and Out points, but leads to some loss of quality. However, the user is given an additional option to keep the file size of the final video under a certain limit expressed in MB.
* After a trimming process has been completed, user can chose to copy the FFmpeg command to clipboard. The command can then be manually modified and executed through a command prompt.

### Trimming Modes Breakdown
|   | Trimming without reencoding  | Trimming with reencoding  |
|---|:---:|:---:|
| Speed | Most videos will be trimmed in seconds<br/>(limited by disk speed) | Most videos will be trimmed in minutes<br/>(limited by CPU speed) |
| Trim precision | In and Out points are adjusted to previous keyframe | In and Out points can be adjusted with frame-accuracy |
| Quality | Lossless | Reduces quality |
| Option to keep the file size under X MB | ❌ No |  ✔️ Yes |
| Option to remove audio | ✔️ Yes |  ✔️ Yes |

## Supported File Extensions
| Video | Audio |
|:---:|:---:|
|.mp4<br/>.mpg<br/>.mpeg<br/>.wmv<br/>.avi<br/>.mov<br/>.mts<br/>.m2ts<br/>.vob|.mp3<br/>.wav<br/>.aiff|