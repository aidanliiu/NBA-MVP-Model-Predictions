## NBA MVP Prediction with Machine Learning

This project uses multiple machine learning algorithms to predict the NBA Most Valuable Player (MVP) based on 16 seasons of player data. It was built and tested in Google Colab, and supported by a full research paper. The goal is to evaluate which models best capture MVP voting patterns using historical performance statistics and physiological data.

### Files
- `nba_mvp_prediction.ipynb` – Google Colab notebook with all code: data cleaning, model training, evaluation, and visualizations
- `NBA_MVP_Paper.pdf` – Full research paper detailing methodology, experiments, and results

### Background
The NBA MVP award is one of the most prestigious honors in professional sports. However, its selection is subjective and influenced by many factors beyond raw stats. This project attempts to quantify MVP selection using machine learning models trained on past seasons. The models evaluate how well player stats and physical attributes predict MVP vote shares.

### Data
We use three main datasets:
- **Player performance statistics**: Per-game, advanced, and total stats (e.g., points, assists, FG%, PER)
- **Physiological data**: Height and weight
- **MVP voting records**: Vote shares and rankings from 2006 to 2022

After filtering players by criteria such as minutes played, points per game, team success, and vote share, the data is cleaned and merged into a final dataset used for training.

### Models Used
The following machine learning models were tested and compared:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Random Forest
- AdaBoost
- Gradient Boosting
- LightGBM
- XGBoost

Each model was evaluated using root mean squared error (RMSE) and R² score. Hyperparameter tuning was done using `GridSearchCV`.

### Sample Results: 2021–22 Season

| Player           | Actual MVP Share | SVM  | Random Forest | KNN  | XGBoost |
|------------------|------------------|------|----------------|------|---------|
| Nikola Jokic     | 0.875            | 0.83 | 0.85           | 0.70 | 0.63    |
| Joel Embiid      | 0.706            | 0.69 | 0.71           | 0.52 | 0.39    |
| Giannis Antetokounmpo | 0.595      | 0.61 | 0.58           | 0.32 | 0.38    |

SVM and Random Forest were the most consistent and accurate in ranking top MVP candidates. Models like AdaBoost and Gradient Boosting tended to underestimate vote shares.

### How to Run
1. Download or clone this repository.
2. Open `nba_mvp_prediction.ipynb` in Google Colab.
3. Run the notebook top to bottom to clean the data, train models, and see performance results.

Or click here to open directly in Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/YOUR_REPO_NAME/blob/main/nba_mvp_prediction.ipynb)

Replace `YOUR_USERNAME` and `YOUR_REPO_NAME` in the link above with your actual GitHub info.

### Future Work
- Add real-time season updates for live predictions
- Incorporate advanced player metrics like RAPTOR and EPM
- Improve model interpretability using SHAP or LIME
- Expand predictions to other awards (e.g., DPOY, Sixth Man)

### Citation
If you use or reference this project, please cite:

**"Determining the NBA MVP Outcome Using Machine Learning Models" (2025)**

---

This project demonstrates how machine learning can be applied to complex, subjective sports awards like MVP selection. It also highlights the value of combining performance stats with model evaluation to better understand voting behavior.
