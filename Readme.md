# LLM Qunatization and Inferencing Tool
This repository houses a Python tool designed to qunatize a large language model using different algorithms like BitsandByets, Llama.cpp, AWQ, and Exllamv2.  The repository also helps in storing these quantized model on HuggingFace hub.
The tool also helps in using quantized models for inferencing tasks. 

More details on google slides can be found here (https://docs.google.com/presentation/d/1ag_uVJq7SWWbCd9IEZaEsLFNVeW-yKoqdPObLxCwqbQ/edit?usp=sharing)
 
**This tool is intended for education and informational purposes only. Please use quantized model in production with caution after proper testing.** 

## Features

- **Qunatization**: The notebook covers different algorithms to quantize large language model.
- **Inferencing**: The notebook covers inferencing using different qunatized model.


## How to use 
- **Install required libraries**: use pip install section to install required python packages to run the program.
- **HuggingFace Hub API key**: HuggingFace hub API key is needed to access gater LLM models, to create a model repo, and push the quantized model to the repo. 
- **How to run**: Open Quantizing_LLMs_and_inferencing_Quantized_model_from_HF.ipynb in colab notebook to run the application. You can run specific section of the notebook relevant for qunatization algorithms.

***What is quantization of Large language model?***

Quantization of Large Language Models (LLMs) is a technique used to reduce the computational and memory requirements of these models by converting their weights and activations from a high-precision 32-bit floating-point representation to a lower-precision format such as 8-bit or 4-bit integers. This process allows LLMs to be more efficiently run on hardware with limited computational resources, including mobile and IoT devices, without significantly compromising LLM’s performance or accuracy.

***What are the benefits of quantization in large language models***
- Reduced Model Size / Memory Footprint
- Faster Inference Speed / Increased Efficiency
- Lower Power Consumption / Energy Efficiency - Suitable for mobile devices
- Model Compression and Portability

***What are different quantization techniques?***
- Post-Training Quantization (PTQ)
- Quantization-Aware Training (QAT)
- Activation-Aware Weight Quantization (AWQ)
- NF4 Quantization - BitsAndBytes
- etc.

***Different Options for Quantization:***
- 16-bit (Float16)
- 8-bit (Int8): for deploying models on edge devices or situations where computational resources are limited
- 4-bit: Useful for extremely resource-constrained environments
- 1-bit (Binary)
- NF4 (4bit-NormalFloat): A specialized 4-bit format designed to efficiently represent a larger bit datatype. It includes steps like normalization, quantization, and dequantization to efficiently represent original 32-bit weights.Suitable for applications requiring a balance between model size reduction and maintaining higher accuracy than traditional 4-bit quantization.
- etc.
