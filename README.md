# EfficientNet_Classification_DeepTooth
Train Classification to predict Gender using EfficientNetB0

# แบบที่ 1 แบบรุ่นพี่
## Parameter
```batch_size = 16
width = 150
height = 150
epochs = 250
dropout_rate = 0.2
input_shape = (height, width, 3)
```
## DataGenerator
```
rescale=1./255, #โมเดลส่วนใหญ่ต้องใช้ RGB ในช่วง 0–1
rotation_range=40,
width_shift_range=0.2,
height_shift_range=0.2,
shear_range=0.2,
zoom_range=0.2,
horizontal_flip=True,
fill_mode='nearest')
-----------------------------------
class_mode= categorical
```
## compile
```
loss= categorical_crossentropy
optimizer= RMSprop
metrics= accuracy
```
### [Train รอบที่ 1 (250 epochs, Freeze)](ของรุ่นพี่_Class_1_Train_2e_4_Freeze.ipynb)
#### Train จากชุดข้อมูลใหม่
```
learning_rate=2e-4
```
### [Predict รอบที่ 1](ของรุ่นพี่_01_Predict_Class.ipynb)
#### ผลจากชุดข้อมูลใหม่
- classification accuracy: 70.10 % 
- MAE: 0.2990455991516437
- MSE: 0.2990455991516437
- RMSE: 0.5468506186808639  
#### [Train ของรุ่นพี่](GG1_Train_2e_4_Freeze.ipynb)
```
learning_rate=2e-4
```
#### [ผลจากรุ่นพี่](https://github.com/Wanita-8943/Main_Project/blob/main/A2_Predict_Freeze.ipynb)
* MAE: 0.36105263157894735
* MSE: 0.36105263157894735
* RMSE: 0.6008765526952665





