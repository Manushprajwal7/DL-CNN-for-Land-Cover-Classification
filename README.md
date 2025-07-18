# ⚖️ AI-Driven Load Balancer for Web Server Optimization

A machine learning-based platform for **intelligent web traffic load balancing** across multiple servers using **Q-Learning** and **Random Forests**. This hybrid system is designed to reduce server overload, enhance response time, and balance incoming requests dynamically.

---

## 🚀 Features

- 📈 **Real-time Traffic Load Simulation**
- 🧠 **Q-Learning Agent** for adaptive server selection
- 🌲 **Random Forest Classifier** for static pattern prediction
- 📊 **Comparative Analysis** between RL and ML models
- 🔍 **Feature Importance** visualization
- 📉 **Load Standard Deviation Metrics** to evaluate balancing
- 📎 **Interactive Plots & Heatmaps**

---

## 🧠 Algorithms Used

### 🔁 Q-Learning (Reinforcement Learning)
- Adaptive policy learning
- Dynamic state-action updates
- Balancing efficiency as reward signal

### 🌲 Random Forest (Supervised Learning)
- Classification of best server action
- Feature importance extraction
- Fast inference with high accuracy

---

## 🛠️ Tech Stack

| Component      | Tools / Libraries                     |
|----------------|----------------------------------------|
| Language       | Python 🐍                              |
| ML Libraries   | `Scikit-learn`, `TensorFlow`, `Keras` |
| RL Logic       | Custom Q-Learning Algorithm            |
| Visualization  | `Matplotlib`, `Seaborn`                |
| Data Handling  | `Pandas`, `NumPy`                      |

---

## 📁 Project Structure

load-balancer-ml/
├── loadbalencerml_model.py # Main ML + RL training & evaluation script
├── synthetic_load_balancing_data.csv # Input dataset
├── *.png # Output plots (heatmaps, metrics)
├── model_comparison.csv # Summary table of metrics

yaml
Copy
Edit

---

## 📊 Dataset Description

A **synthetic dataset** simulating 3-server load conditions with features like:
- `Server1_Load`, `Server2_Load`, `Server3_Load`
- `Avg_Load`, `Load_StdDev`
- `Best_Server_Action` (target)
- Engineered features: `Load_Range`, `Load_Imbalance_Score`, etc.

---

## 📦 Installation & Setup

### 🔧 Prerequisites

- Python 3.7+
- Recommended: Create a virtual environment

### 🔽 Install dependencies

```bash
pip install -r requirements.txt
(Manually install: numpy, pandas, matplotlib, seaborn, scikit-learn)

▶️ How to Run
bash
Copy
Edit
python loadbalencerml_model.py
This will:

Load and preprocess the dataset

Train Q-Learning and Random Forest models

Generate evaluation plots

Print summary metrics

📈 Output Visualizations
load_distributions.png: Server load histograms

correlation_heatmap.png: Feature correlation

q_learning_training_history.png: Rewards and efficiency over time

q_table_heatmap.png: Q-Table heatmap

rf_confusion_matrix.png: RF prediction performance

feature_importance.png: RF feature weights

accuracy_by_load.png: Accuracy under different load conditions

load_balancing_simulation.png: Live server load comparison

📊 Performance Summary
Metric	Q-Learning	Random Forest
Accuracy (on dataset)	~89%	~94%
Training Time	~4.5 seconds	~2.0 seconds
Load Balancing Efficiency	✅ Adaptive	✅ Static

🧠 Learnings & Insights
Q-Learning adapts better to real-time load fluctuations.

Random Forest performs well in static load environments.

Hybrid models can enhance robustness.

Load_Imbalance_Score is a critical KPI for balancing.

📌 Recommendations
✅ Use RF in stable environments.

🔄 Use Q-Learning for real-time, dynamic systems.

⚙️ Monitor Load_StdDev and Load_Imbalance_Score continuously.

🤝 Future work: deploy as a microservice for live traffic balancing.

🤝 Contributing
Feel free to fork the repo, make enhancements, and submit PRs.

bash
Copy
Edit
git checkout -b feature/my-feature
git commit -m "Add my feature"
git push origin feature/my-feature
📬 Contact
Manush Prajwal
📧 Email: manushprajwal555@gmail.com
📂 Repo: GitHub - Load Balancer ML

Built with ❤️ for optimized infrastructure.
