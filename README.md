# Fewshot-PoseTransformer-ActionClassifier
# 🧠 Few-Shot Human Action Recognition using YOLO and Transformer

This project focuses on **recognizing human actions** in videos using pose keypoints extracted from YOLOv8 Pose model, followed by a **Transformer-based few-shot classification model**. It is optimized for very limited data (as few as 5 videos per class).

---

## 🎯 Project Highlights

- 🔍 **Pose Extraction** using YOLOv8 pose model (`yolov8n-pose.pt`)
- 🧠 **Transformer-based Action Classification** using cosine similarity
- 🧪 **Few-shot training**: only 5 videos per class (4 classes used)
- 🎞️ **Annotated Output Video** with keypoints + predicted action label
- 📈 Generalizable and lightweight pipeline for real-time systems

---

Each folder contains 5 short video clips. Keypoints are extracted frame-by-frame using Ultralytics' YOLOv8 pose model.

---

## 🧩 Workflow Overview

### 🔁 Full Pipeline
1. 📹 Load video clip
2. 🤖 Extract pose using `YOLO('yolov8n-pose.pt')`
3. 📏 Normalize & reshape keypoints
4. 🧠 Feed to Transformer for few-shot classification
5. 🎥 Annotate and save result with action name and pose

---

### 📈 Flowchart

![Workflow](path_to_your_workflow_image.png)

---

## 📽️ Demo Video

🎥 [Click here to see output](./final_result.avi)

---

## 🧠 Few-Shot Learning

This project uses **Few-Shot Learning** techniques:
- Only **5 examples per class**
- Cosine classifier instead of softmax for metric-based learning
- Efficient transformer for temporal modeling of pose sequences

---

## 🛠️ Requirements

Install dependencies using:

```bash
pip install -r requirements.txt


