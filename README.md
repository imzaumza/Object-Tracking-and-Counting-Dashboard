<h1 align="center">Object Tracking and Counting Dashboard</h1>

## :innocent: Motivation
We adore statistics and graphs and figures as AI engineers! So, why not project the inference data onto a platform in order to better understand the inference? When a model is deployed on the edge for monitoring, it necessitates extensive frontend and backend development in addition to deep learning efforts – from gathering live data to showing accurate results. So I decided to build a small-scale video analytics program to learn what features would be valuable for such a product and what restrictions might exist.

## :framed_picture: Demo


## :key: Features

<ol>
    <li>Choose input source - Local, RTSP or Webcam</li>
    <li>Input class threshold</li>
    <li>Set FPS drop warning threshold</li>
    <li>Option to save inference video</li>
    <li>Input class confidence for drift detection</li>
    <li>Option to save poor performing frames</li>
    <li>Display objects in current frame</li>
    <li>Display total detected objects so far</li>
    <li>Display System stats - Ram, CPU and GPU usage</li>
    <li>Display poor performing class</li>
    <li>Display minimum and maximum FPS recorded during inference</li>
</ol> 

## :dizzy: How to use?
<ol>
    <li>Clone this repo</li>
    <li>Install all the dependencies</li>
    <li>Download deepsort <a href="https://drive.google.com/drive/folders/1xhG0kRH1EX5B9_Iz8gQJb7UNnn_riXi6">checkpoint</a> file and paste it in deep_sort_pytorch/deep_sort/deep/checkpoint</li>
    <li>Run -> streamlit run app.py</li>
</ol>

## :star: Recent changelog
<ol>
    <li>Updated yolov5s weight file name in detect() in app.py</li>
    <li>Added drive link to download DeepSort checkpoint file (45Mb).</li>
</ol>

## Note
The input video should be in same folder where app.py is. If you want to deploy the app in cloud and use it as a webapp then - download the user uploaded video to temporary folder and pass the path and video name to the respective function in app.py . This is Streamlit bug. Check <a href="https://stackoverflow.com/questions/65612750/how-can-i-specify-the-exact-folder-in-streamlit-for-the-uploaded-file-to-be-save">Stackoverflow</a>.

Reference / Credit: https://github.com/SahilChachra/Video-Analytics-Dashboard
