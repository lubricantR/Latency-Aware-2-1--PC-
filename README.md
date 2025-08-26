# Code for Latency-Aware (2+1)-PC and Its Application to Secure Transformer Inference
Latency-Aware 21PC: Enhanced Transformer Inference
This repository extends the work from the paper "SHAFT: Secure, Handy, Accurate, and Fast Transformer Inference" (GitHub https://github.com/andeskyl/SHAFT/tree/main) to provide latency-aware optimizations for secure transformer inference using CrypTen. Our implementation, housed in the latency_aware_21PC directory, is fully compatible with SHAFT's environment setup and introduces performance enhancements for private inference.
Installation
Our code aligns with SHAFT's environment configuration. Follow SHAFT's setup instructions, then replace the SHAFT directory with our latency_aware_21PC directory. The following steps assume Ubuntu 22.04 with Python 3.10.12.

1. Install Dependencies
pip install torch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2 --index-url https://download.pytorch.org/whl/cu118
pip install wheel==0.40.0

2. Install Latency-Aware 21PC
cd latency_aware_21PC
pip install .


Running Experiments
Our examples directory contains subdirectories for reproducible experiments, with additional dependencies listed in each subdirectory’s requirements.txt. Refer to the README.md in each subdirectory for specific setup and execution instructions. 

The experiments include:

buildingblocktest - Performance of basic building blocks
gelu_gpt2acc - Evaluation of GPT-2's accuracy on wikitext-2 and PTB
text-generation - Assesses private inference costs for GPT-2 with latency improvements.
image-classification - Analyzes private inference costs for ViT-base with enhanced performance.



License
This project is MIT licensed, as found in the LICENSE file.
