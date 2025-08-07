Bachelorarbeit/
├── DMP.md #Datenmanagementplan
├── Dataset_MetaData.md #Metadaten von Datensatz  
├── EDA/
│   ├── EDA.ipynb #Code zur explorative Datenanalyse
│   ├── features.csv #Originaler Datensatz: Features
│   └── targets.csv #Originaler Datensatz: Target
├── Modelle/
│   ├── Modellvergleich.ipynb # Code zur Vergleichung der Modellperformancen
│   ├── Entscheidungsbaum/
│   │   ├── decision_tree.pkl #Modell-Datei
│   │   └── Entscheidungsbaum.ipynb
│   ├── KNN-Model/
│   │   ├── KNN.ipynb
│   │   └── knn.pkl #Modell-Datei  
│   ├── LogReg-Model/
│   │   ├── LogReg.ipynb
│   │   └── logreg.pkl #Modell-Datei
│   └── Random_Forest/
│       ├── RF.ipynb
│       └── rf.pkl #Modell-Datei
├── Resampling/
│   ├── Preprocessing.ipynb # Code der Preprocessing
│   ├── X_test.csv #originale Testdaten X
│   ├── X_test_ros.csv #skalierte Testdaten nach ROS X
│   ├── X_test_stm.csv #skalierte Testdaten nach STM X
│   ├── X_train.csv #originale Trainingsdaten X
│   ├── X_train_ros.csv #resampelte Trainingsdaten mit RandomOverSampler X
│   ├── X_train_stm.csv #resampelte Trainingsdaten mit SMOTETomek X
│   ├── X_val.csv #originale Validierungsdaten X
│   ├── X_val_ros.csv #skalierte Validierungsdaten nach ROS X
│   ├── X_val_stm.csv #skalierte Validierungsdaten nach SMT X
│   ├── y_test.csv #originale Testdaten y
│   ├── y_train.csv #originale Trainingsdaten y
│   ├── y_train_ros.csv #skalierte Trainingsdaten nach ROS y
│   ├── y_train_stm.csv #skalierte Trainingsdaten nach STM y
│   └── y_val.csv #originale Validierungsdaten y
└── xAI/
    ├── shap_explainer.joblib #exportierte Shap_explainer von RandomForest SHAP
    ├── shap_values.joblib #exportierte Shap_value von RandomForest SHAP
    ├── xAI_Entscheidungsbaum.ipynb #Code zum Einsatz von xAI auf Entscheidungsbaum
    ├── xAI_kNN.ipynb #Code zum Einsatz von xAI auf kNN
    ├── xAI_LogReg.ipynb # Code zum Einsatz von xAI auf Logistische Regression
    └── xAI_RF.ipynb # Code zum Einsatz von xAI auf Random Forest
