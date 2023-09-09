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
### [Train รอบที่ 1 (250 epochs, Freeze)]()

#### Train จากชุดข้อมูลใหม่
![image](https://github.com/natthanich/EfficientNet_Deeptooth/assets/108257658/364c2adb-6d7e-415a-8400-3a79c544e4e2)
![image](https://github.com/natthanich/EfficientNet_Deeptooth/assets/108257658/70e9cfe7-5e7b-4795-9eff-c31009da653a)

#### [Train ของรุ่นพี่](https://github.com/Wanita-8943/Main_Project/blob/main/A2_Train_Freeze.ipynb) 
![image](https://github.com/natthanich/EfficientNet_Deeptooth/assets/108257658/3f103b80-8a95-4704-9ed6-362ef9bc80df)
![image](https://github.com/natthanich/EfficientNet_Deeptooth/assets/108257658/ee64b657-4d78-43bd-b43b-866d9003a7f8)

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

