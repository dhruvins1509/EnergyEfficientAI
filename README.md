# EnergyEfficientAI
Compare model compression methods (quantization, pruning, distillation) on a deep neural network.



## Project Overview
This project compares different **model compression methods**—**quantization**, **pruning**, and **knowledge distillation (KD)**—on deep neural networks using the **CIFAR-10 dataset**.  
It focuses on evaluating the trade-offs between:

- **Model size**  
- **Computational efficiency**  
- **Accuracy**  

---

## Installation

1. Make sure you have Python 3.8 or higher installed.  
2. Install the required Python libraries using the provided `requirements.txt`:


bash
pip install -r requirements.txt


---

## Project Structure

```
.
├── Baseline_Model_Training.ipynb     # Train ResNet-18 and WideResNet-28-10 models
├── Model_Pruning.ipynb               # Apply pruning to compress models
├── Model_Quantization.ipynb          # Apply quantization
├── Knowledge_Distillation.ipynb      # Apply knowledge distillation (KD)
├── wide_resnet28_10.py               # WideResNet-28-10 architecture used in notebooks
├── requirements.txt                  # Required Python libraries
└── README.md                         # Project overview and instructions
```

---

## Usage Instructions

Run the notebooks in the following sequence for correct workflow:

1. **Baseline_Model_Training.ipynb**

   * Trains baseline models: ResNet-18 and WideResNet-28-10.
2. **Model_Pruning.ipynb**

   * Applies pruning to reduce model parameters.
3. **Model_Quantization.ipynb**

   * Performs quantization to reduce model size and improve efficiency.
4. **Knowledge_Distillation.ipynb**

   * Trains a student model using knowledge distillation.

> The file `wide_resnet28_10.py` contains the WideResNet-28-10 architecture used in both baseline training and KD notebooks.

---

## Flow Diagram

```text
Baseline_Model_Training.ipynb
            ↓
     Model_Pruning.ipynb
            ↓
   Model_Quantization.ipynb
            ↓
 Knowledge_Distillation.ipynb
```

---

## Author

**Dhruvin Sojitra**
📧 Email: [dhruvin.sojitra@hof-university.de](mailto:dhruvin.sojitra@hof-university.de)

---

## References

* CIFAR-10 Dataset: [https://www.cs.toronto.edu/~kriz/cifar.html](https://www.cs.toronto.edu/~kriz/cifar.html)
