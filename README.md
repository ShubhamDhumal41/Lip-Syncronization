# Lip-Syncronization

# Lip Sync using Moviepy

This Python script demonstrates a simple lip sync using the Moviepy library. It synchronizes the audio of a given video with a provided audio file to create a lip-synced output video.

## Requirements

- Python 3.x
- Moviepy library (`pip install moviepy`)
- OS ('import OS')

- from moviepy.editor import VideoFileClip, AudioFileClip
- import os

## How to Use

1. Place your video file (input_video.mp4) and the audio file (input_audio.wav) in the same directory as the `lip_sync.ipynb` script.
2. You can find the Video and Audio File from below link
- Video - https://openinapp.co/5cwva
- Audio - https://openinapp.co/o9vuj

## Getting Started
1. Ensure you have a video file (e.g., TechNews.mp4) and an audio file (e.g., output10.wav) that you want to lip-sync.
2. Update the video_path and audio_path variables in the lip_sync.py script to point to your respective video and audio files:

## Storing Paths to video and audio files
video_path = "path/to/video.mp4"
audio_path = "path/to/audio.wav"


## Loading video and audio clips
video_clip = VideoFileClip(video_path)
audio_clip = AudioFileClip(audio_path)


## Setting the audio of the video clip to the loaded audio clip
video_clip = video_clip.set_audio(audio_clip)

## Setting the duration of the video clip to match the duration of the audio clip
video_clip = video_clip.set_duration(audio_clip.duration)

## Specifying the output path for the lip-synced video
output_path = "path/to/output.mp4"

## Stored the final lip-synced video to the specified output path
video_clip.write_videofile(output_path, codec='libx264', audio_codec='aac')                                                                                                                      
## Lip-Synced Video is Successfully stored and Autoplayed by system
os.system(f"start {output_path}")

## Contributing
Contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## Acknowledgments
We would like to acknowledge the MoviePy library for providing the necessary tools and functionalities for lip-syncing and video editing.

