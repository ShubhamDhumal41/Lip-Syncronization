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

3. Load video and audio files, ensuring compatibility with various formats (MP4, WAV, etc.).

4. Determine the durations of the video and audio for synchronization.

5. Adjust video duration to match audio duration, either by looping the video or trimming it accordingly.

6. Synchronize the lip movements with the audio to create a visually realistic and cohesive output.

7. Save the final synchronized video with lip-synced audio for further analysis and presentation.

8. The lip-synced video will be saved at the specified output_path in MP4 format with the H.264 video codec and AAC audio codec.

9. The generated lip-synced video file will be stored at the specified output_path. It will also be autoplayed by the system.

## Note
The project showcases how lip sync can be achieved programmatically, enabling applications in video editing, media production, and entertainment industries. The model's effectiveness can be assessed through visual inspection and further analysis of lip-sync accuracy. The complete code and instructions are available in the GitHub repository, along with sample inputs and outputs for demonstration.

## Contributing
Contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## Acknowledgments
We would like to acknowledge the MoviePy library for providing the necessary tools and functionalities for lip-syncing and video editing.
Also I would like to acknowledge OpeninApp for giving the access to the Video and Audio file.

