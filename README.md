# yolov4-deepsort-bkk_dataset
Object tracking implemented with YOLOv4, DeepSort, and TensorFlow.

repository นี้เป็นไฟล์ที่ได้แก้ไขเพิ่มเติมจาก github repository theAIGuysCode/yolov4-deepsort
เพื่อให้ได้ไฟล์ .csv ออกมาเป็น dataset และปรับแก้ parameters เพิ่มเติม
โดนมีไฟล์ README อยู่แล้ว สามารถไปดูได้ที่ไฟล์ README_theAIGuysCode.md

repository นี้ใช้กับไฟล์ google colab {}
เมื่อรันไฟล์ google colab นี้จะอ้างอิงถึง repository นี้โดยอัตโนมัติ
  Platform: Google Colab Ubuntu
  Python Version: Python 3.8 with GPU Runtime
  Dependencies: (from google colab)
  !pip install tensorflow==2.3.0
  !pip install protobuf==3.19.6
  !pip install certifi==2022.12.7
  !pip install idna==2.10
  !pip install tensorboard==2.9.1
  !pip install tensorboard_data_server==0.6.1
  !pip install requests==2.25.1
  !pip install opencv-python
  !pip install easydict
  !pip install Pillow
  !pip install matplotlib
  !pip install numpy==1.20

ค่าต่าง ๆ ที่สามารถปรับจูนได้ใน ไฟล์ แต่ละบรรทัดต่าง ๆ ที่พบเจอคือ

  ไฟล์ object_tracker.py
    48: iou_threshold
    49: score threshold
    58: nms_max_overlap
    149: max_output_size_per_class
    150: max_total_size
    178: allowed_classes
    221: track.time_since_update
    
  ไฟล์ deep_sort/linear_assignment.py
    190: gating_distance
    
  ไฟล์ deep_sort/tracker.py
    40: max_iou_distance
    40: max_age
    40: n_init
      
  ซึ่งความหมายและรายละเอียดการแก้ต่าง ๆ สามารถดูเพิ่มเติมได้ในรายงาน
  
  
  
