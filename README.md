# NIMS-AI

Detect & Cleanse backdoor triggers in neural network models

## 👀 Overview

### Backdoor Trigger

![KakaoTalk_Photo_2023-12-10-01-26-38 001](https://github.com/BluberryPie/NIMS-AI/assets/63835339/fc880bb6-8239-48b2-bdd2-92436f3c28f2)

### Sample - Poisoned Image

![KakaoTalk_Photo_2023-12-10-01-26-39 002](https://github.com/BluberryPie/NIMS-AI/assets/63835339/4cf8de77-1682-4de9-9c5b-c9d23011a890)

### Reversed Trigger

![trigger](https://github.com/BluberryPie/NIMS-AI/assets/63835339/ed6d588e-d97e-4571-8e76-c9104e38a7ae)

### Demo

https://github.com/BluberryPie/NIMS-AI/assets/63835339/106476cb-730d-47a1-a29b-da1b789fb090

## 🏃🏻‍♂️ Run Notebooks

1. `Talpiot_NIMS_Poison.ipynb`
    - (Input) `train`, `test` data
    - (Output) Poisoned model (`model-{xxx}.pt`)

2. `Talpiot_NIMS_Detect.ipynb`
    - (Input) `train` data, poisoned model (`model-{xxx}.pt`)
    - (Output) Reversed trigger (`mask.pt`, `delta.pt`)

3. `Talpiot_NIMS_Cleanse.ipynb`
    - (Input) `train`, `test` data, poisoned model (`model-{xxx}.pt`)
    - (Output) Cleansed model (`model-clean-{xxx}.pt`)
