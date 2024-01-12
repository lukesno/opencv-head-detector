# Pipeline
1) head-detector-opencv\face_detection.py
2) EVM -> http://people.csail.mit.edu/mrub/evm/#code
3) opencv-red-channel-extraction\extract_red_channel.py
4) opencv-red-time-plot\plot_red_channel_over_time.py
5) opencv-peak-analysis\peak_analysis.py
6) polar-api-client\main_web_app.py 
   (replace your config.yml with your Polar credentials)

To run each script find instructions in each README

# future
We want each script to subsequently call each other.

In Powershell, use pipeline_win.ps1 to put a video through the entire processing pipeline:
    .\pipeline_win.ps1 <input_vid_path> <output_dir>

NOTE: A new directory will be created under output_dir, using the name of the video input file

Example:
    .\pipeline_win.ps1 .\EVM\EVM_Matlab_bin-1.1-win64\elevated_130bpm.mp4 res

