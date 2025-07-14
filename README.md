Player Re-Identification in a Single Feed 🎯
📌 Objective
Detect and track football players in a 15-second video using YOLOv11 for detection and Deep SORT for maintaining consistent player IDs — even when players leave and re-enter the frame.
🧠 Approach
- YOLOv11 was used to detect players frame-by-frame.
- Deep SORT was used to assign consistent IDs using spatial and appearance-based tracking.
- OpenCV handled reading the input video and writing the output.
- The final result is a video (output.mp4) where each player has a unique ID that stays the same even if they disappear and reappear.
📁 Files Included
File Name	Description
player_tracking.ipynb	Main Jupyter Notebook with full code
output.mp4	Output video showing tracked players
requirements.txt	Python libraries used in the project
report.pdf	Report describing the approach used
⚙️ How to Run
1. Clone or download the project folder.
2. Install required packages using:
   pip install -r requirements.txt
3. Open the Jupyter Notebook: player_tracking.ipynb
4. Run all cells sequentially.
5. output.mp4 will be generated in the same directory.
🛠️ Libraries Used
- ultralytics (YOLOv11)
- deep_sort_realtime
- filterpy
- opencv-python-headless
- numpy
