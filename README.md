# Physics-Informed Neural Networks & ML Controllers for Vehicle Dynamics  

This project explores **state prediction using Physics-Informed Neural Networks (PINNs)** and **machine learning–based control methods** for vehicle dynamics in the autonomous driving domain.  

The goal is to:  
1. Predict vehicle states (position, velocity, yaw rate, etc.) using PINNs.  
2. Compare PINNs with standard neural networks.  
3. Implement classical controllers (PID, MPC) for trajectory following.  
4. Develop ML-based controllers (Imitation Learning, Reinforcement Learning).  

---

##  Project Structure  

```
vehicle-dynamics-ml/
│── README.md                # Project overview
│── requirements.txt         # Python dependencies
│── .gitignore               # Ignore cache, venv, data
│
├── src/                     # Source code
│   ├── models/              # Neural nets & PINNs
│   │   ├── baseline_nn.py
│   │   ├── pinn.py
│   │
│   ├── controllers/         # Classical & ML controllers
│   │   ├── pid.py
│   │   ├── mpc.py
│   │   ├── imitation.py
│   │   ├── rl_agent.py
│   │
│   ├── simulation/          # Vehicle models & environment
│   │   ├── bicycle_model.py
│   │   ├── utils.py
│   │
│   └── training/            # Training scripts
│       ├── train_baseline.py
│       ├── train_pinn.py
│       ├── train_imitation.py
│       ├── train_rl.py
│
├── notebooks/               # Jupyter notebooks for experiments
│   ├── 01_vehicle_dynamics.ipynb
│   ├── 02_nn_vs_pinn.ipynb
│   └── 03_controllers.ipynb
│
├── data/                    # Simulation datasets
│   └── sample_data.csv
│
└── results/                 # Plots, logs, and animations
    ├── predictions/
    ├── controllers/
    └── animations/
```

---

## Getting Started  

### 1️ Clone the repository
```bash
git clone https://github.com/RoyEl23/Motion_Prediction_of_Automated_Vehicle-master.git
cd vehicle-dynamics-ml
```

### 2️ Create a virtual environment
```bash
python -m venv venv
venv\Scripts\activate   # Windows
source venv/bin/activate # Mac/Linux
```

### 3️ Install dependencies
```bash
pip install -r requirements.txt
```

---

## Dependencies  

- `numpy` – numerical computations  
- `scipy` – scientific functions  
- `matplotlib` – plotting and visualization  
- `torch` – neural networks (PyTorch)  
- `gymnasium` – reinforcement learning environments  
- `stable-baselines3` – RL algorithms (PPO, DDPG, etc.)  
- `cvxpy` – optimization for MPC  

---

## Roadmap  

- ✅ Week 1: Vehicle dynamics simulation (kinematic bicycle model)  
- ✅ Week 2: Baseline NN for state prediction  
- ✅ Week 3: PINNs for improved prediction  
- ✅ Week 4: Classical controllers (PID, MPC)  
- ✅ Week 5: ML-based controllers (IL, RL)  
- ✅ Week 6: Experiments & results  

---

## Results (to be added)  

- PINN vs NN prediction accuracy  
- Controller performance (tracking error, smoothness)  
- Visualizations and animations  

---

## 📝 License  

This project is open source under the [MIT License](LICENSE).  
