## NBA MVP Prediction with Machine Learning

This project uses machine learning to predict the NBA Most Valuable Player (MVP) based on 16 seasons of player data. The code is implemented in Google Colab, and the models include Logistic Regression, KNN, SVM, Random Forest, AdaBoost, Gradient Boosting, LightGBM, and XGBoost.

### Files
- `nba_mvp_prediction.ipynb` – Colab notebook with all code and model evaluation
- `NBA_MVP_Paper.pdf` – Full research paper detailing methods, results, and conclusions

### Summary
We trained models on over 400 players using per-game, advanced, and physiological stats along with MVP vote shares. SVM and Random Forest achieved the best results in predicting MVP rankings.

### How to Run
Open the notebook in Google Colab and run each cell in order. The notebook includes data cleaning, model training, evaluation, and visualizations.

### Future Work
- Use real-time season updates
- Add explainability tools like SHAP
- Extend to other awards (e.g., DPOY, ROTY)
