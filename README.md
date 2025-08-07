# Datenmanagementplan

## Administrative Informationen

**Projekttitel:** BA - Transparente KI in der Medizin: Bewertung der Zuverlässigkeit und Erklärbarkeit von KI-Modellen zur Diabetes-Diagnose

**Projektbeschreibung:** 
Diese Projekt untersucht systematisch die Performance von KI-Modellen in der Diabetes-Diagnose. Der Schwerpunkt liegt dabei auf zwei Aspekten: die Performance von KI-Modellen und der Erklärbarkeit ihrer Vorhersagen durch Anwendung von xAI-Methoden zu untersuchen.

## Autor*innen

**Author:** Hai Hung Nguyen

**Betreurer:** Prof. Dr. Martin Spott, Prof. Dr. Ingo Claßen

**Institution:**
Hochschule für Technik und Wirtschaft Berlin
ROR: <https://ror.org/01xzwj424>

## Datensatz

Das US-amerikanische Center for Disease Control and Prevention (CDC) führt seit 1984 die Gesundheitsumfrage „Behavioral Risk Factor Surveillance System“ (BRFSS) durch, bei der jährlich über 400.000 Amerikaner zu gesundheitlichen Risikoverhaltensweisen, chronischen Erkrankungen und ihrem Alltagsverhalten befragt werden. 
Aus dem Jahr 2015, in dem 441.455 Teilnehmer Antworten zu 330 Merkmalen gaben, wurde der spezifische „CDC Diabetes Health Indicators“-Datensatz abgeleitet. 
Dieser für die Arbeit verwendete Datensatz umfasst 253.680 Beobachtungen und konzentriert sich auf 21 Merkmale, die für Diabetes mellitus relevant sind.

**Sprache:** Englisch.

## Datenzugriff und Datenschutz

Datensatz ist von CDC erstellt und zugreifbar unter <https://doi.org/10.24432/C53919>. 

Lizenzvereinbarung: CC0: Public Domain, No Copyright

Das Projekt und die verwendete Daten sollen nach 10 Jahren Aufbewahrungszeit gelöscht werden: 08.08.2035.

## Zeitraum

Die Bearbeitung wurden am 31.05.2025 bis 08.08.2025 durchgeführt.

## Angewendete Software

* Zur Codeverfassung: DataSpell, Python 3.13

## Datenformate

Daten im Projekt liegen in folgenden Formaten vor:

* Code (.ipynb): JupyterNotebook,
* Datensatz (.csv): als separate Datei abgespeichert,
* trainierte Finalmodelle (.pkl): Finale Modell nach Training und Optimierung

## Ablage und Speicherung

Ablageort: <https://github.com/hungnguyen5298/Bachelorarbeit.git>

Ablagestruktur:
```markdown
Bachelorarbeit/
├── DMP.md #Datenmanagementplan = README
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

```
