# EfficientNet_Classification_DeepTooth
Train Classification to predict Gender using EfficientNetB0

# แบบที่ 1 แบบรุ่นพี่
[Drive: Model --> EfficientNet_Class_ตามรุ่นพี่](https://drive.google.com/drive/u/0/folders/1gcKfLRMW9bdXK00KoxQvzCdfypyPALKf)
## Parameter
```batch_size = 16
width = 150
height = 150
epochs(All!) = 1050 (250250,250,250,50)
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
#### [Train ของรุ่นพี่ (250 epochs, Freeze)](https://github.com/Wanita-8943/run/blob/main/GG1_Train_2e_4_Freeze.ipynb)
```
learning_rate=2e-4
```
### [Predict รอบที่ 1](ของรุ่นพี่_01_Predict_Class.ipynb)
#### ผลจากชุดข้อมูลใหม่
- classification accuracy: 70.10% 
- MAE: 0.2990455991516437
- MSE: 0.2990455991516437
- RMSE: 0.5468506186808639  

#### [ผลจากรุ่นพี่](https://github.com/Wanita-8943/run/blob/main/Predict_GG1_2e_4_250%E0%B8%A3%E0%B8%AD%E0%B8%9A.ipynb)
* classifier accuracy: 63.89%
* MAE: 0.36105263157894735
* MSE: 0.36105263157894735
* RMSE: 0.6008765526952665

### [Train รอบที่ 2 (250 epochs, Freeze)](ของรุ่นพี่_Class_2_Train_2e_4_Freeze.ipynb)
#### Train จากชุดข้อมูลใหม่
```
learning_rate=2e-4
```
#### [Train ของรุ่นพี่ (250 epochs, Freeze)](https://github.com/Wanita-8943/run/blob/main/GG2_Train_2e_4_Freeze.ipynb)
```
learning_rate=2e-4
```
### [Predict รอบที่ 2](ของรุ่นพี่_02_Predict_Class.ipynb)
#### ผลจากชุดข้อมูลใหม่
- classification accuracy: 70.52% 
- MAE: 0.2948038176033934
- MSE: 0.2948038176033934
- RMSE: 0.5429583939892572  

#### [ผลจากรุ่นพี่](https://github.com/Wanita-8943/run/blob/main/Predict_GG2_2e-4_250%E0%B8%A3%E0%B8%AD%E0%B8%9A.ipynb)
- classifier accuracy: 65.16%
- MAE: 0.34842105263157896
- MSE: 0.34842105263157896
- RMSE: 0.5902720157957507

### [Train รอบที่ 3 (250 epochs, Freeze)](ของรุ่นพี่_Class_3_Train_8e_5_Freeze.ipynb)
#### Train จากชุดข้อมูลใหม่
```
learning_rate=8e-5
```
#### [Train ของรุ่นพี่ (250 epochs, Freeze)](https://github.com/Wanita-8943/run/blob/main/B0_3_(8e-5)_Gender3_Train_Freeze.ipynb)
```
learning_rate=8e-5
```
### [Predict รอบที่ 3](ของรุ่นพี่_03_Predict_Class.ipynb)
#### ผลจากชุดข้อมูลใหม่
- classification accuracy: 71.69% 
- MAE: 0.2831389183457052
- MSE: 0.2831389183457052
- RMSE: 0.5321079950026171

#### [ผลจากรุ่นพี่](https://github.com/Wanita-8943/run/blob/main/B0_3_(8e-5)_Gender3_Predict_Freeze.ipynb)
- classifier accuracy: 66.95%
- MAE: 0.33052631578947367
- MSE: 0.33052631578947367
- RMSE: 0.5749141812387947

### [Train รอบที่ 4 (250 epochs, Unfreeze)](ของรุ่นพี่_Class_4_Train_8e_5_Unfreeze.ipynb)
#### Train จากชุดข้อมูลใหม่
```
learning_rate=8e-5
```
#### [Train ของรุ่นพี่ (250 epochs, Unfreeze)](https://github.com/Wanita-8943/run/blob/main/B0_4_(8e-5)_Gender4_Train_Unfreeze.ipynb)
```
learning_rate=8e-5
```
### [Predict รอบที่ 4](ของรุ่นพี่_04_Predict_Class.ipynb)
#### ผลจากชุดข้อมูลใหม่
- classification accuracy: 85.15% 
- MAE: 0.14846235418875928
- MSE: 0.14846235418875928
- RMSE: 0.3853081288900602
#### [ผลจากรุ่นพี่](https://github.com/Wanita-8943/run/blob/main/B0_4_(8e-5)_Gender4_Predict_Unfreeze.ipynb)
- classifier accuracy: 70.32%%
- MAE: 0.2968421052631579
- MSE: 0.2968421052631579
- RMSE: 0.5448321808255804

### [Train รอบที่ 5 (50 epochs, Unfreeze)](ของรุ่นพี่_Class_5_Train_8e_5_Freeze.ipynb)
#### Train จากชุดข้อมูลใหม่
```
learning_rate=8e-5
```
### [Predict รอบที่ 5](ของรุ่นพี่_05_Predict_Class.ipynb)
#### ผลจากชุดข้อมูลใหม่
- classification accuracy: 84.84% 
- MAE: 0.15164369034994699
- MSE: 0.15164369034994699
- RMSE: 0.38941454820017574

# แบบที่ 2 224 (Best Accuracy of EffNet)
[Drive: Model --> EfficientNet_Class_Func_224](https://drive.google.com/drive/u/0/folders/1-SvD1d9any3AMDkLwb31e2SduLk82sgV)
## Parameter
```
batch_size = 16
width = 224
height = 224
epochs(All!) = 1250 (250,250,250,250,250)
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
class_mode = 'raw',
color_mode= 'rgb',
```
## compile
```
loss= binary_crossentropy
optimizer= Adam
metrics= accuracy
```
### [Train รอบที่ 1 (250 epochs, Freeze)](224_01_Func_Eff_Classification_Train_250_Freeze.ipynb)
```
learning_rate=2e-4
```
#### [Predict รอบที่ 1](224_01_Predict_Class_Func.ipynb)
- classifier accuracy = 75.72%
- MAE: 0.31071181607868203
- MSE: 0.15842245076349293
- RMSE: 0.3980231786761833
 
### [Train รอบที่ 2 (250 epochs, Freeze)](224_02_Func_Eff_Classification_Train_250_Freeze.ipynb)
```
learning_rate=2e-4
```
#### [Predict รอบที่ 2](224_02_Predict_Class_Func.ipynb)
- classifier accuracy = 76.35%
- MAE: 0.2990765265628107
- MSE: 0.16170641546095552
- RMSE: 0.40212736223857676
  
### [Train รอบที่ 3 (250 epochs, Unfreeze)](224_03_Func_Eff_Classification_Train_250_Unfreeze.ipynb)
```
learning_rate=2e-5
```
#### [Predict รอบที่ 3](224_03_Predict_Class_Func.ipynb)
- classifier accuracy = 84.52%
- MAE: 0.16445366192832148
- MSE: 0.1234872460014169
- RMSE: 0.35140752126472324

### [Train รอบที่ 4 (250 epochs, Unfreeze)](224_04_Func_Eff_Classification_Train_250_Unfreeze.ipynb)
```
learning_rate=2e-5
```
#### [Predict รอบที่ 4](224_04_Predict_Class_Func.ipynb)
- classifier accuracy = 85.90%
- MAE: 0.14529008906873825
- MSE: 0.11789015906040803
- RMSE: 0.34335136385400894

### [Train รอบที่ 5 (250 epochs, Unfreeze)](224_05_Func_Eff_Classification_Train_250_Unfreeze.ipynb)
```
learning_rate=8e-6
```
#### [Predict รอบที่ 5](224_05_Predict_Class_Func.ipynb)
- classifier accuracy = 87.80%
- MAE: 0.13325601550983818
- MSE: 0.10793187427755038
- RMSE: 0.3285298681665799
- ![image](https://github.com/natthanich/EfficientNet_Classification_DeepTooth/assets/108257658/6135df37-c24e-4a89-9cc6-7fa40b600182)

# แบบที่ 3 02 (Lowest RMSE of EffNet)
[Drive: Model --> EfficientNet_Class_Func](https://drive.google.com/drive/u/0/folders/1-UDJZY5xgdAh5sxG0QnR2NI_G31xN7s7)
## Parameter
```
batch_size = 16
width = 224
height = 224
epochs(All!) = 2,250 (250,250,250,250,250,250,250,250,250)
dropout_rate = 0.2
input_shape = (height, width, 3)
```
## DataGenerator
```
rescale=1./255, #โมเดลส่วนใหญ่ต้องใช้ RGB ในช่วง 0–1
rotation_range=90,
fill_mode='reflect',
horizontal_flip=True,
vertical_flip=True
-----------------------------------
class_mode = 'raw',
color_mode= 'rgb',
```
## compile
```
loss= binary_crossentropy
optimizer= Adam
metrics= accuracy
```
### [Train รอบที่ 1 (250 epochs, Freeze)](02_1_Func_Eff_Classification_Train_250_Freeze.ipynb)
```
learning_rate=2e-4
```
#### [Predict รอบที่ 1](02_1_Predict_Class_Func.ipynb)
- classifier accuracy = 78.47%
- MAE: 0.28457237939199204
- MSE: 0.14829514322328702
- RMSE: 0.3850910843206929
 
### [Train รอบที่ 2 (250 epochs, Freeze)](02_2_Func_Eff_Classification_Train_250_Freeze.ipynb)
```
learning_rate=2e-4
```
#### [Predict รอบที่ 2](02_2_Predict_Class_Func.ipynb)
- classifier accuracy = 78.26%
- MAE: 0.2774899643803265
- MSE: 0.14886254335112464
- RMSE: 0.3858270899653427
  
### [Train รอบที่ 3 (250 epochs, Freeze)](02_3_Func_Eff_Classification_Train_250_Freeze.ipynb)
```
learning_rate=2e-5
```
#### [Predict รอบที่ 3](02_3_Predict_Class_Func.ipynb)
- classifier accuracy = 78.58%
- MAE: 0.26505273066212703
- MSE: 0.1465098407238998
- RMSE: 0.38276603914649976

### [Train รอบที่ 4 (250 epochs, Freeze)](02_4_Func_Eff_Classification_Train_250_Freeze.ipynb)
```
learning_rate=2e-5
```
#### [Predict รอบที่ 4](02_4_Predict_Class_Func.ipynb)
- classifier accuracy = 78.69%
- MAE: 0.27248133876770075
- MSE: 0.15136578368980314
- RMSE: 0.38905755832499017

### [Train รอบที่ 5 (250 epochs, Freeze)](02_5_Func_Eff_Classification_Train_250_Freeze.ipynb)
```
learning_rate=8e-6
```
#### [Predict รอบที่ 5](02_5_Predict_Class_Func.ipynb)
- classifier accuracy = 78.58%
- MAE: 0.2663221819079254
- MSE: 0.147616516459452
- RMSE: 0.3842089489580533

### [Train รอบที่ 6 (250 epochs, Unfreeze)](02_6_Func_Eff_Classification_Train_250_Unfreeze.ipynb)
```
learning_rate= 8e-6
```
#### [Predict รอบที่ 6](02_6_Predict_Class_Func.ipynb)
- classifier accuracy = 86.85%
- MAE: 0.16980871327073188
- MSE: 0.10893404435876028
- RMSE: 0.3300515783309637

### [Train รอบที่ 7 (250 epochs, Unfreeze)](02_7_Func_Eff_Classification_Train_250_Unfreeze.ipynb)
```
learning_rate= 8e-7
```
#### [Predict รอบที่ 7](02_7_Predict_Class_Func.ipynb)
- classifier accuracy = 87.06%
- MAE: 0.16680725170021027
- MSE: 0.10272266559131953
- RMSE: 0.3205037684510426
  
### [Train รอบที่ 8 (250 epochs, Unfreeze)](02_8_Func_Eff_Classification_Train_250_Unfreeze.ipynb)
```
learning_rate= 8e-8
```
#### [Predict รอบที่ 8](02_8_Predict_Class_Func.ipynb)
- classifier accuracy = 86.96 %
- MAE: 0.16760564975753514
- MSE: 0.10294154264012242
- RMSE: 0.3208450445933713

### [Train รอบที่ 9 (250 epochs, Unfreeze)](02_9_Func_Eff_Classification_Train_250_Unfreeze.ipynb)
```
learning_rate= 8e-8
```
#### [Predict รอบที่ 9](02_9_Predict_Class_Func.ipynb)
- classifier accuracy = 87.17%
- MAE: 0.16835615138141136
- MSE: 0.10422516916178248
- RMSE: 0.3228392311380116
  
- ![image](https://github.com/natthanich/EfficientNet_Classification_DeepTooth/assets/108257658/2394dc36-e435-4717-81c6-3d821a19be1c)

