# da6401_assignment2
# DA6401 Assignment 2: Training CNNs & Transfer Learning

This repository contains the implementation for **DA6401 – Assignment 2**, which includes:

- **Part A:** Training a CNN from scratch on the iNaturalist dataset
- **Part B:** Fine-tuning a pre-trained model (ResNet-50) on the same dataset

---

## 📁 Folder Structure

```bash
.
├── partA
│   ├── main.ipynb                # CNN from scratch with wandb logging
│   ├── sweep.yaml                # wandb sweep config for Part A
│   
│
├── partB
│   ├── main.ipynb                # Fine-tune pre-trained ResNet50
│
├── README.md
└── requirements.txt
```

---

## 📦 Setup

```bash
# Clone the repo
!git clone https://github.com/Yogesh0arya/da6401_assignment2.git
cd da6401_assignment2

# Install requirements
pip install -r requirements.txt
```

---

## 📌 Dataset

Download the **iNaturalist subset** from: [nature_12K.zip](https://storage.googleapis.com/wandb_datasets/nature_12K.zip)

Extract it into the root folder:
```bash
./inaturalist_12K/
  └── train/
  └── test/
```

---

## 🚀 Part A: Train from Scratch

### Run Training:
```bash
cd partA
jupyter notebook main.ipynb
```

### Run wandb Sweep:
```bash
wandb sweep sweep.yaml
wandb agent <username>/<project>/<sweep-id>
```

---

## 🔁 Part B: Fine-tune Pretrained Model

### Run:
```bash
cd partB
jupyter notebook main.ipynb
```

You can modify the freezing strategy and learning rate in the `wandb.init(config)` block.

---

## 🧪 Report Links

- **wandb Report:** https://api.wandb.ai/links/yogesh084arya-indian-institute-of-technology-madras/x08cvb8q
- **Part A GitHub:** https://github.com/Yogesh0arya/da6401_assignment2/tree/main/partA
- **Part B GitHub:** https://github.com/Yogesh0arya/da6401_assignment2/tree/main/partB

---

## 🧾 Declaration

```
I, Yogesh Arya (Roll No: DA24M028), swear on my honour that I have written the code and the report by myself and have not copied it from the internet or other students.
```

---

## ✨ Credits

Created with ❤️ using PyTorch, Torchvision, and Weights & Biases.

---
