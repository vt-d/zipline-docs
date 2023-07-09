# Video Thumbnails

Video Thumbnails are generated by [ffmpeg](https://ffmpeg.org), by taking the first frame of a video and saving it as a jpeg file within your datasource.

## How?

Video thumbnails are generated on an interval. By default every 10 minutes, Zipline will search for video files that do not have a thumbnail associated with them, and generate one for each.

To combat freezing the server, Zipline creates threads that are offloaded from Zipline's main server to generate thumbnails.

## Viewing

Once a video has a thumbnail, users can see the thumbnail on any portion of the dashboard that displays the video. This replaced the old placeholder that only said "Click to play video", which is replaced with the thumbnail, with a play-button on top of it, to indicate that it is a video.