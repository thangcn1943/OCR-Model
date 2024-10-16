# OCR-Model
![image](https://github.com/user-attachments/assets/ac6c3ebf-f3a1-4ee6-97eb-6b74d99355f8)
## Pipeline bài toán
![image](https://github.com/user-attachments/assets/66e4dcb5-ca68-4be3-9718-27ee8a6f0313)
## Link dataset: http://surl.li/glwqyd
Dataset gồm các folder ảnh và xml chứa các label gồm: đường dẫn ảnh, kích thước, các bboxes, text  
      ![image](https://github.com/user-attachments/assets/0bc1b0e9-9b7b-4769-8009-e7575f6716d1)

## 1. Tiền xử lý dữ liệu  
Extract thông tin từ file word.xml về dạng yolo_data để đưa vào mô hình YOLOv8
    ![image](https://github.com/user-attachments/assets/d78de8f4-f276-487d-a173-19d2e0c96cb8)

## 2. Text detection
Sử dụng mô hình YOLOv8 đã được pre trained để training  
yolo_dataset:
  ![image](https://github.com/user-attachments/assets/2ccc1acc-08c9-40d8-a5ce-680356e227eb)
## 3. Text recognition 
Sử dụng mô hình CRNN với phương pháp transfer learning từ ResNet101: các lớp cuối cùng của ResNet101 sẽ được tinh chỉnh (fine-tuning) bằng cách thay đổi 3 lớp cuối cùng để thích nghi với việc nhận diện và học các ký tự.   

![image](https://github.com/user-attachments/assets/6f91258f-e003-40d2-bf7c-e76b6f4a41f9)
## 4. Kết quả 
![image](https://github.com/user-attachments/assets/77165de2-9ea5-4c1e-86c6-02dec543eb5d)
