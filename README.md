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
### [Train รอบที่ 1 (250 epochs, Freeze)](ของรุ่นพี่_Class_1_Train_2e_4_Freeze.ipynb)

#### Train จากชุดข้อมูลใหม่


#### [Train ของรุ่นพี่](https://github.com/Wanita-8943/Main_Project/blob/main/A2_Train_Freeze.ipynb) 

## [Predict รอบที่ 2]()
#### ผลจากชุดข้อมูลใหม่
- classification accuracy: 5.30% 
- MAE: 4.737009544008483
- MSE: 30.04559915164369
- RMSE: 5.481386608481807
- ![image](https://github.com/natthanich/EfficientNet_Deeptooth/assets/108257658/0e258bc2-6310-4b11-977b-c6966b5f423e)


#### [ผลจากรุ่นพี่](https://github.com/Wanita-8943/Main_Project/blob/main/A2_Predict_Freeze.ipynb)
- classification accuracy: 5.26%
- MAE: 4.7368421052631575
- MSE: 30.0
- RMSE: 5.477225575051661
- ![image](https://github.com/natthanich/EfficientNet_Deeptooth/assets/108257658/c50e3a61-147e-494c-b6d7-57b9ce1e798d)

