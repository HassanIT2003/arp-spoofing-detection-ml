# 🧠 ARP Spoofing Detection Using Machine Learning  
> *Developed by Muhammad Hassan Noonari*  
> SIT327 – Network Forensics (HD Project 2025)

![Python](https://img.shields.io/badge/Python-3.8-blue)
![Scapy](https://img.shields.io/badge/Scapy-Network_Toolkit-orange)
![TensorFlow](https://img.shields.io/badge/TensorFlow-ML_Framework-red)
![Keras](https://img.shields.io/badge/Keras-Deep_Learning-yellow)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 🌐 Overview

This project is a **Machine Learning-based system to detect ARP spoofing (poisoning) attacks**, simulating real-world network threats. It demonstrates how packet capture data can be used to train intelligent models that analyze network behavior, identify anomalies, and alert network defenders in real time.

🚀 **Languages & Tools**: Python 3, Scapy, TensorFlow, Keras  
🛡️ **Focus**: Network forensics, ARP spoofing, packet classification  
📘 **Use Case**: Academic research, cybersecurity education, and ML-based intrusion detection systems.

---

## 🎯 Objectives

- ✅ Detect ARP spoofing attempts using supervised learning.
- 📊 Train classifiers on extracted PCAP features (packet metadata).
- ⚙️ Automate forensic analysis using intelligent detection.
- 🧪 Validate models using metrics like precision, recall, and F1-score.

---

## 📁 Project Structure

```bash
├── data/                         # Training and testing PCAP files
│   ├── poisoning_test.pcap
│   └── training1.pcap - training4.pcap
│
├── features/                     # Feature extraction logic
│   ├── dataset_processing.py
│   └── pcap_classifier.py
│
├── model/                        # ML models and execution
│   ├── model_creator.py
│   ├── main.py
│   └── argument_parser.py
│
├── README.md                     # Project overview (this file)
└── requirements.txt              # Python dependencies
```

---

## ⚙️ How to Use

### 🔧 1. Install Dependencies

Install all required libraries using:

```bash
pip install -r requirements.txt
```

> ✅ Make sure you're using **Python 3.8+** and have a working environment for Scapy, TensorFlow, and Keras.

---

### 🧠 2. Train a Model

Train a model using one of the provided PCAP datasets:

```bash
python model/model_creator.py --train data/training1.pcap
```

You can substitute `training1.pcap` with any other file such as `training2.pcap`, `training3.pcap`, etc.

---

### 🔍 3. Run ARP Spoof Detection

Run detection on a test capture file:

```bash
python model/main.py --input data/poisoning_test.pcap
```

The model will output whether an ARP spoofing attempt is detected based on the PCAP input.

---

## 📊 Evaluation Metrics

The model performance is evaluated using:

- ✔️ **Accuracy**
- 🎯 **Precision & Recall**
- 📈 **F1 Score**
- 📉 **Confusion Matrix**
- 🔍 **ROC Curve**

> These are printed during training and shown in logs when testing the model.

---

## 📚 References

This project is backed by research in the field of ML-based network forensics:

- Sharma & Gupta (2023), *Predicting ARP Spoofing with ML*, IJNS.
- Noor et al. (2023), *Trigger Acquire Analysis Report Action Method*, JCNC.
- Vajrobol et al. (2023), *ML for Spoofing in IoT*, JHSN.
- Kozelko & Tkachuk (2019), *Deep Learning for DNS Spoofing Detection*.

📄 For a full literature review with IEEE-style citations, refer to `HD_Task_Network_Forensic.pdf`.

---

## 👨‍💻 About the Author

**Muhammad Hassan Noonari**  
🎓 Bachelor of Cybersecurity (Deakin University)  
🔒 Network Forensics | Ethical Hacking | AI in Security  
🌐 GitHub: [@yourusername](https://github.com/yourusername)  
📫 Email: *your.email@example.com*

---

## 📄 License

This project is licensed under the **MIT License**.

> You are free to use, modify, and distribute this project for academic, research, or personal use — just give credit where it’s due!
