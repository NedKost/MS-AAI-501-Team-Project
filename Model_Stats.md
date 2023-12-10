## Model performance statistics

| Model Name          | Feature Set | Dataset                | AUC    | F1     | Accuracy |
|---------------------|-------------|------------------------|--------|--------|----------|
| Neural Net          | 1           | Subset_no_weather      | 0.6225 | 0.5704 | 0.5848   |
| Neural Net          | 1           | Subset_weather         | 0.6401 | 0.5861 | 0.5980   |
| Neural Net          | 1           | All_balanced           | 0.6849 | 0.4936 | 0.6656   |
| Neural Net          | 1 & 2       | Subset_no_weather      | 0.9578 | 0.8991 | 0.9026   |
| Neural Net          | 1 & 2       | Subset_weather         | 0.9579 | 0.8987 | 0.9021   |
| Neural Net          | 1 & 2       | All_balanced           | 0.9644 | 0.8926 | 0.9184   |
| Random Forest       | 1           | Subset                 | 0.6889 | 0.6303 | 0.6368   |
| Random Forest       | 1           | Subset                 | 0.6534 | 0.6022 | 0.6108   |
| Random Forest       | 1           | All_balanced           | 0.7372 | 0.5831 | 0.6916   |
| Random Forest       | 1 & 2       | Subset_no_weather      | 0.9610 | 0.9029 | 0.9057   |
| Random Forest       | 1 & 2       | Subset_weather         | 0.9633 | 0.9027 | 0.9057   |
| Random Forest       | 1 & 2       | All_balanced           | 0.9693 | 0.8979 | 0.9208   |
| XGBoost Classifier  | 1, 2 & 3    | Subset                 | 0.9683 | 0.9118 | 0.9135   |
| XGBoost Classifier  | 1           | Subset                 | 0.6919 | 0.6398 | 0.6334   |
| XGBoost Classifier  | 1           | Full Dataset           | 0.7380 | 0.5471 | 0.6931   |