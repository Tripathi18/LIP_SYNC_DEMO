**Lip-Sync Video Generator**

This Python script combines a video file with an audio file to generate a lip-synced video. The script utilizes the OpenCV and MoviePy libraries to extract video frames, read audio files, and synchronize them to create a new output video.

**Prerequisites**

Make sure you have the following libraries installed:

OpenCV

MoviePy

You can install the required libraries using pip:

pip install opencv-python

pip install moviepy

**Usage**

Place your video file (video.mp4) and audio file (output10.wav) in the same directory as the script.
Update the video_path and audio_path variables in the script with the correct file names or paths.

video_path = 'video.mp4'  # Path of your video file

audio_path = 'output10.wav'  # Path of your audio file

Run the script. It will generate a lip-synced video by combining the video frames and audio. The output video will be saved as output_video_1.mp4.

python lip_sync.py

**Note: Ensure that the video and audio files have compatible formats and codecs.**

**Customization**

If you want to change the output video file name or path, modify the output_path variable in the script:

output_path = 'output_video_1.mp4'  # Final output video name

You can adjust the extracted video duration to match the audio by modifying the subclip function:

video = mp.VideoFileClip(video_path).subclip(0, audio_duration)

To change the codec used for the output video, modify the codec parameter in the write_videofile function:

video_with_audio.write_videofile(output_path, codec='libx264')

**Feel free to modify and use the code according to your requirements.**

**Troubleshooting**

If you encounter any issues or errors while running the script, make sure you have the necessary dependencies installed (OpenCV and MoviePy) and that the file paths are correct.

For further assistance or inquiries, please contact me at ayusht18dec@gmail.com.
