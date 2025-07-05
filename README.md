This project is a real-time   violence detection system   powered by deep learning and computer vision. Using a hybrid model combining   YOLOv5   for person detection and a custom-trained   LSTM-based action recognition model  , it identifies violent activities in live video feeds and sends immediate alerts via   Telegram Bot  .

🚀 Key Features

   Real-time person detection   using YOLOv5 (`yolov5s.pt`)
     Violence activity recognition   with an ONNX-converted deep learning model (`violence_detector.onnx`)
   Integrated with   Telegram Bot API   for instant alert delivery
   Works with   webcam feeds   and can be extended to CCTV/IP cameras
   Modular structure with training and inference code separated in Jupyter Notebooks

  🧠 Model Architecture

     Person Detection:   YOLOv5 (pretrained weights)
     Action Recognition:   CNN-LSTM model trained on labeled violent/non-violent video data, exported to ONNX for efficient inference
     Inference Pipeline:   YOLOv5 detects people → cropped regions passed to the violence detection model → if violent activity is detected, a Telegram alert is triggered

  📁 Files

   `model training.ipynb` – Custom training pipeline for action recognition
   `violence detection and alert system.ipynb` – Real-time video inference with alert integration
   `yolov5s.pt` – Pretrained YOLOv5 weights
   `violence_detector.onnx` – Exported ONNX model for violence classification

  🔔 Telegram Bot Integration

   Built using the `python-telegram-bot` library
   Sends alerts with   timestamps   and   activity details  
   Ideal for integration in   surveillance systems  

  ⚙️ Tech Stack

   Python, OpenCV, PyTorch, ONNX Runtime, Telegram Bot API
   YOLOv5 for object detection
   LSTM-based model for sequence classification

