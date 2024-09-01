

# UNSW-NB15 Cybersecurity Attack Classification

This repository contains the code for classifying cybersecurity attacks using the UNSW-NB15 dataset. The project leverages a combination of Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) networks for the classification of various attack categories.

## Table of Contents

- [Dataset](#dataset)
- [Installation](#installation)
- [Model Architecture](#model-architecture)
- [Training](#training))
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Dataset

The dataset used in this project is the UNSW-NB15 dataset. It consists of various types of network traffic, categorized into different attack types:

- **Normal**
- **Reconnaissance**
- **Backdoor**
- **DoS**
- **Exploits**
- **Analysis**
- **Fuzzers**
- **Worms**
- **Shellcode**
- **Generic**

The dataset is split into four CSV files and includes features like `service`, `state`, `ct_flw_http_mthd`, `is_ftp_login`, and more.

## Installation

To run this project, you will need to install the following dependencies:

```bash
pip install pandas numpy tensorflow scikit-learn seaborn matplotlib
```

You can clone this repository and set up the environment using the following commands:

```bash
git clone https://github.com/saadnaveeddev/unsw-nb15-cybersecurity-classification.git
cd unsw-nb15-cybersecurity-classification
```

## Model Architecture

The model architecture consists of a combination of Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) layers. The architecture includes:

- Conv1D and MaxPooling1D layers for feature extraction
- BatchNormalization for stabilizing and accelerating the training process
- LSTM layers for sequential data processing
- Dense layers for final classification

The model is compiled with the Adam optimizer and `categorical_crossentropy` loss function.

## Training

To train the model, use the following script:

```python
history = model.fit(x_train, y_train, epochs=5, batch_size=256, validation_data=(x_val, y_val))
```

This will train the model on the training dataset and validate it on the validation dataset.



## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue for any bug fixes, improvements, or suggestions.

## License

This project is licensed under the MIT License

## Contact

For any inquiries, please reach out to Saad Naveed at saad.naveed.dev@gmail.com.

---
