Titanic Survival Prediction 

 Project Overview
Σε αυτό το project αναλύουμε το κλασικό Titanic dataset και φτιάχνουμε ένα Machine Learning μοντέλο που προβλέπει αν ένας επιβάτης επέζησε ή όχι.

 Βήματα
1. Φόρτωση dataset (Titanic CSV).
2. Εξερεύνηση δεδομένων (EDA) με pandas & seaborn.
3. Καθαρισμός δεδομένων:
   - Αντικατάσταση missing values (`Age`, `Embarked`).
   - Αφαίρεση `Cabin` (πολλά κενά).
   - One-hot encoding για κατηγορικές μεταβλητές (`Sex`, `Embarked`).
   - Drop irrelevant στήλες (`Name`, `Ticket`, `PassengerId`).
4. Machine Learning Pipeline:
   - Features = Age, Pclass, Sex, SibSp, Parch, Fare, Embarked.
   - Target = Survived.
   - Train/Test split.
   - Logistic Regression μοντέλο.
5. Αξιολόγηση:
   - Accuracy score.
   - Classification report.
   - Confusion matrix visualization.

 Αποτελέσματα
Το Logistic Regression πέτυχε ~80% accuracy στο test set, δείχνοντας ότι τα χαρακτηριστικά όπως Sex και Pclass είναι κρίσιμα για την επιβίωση.

 Libraries
- pandas, numpy
- seaborn, matplotlib
- scikit-learn

 Επόμενα Βήματα
- Δοκιμή πιο σύνθετων μοντέλων (Random Forest, XGBoost).
- Feature engineering (π.χ. οικογένεια, τίτλος από Name).
- Hyperparameter tuning.
