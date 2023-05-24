# Daedalus

This is an updated version of the code required to run Daedalus in 2023.

Daedalus is an attack method on object detection originally proposed in the paper "Daedalus: Breaking Non-Maximum Suppression in Object Detection via Adversarial Examples".

Since the original paper, both the YOLO object detection model, and Tensorflow have received major updates, rendering the original Daedalus source code somewhat obsolete.

During my research for my bachelor's thesis "Adversarial attacks on road sign detectors", I set out to update the Daedalus attack to make it easier to use. The main aim of the repository is to execute the Daedalus attack in Google Colab for free GPU usage and skipping dependency installations on your own environment.

## Usage

1. Clone the repository into Google Colab.
2. Execute the notebook.

## Branch-specific information

To run YOLOv3, the original pre-trained model that the original source code recommends is being used. In the source code, I have made it download the model from my personal Google Drive for ease of use, but, if you find that the file can't be downloaded, check out the original Daedalus repository (see _Credits_) to get their download link.

As Google has dropped all support for Tensorflow 1 and older versions of Python in Colab, the main notebook installs a virtual environment with an older Python version, as well as older versions of Tensorflow, Keras and H5Py to ensure compatibility with the original source code. Because of this, all code execution of Daedalus is done using shell commands from within Colab.

## Credits

The original Daedalus research paper.

```text
@artical{9313033,
author={Wang, Derui and Li, Chaoran and Wen, Sheng and Han, Qing-Long and Nepal, Surya and Zhang, Xiangyu and Xiang, Yang},
journal={IEEE Transactions on Cybernetics},
title={Daedalus: Breaking Nonmaximum Suppression in Object Detection via Adversarial Examples},
year={2021},
volume={},
number={},
pages={1-14},
doi={10.1109/TCYB.2020.3041481}}
```

The original Daedalus implementation repository - <https://github.com/NeuralSec/Daedalus-attack>
