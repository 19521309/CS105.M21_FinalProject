# CS105.M21 - Facial Expression Recognition

## Nhóm 10

**Giảng viên viên hướng dẫn :  Đỗ Văn Tiến**
| MSSV       |  Họ và Tên       | Công Việc                               |
| -----------| -------------    |-----------------------------------------|
| 19522454   | Nguyễn Tấn Tú    | [Train ResNet50](https://www.kaggle.com/code/tunguyentan/face-emotion-recognition-using-resnet50), [Detect Face and Predict](https://colab.research.google.com/drive/1xiKulEmis7lrTgW7ktfXT0S3dubX3dX8?usp=sharing)|
| 19522555   | Nguyễn Thị Như Ý | [Train VGG16](https://www.kaggle.com/code/tunguyentan/face-emotion-recognition-using-vgg16/notebook), làm slide PowerPoint   |
| 19521217   | Trần Nguyễn Quỳnh Anh | Thu thập private test data, làm slide PowerPoint|
| 19521309   | Đinh Hoàng Linh Đan | Deploy web API |
#### Kết quả nhận được của 3 model sau khi train, [here](https://drive.google.com/drive/folders/1i6WXwbLw936VR_8g6qYCzWL8z_WaHlAN?usp=sharing)

## Detect Face and Predict
Detect khuôn mặt sử dụng thư viện của OpenCV. Với các tham số scaleFactor  = 1.05, minNeighbors =  6, minSize = (int(x_min), int(y_min))
Với, original là ảnh input
##### *x_min = original.shape[0]/15 , 1/15 chiều cao của ảnh*
##### *y_min = original.shape[1]/15 , 1/15 chiều rộng của ảnh* 
     
***Source code*** của Detect Face and Predict trong file DetectFaceAndPredict.ipynb

## Ứng dụng dự đoán biểu cảm gương mặt sử dụng Streamlit, Python dựa trên 3 model đã được train ở trên.
***Source code*** của Deploy Web API trong file streamlit.py.
