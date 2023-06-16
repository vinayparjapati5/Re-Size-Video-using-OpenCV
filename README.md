# Re-Size-Video-using-OpenCV
# Methodology
![image](https://github.com/vinayparjapati5/Re-Size-Video-using-OpenCV/assets/114856104/d596f581-8a93-4995-af18-db905fd1db27)
# Code Explanation
The code you provided performs the following steps:

1. Imports the necessary libraries, `cv2` for computer vision operations and `VideoFileClip` from `moviepy.editor` for video processing.

2. Specifies the path to the input video file and creates a `VideoCapture` object named `cap` to load the video file.

3. Retrieves the video properties such as frames per second, width, and height of the video.

4. Calculates the new dimensions for resizing the video by reducing the width and height by 50% (rescaling to 50% of the original size).

5. Specifies the output path for the resized video and creates a `VideoWriter` object named `out` to write the resized frames to the output video file. The video codec is set to "mp4v".

6. Starts a loop to process each frame of the video. It reads each frame using the `cap.read()` method, resizes the frame using `cv2.resize()`, and writes the resized frame to the output video using `out.write()`.

7. Checks if the 'q' key is pressed to quit the loop and stop the program.

8. Releases the video capture and writer objects using `cap.release()` and `out.release()` to free up system resources.

9. Closes any OpenCV windows that were opened during the process using `cv2.destroyAllWindows()`.

10. Adds audio to the resized video using `VideoFileClip` from `moviepy.editor`. It loads the resized video clip, loads the original video clip, extracts the audio from the original clip, and sets the audio to the resized clip. Then it writes the final video with audio to the output file.

11. Prints a message indicating that the resizing is complete and the resized video with audio is saved.

Overall, this code loads a video, resizes its frames to 50% of the original size, saves the resized video, adds the audio from the original video, and saves the final video with audio.

