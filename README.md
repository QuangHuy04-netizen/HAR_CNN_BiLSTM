# Human Activity Recognition (HAR) using CNN-BiLSTM

##  Giới thiệu
-Xây dựng mô hình đưa ra dự đoán về hành dộng của con người(đầu vào là chuỗi tín
hiệu cảm biến).  

-Thông qua việc phân tích và xử lý dữ liệu của 30 người độ tuổi từ 19-48. Mỗi người
thực hiện sáu hoạt động (ĐI BỘ, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS,
NGỒI, ĐỨNG, NẰM), sử dụng gia tốc kế và con quay hồi chuyển được nhúng.

-Kết quả của mô hình có thể giúp ích cho việc nghiên cứu hay có thể áp dụng cho hệ
thống camera, giao thông, giám sát, hệ thống cảnh báo, phòng chống xâm nhập,...

##  Dữ liệu
- **Nguồn:** [UCI HAR Dataset](https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones)
- Hoặc tải từ Kaggle: [Human Activity Recognition with Smartphones](https://www.kaggle.com/datasets/uciml/human-activity-recognition-with-smartphones)
- File cần thiết: `train.csv`, `test.csv`

##  Mô hình
- Baseline: CNN đơn giản (2 lớp Conv1D + Dense)
- Cải tiến: Hybrid CNN-BiLSTM với BatchNormalization và Dropout

## Roadmap
![Baseline CNN](images/baseline_cnn.png)
![Hybrid CNN-BiLSTM](images/hybrid_cnn_bilstm.png)

##  Cài đặt và chạy
```bash
pip install -r requirements.txt
jupyter notebook notebooks/processing_model.ipynb
