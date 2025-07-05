# formula1-finish-position-predictor
Built a Python-based Formula 1 driver performance prediction system using 9 linked F1 datasets. Cleaned and merged driver, constructor, race, and results data to train a machine learning model that predicts a driver’s finishing position. Implemented as a terminal app for user input and output.
## 📂 **Datasets Used**

The project combines and processes:
- **drivers** — Driver information
- **constructors** — Constructor/team details
- **races** — Race information
- **results** — Actual race results
- **qualifying** — Qualifying session details
- **lap_times** — Lap-by-lap times
- **pit_stops** — Pit stop records
- **driver_standings** — Championship points for drivers
- **constructor_standings** — Constructor points

---

## ⚙️ **Workflow**

**1️⃣ Load and Validate**  
- Checks if all required dataset files exist.
- Loads CSV files using `pandas`.

**2️⃣ Clean and Preprocess**  
- Handles missing values and inconsistencies.
- Converts categorical data using `LabelEncoder`.
- Scales numerical features using `StandardScaler`.

**3️⃣ Train the Model**  
- Selects and merges relevant features.
- Trains a regression model (e.g., Linear Regression, Random Forest) to predict finishing position.
- Saves the trained model using `pickle`.

**4️⃣ Predict in Terminal**  
- Loads the saved model.
- Takes 14 user input features in the terminal.
- Predicts and displays the expected finishing position.

## 🛠️ **Key Technologies**

- **Python 3**
- **TensorFlow** and **Keras** for building and training neural networks
- **Keras Tuner** for hyperparameter tuning
- `pandas`, `numpy` for data processing
- `pickle` or `joblib` for model saving (if used)
- Terminal-based user input/output
