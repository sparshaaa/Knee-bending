# Knee-bending
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Knee Exercise Video Analysis with Mediapipe</title>
</head>
<body>
    <h1>Knee Exercise Video Analysis with Mediapipe</h1>
    <p>This project uses the Mediapipe library to analyze a video of a knee exercise. It tracks specific landmarks on the body to calculate the angle of the knee during the exercise, counts repetitions, and provides feedback based on the knee's position and duration.</p>
    
    <h2>Requirements</h2>
    <ul>
        <li>Python 3.6+</li>
        <li>OpenCV</li>
        <li>Mediapipe</li>
        <li>Numpy</li>
    </ul>
    
    <h2>Installation</h2>
    <ol>
        <li>
            <p><strong>Clone the repository:</strong></p>
            <pre><code>git clone &lt;repository_url&gt;
cd &lt;repository_directory&gt;</code></pre>
        </li>
        <li>
            <p><strong>Install the required Python packages:</strong></p>
            <pre><code>pip install opencv-python mediapipe numpy</code></pre>
        </li>
    </ol>
    
    <h2>Running the Script</h2>
    <ol>
        <li>
            <p>Place the video file (<code>knee_exercise_video.mp4</code>) in an accessible directory.</p>
        </li>
        <li>
            <p>Update the path to the video file in the script if necessary:</p>
            <pre><code>cap = cv2.VideoCapture(r"C:\path\to\your\video\knee_exercise_video.mp4")</code></pre>
        </li>
        <li>
            <p>Run the script:</p>
            <pre><code>python knee_exercise_analysis.py</code></pre>
        </li>
    </ol>

    <h2>Script Explanation</h2>
    <p>The script performs the following steps:</p>
    <ol>
        <li>Sets up the video capture and writer to process the input video and save the output.</li>
        <li>Initializes Mediapipe's Pose module for pose detection.</li>
        <li>Processes each frame of the video to detect body landmarks.</li>
        <li>Calculates the angle of the knee using the detected landmarks.</li>
        <li>Displays the calculated angle, repetition count, stage, timer, and feedback on the video.</li>
        <li>Counts repetitions and provides feedback based on the knee's bending duration.</li>
        <li>Saves the processed video with the overlaid information.</li>
    </ol>
</body>
</html>
