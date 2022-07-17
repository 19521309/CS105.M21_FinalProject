# CS105.M21 - Facial Expression Recognition

## Nhóm 12

**Giảng viên viên hướng dẫn :  Nguyễn Vinh Tiệp**
| MSSV       |  Họ và Tên       | Công Việc                               |
| -----------| -------------    |-----------------------------------------|
| 19522454   | Nguyễn Tấn Tú    | [Train ResNet50](https://www.kaggle.com/code/tunguyentan/face-emotion-recognition-using-resnet50), [Detect Face and Predict](https://colab.research.google.com/drive/1xiKulEmis7lrTgW7ktfXT0S3dubX3dX8?usp=sharing)|
| 19522555   | Nguyễn Thị Như Ý | [Train VGG16](https://www.kaggle.com/code/tunguyentan/face-emotion-recognition-using-vgg16/notebook), làm slide PowerPoint   |
| 19521217   | Trần Nguyễn Quỳnh Anh | Thu thập private test data, làm slide PowerPoint|
| 19521309   | Đinh Hoàng Linh Đan | Deploy web API |
## Link Google Drive :
- Link goodgle drive chứa toàn bộ private test dataset, source code, model, kết quả: [here](https://drive.google.com/drive/folders/1q8-q92FlpLNYbcPiv-oMGzA5p_uyCLLs?usp=sharing)
## Dataset
- Dataset nhóm sử dụng là FER2013 trên Kaggle [ở đây](https://www.kaggle.com/datasets/nicolejyt/facialexpressionrecognition)\
- Private test data : [ở đây](https://drive.google.com/drive/u/0/folders/1lHtybnr5VOFmBN83Ky9vLHFs8bJtw3wC)
## Các nghiên cứu trước
### Rank 1:
- Model : Ensemble ResMaskingNet with 6 other CNNs
- Accuracy : 76.82%
- [Link](https://arxiv.org/pdf/1307.0414v1.pdf)
### Rank 2:
- Model : Local Learning Deep+BOW
- Accuracy : 75.42%
- [Link](https://arxiv.org/pdf/1804.10892v7.pdf)
### Rank 3:
- Model : LHC-Net
- Accuracy : 74.42%
- [Link](https://arxiv.org/pdf/2111.07224v2.pdf)
## Model nhóm sử dụng : [ở đây](https://drive.google.com/drive/folders/1Gr-u9cjommoOPQznk-gOBWAQSxXnolmE?usp=sharing) 
- ResNet50 : Accuracy 65.94%
- VGG16 : Accuracy 68.63%
## Test trên private test data
- ***Source code*** trong file PredictOnTestImages.ipynb
- ***Source code*** của Detect face and predict trong file DetectFaceAndPredict.ipynb
## Ứng dụng dự đoán biểu cảm gương mặt sử dụng Streamlit, Python dựa trên 2 model đã được train ở trên.
***Source code*** của Deploy Web API trong file app_ResNet50.py và app_VGG16.py
- Link video demo : [here](https://drive.google.com/drive/folders/1rV8oQ9Lk6bVwVyhxD3lj0bVVHqPq6tKT?usp=sharing)
- Link detect face và dự đoán biểu cảm khuôn mặt bằng ResNet50 : [here](https://huggingface.co/spaces/linhdan412/Facial_Emotion_Regconition_ResNet50?fbclid=IwAR194dLHOM9y5Jzahm4mXnmCNE1Urch6obmpL-in2DLzRXTyUtSCCcVjv9k)
- Link detect face và dự đoán biểu cảm khuôn mặt bằng VGG16 : [here](https://huggingface.co/spaces/linhdan412/Facial_Emotion_Regconition)
