# Lip-Syncronization

# Lip Sync using Moviepy

This Python script demonstrates a simple lip sync using the Moviepy library. It synchronizes the audio of a given video with a provided audio file to create a lip-synced output video.

## Requirements

- Python 3.x
- Moviepy library (`pip install moviepy`)
- OS ('import OS')

from moviepy.editor import VideoFileClip, AudioFileClip
import os

## How to Use

1. Place your video file (input_video.mp4) and the audio file (input_audio.wav) in the same directory as the `lip_sync.ipynb` script.
2. You can find the Video and Audio File from below link
Video - https://openinapp.co/5cwva
Audio - https://openinapp.co/o9vuj

# Storing Paths to video and audio files
video_path = "path/to/video.mp4"
audio_path = "path/to/audio.wav"


# Loading video and audio clips
video_clip = VideoFileClip(video_path)
audio_clip = AudioFileClip(audio_path)


# Setting the audio of the video clip to the loaded audio clip
video_clip = video_clip.set_audio(audio_clip)

# Setting the duration of the video clip to match the duration of the audio clip
video_clip = video_clip.set_duration(audio_clip.duration)

# Specifying the output path for the lip-synced video
output_path = "C:\\Users\\Shubham\\OneDrive\\Desktop\\Python\Output5.mp4"

# Stored the final lip-synced video to the specified output path
video_clip.write_videofile(output_path, codec='libx264', audio_codec='aac')                                                                                                                      
# Lip-Synced Video is Successfully stored and Autoplayed by system
os.system(f"start {output_path}")



