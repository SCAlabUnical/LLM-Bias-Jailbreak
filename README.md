# Are Large Language Models _Really_ Bias-Free? Jailbreak Prompts for Assessing Adversarial Robustness to Bias Elicitation

## Overview

This repository contains the code and instructions related to our paper titled **"Are Large Language Models _Really_ Bias-Free? Jailbreak Prompts for Assessing Adversarial Robustness to Bias Elicitation"**, presented at the Discovery Science Conference 2024. Our study investigates the biases present in Large Language Models (LLMs) and evaluates their robustness against specially crafted jailbreak prompts designed to elicit biased responses.

## Abstract

Large Language Models (LLMs) have revolutionized artificial intelligence, demonstrating remarkable computational power and linguistic capabilities. However, these models are inherently prone to various biases stemming from their training data. These include selection, linguistic, and confirmation biases, along with common stereotypes related to gender, ethnicity, sexual orientation, religion, socioeconomic status, disability, and age. This study explores the presence of these biases within the responses given by the most recent LLMs, analyzing the impact on their fairness and reliability. We also investigate how known prompt engineering techniques can be exploited to effectively reveal hidden biases of LLMs, testing their adversarial robustness against jailbreak prompts specially crafted for bias elicitation. Extensive experiments are conducted using the most widespread LLMs at different scales, confirming that LLMs can still be manipulated to produce biased or inappropriate responses, despite their advanced capabilities and sophisticated alignment processes. Our findings underscore the importance of enhancing mitigation techniques to address these safety issues, toward a more sustainable and inclusive artificial intelligence.
## Repository Contents

This repository includes the following Python files:

1. **`bias_prompting.py`**: contains the code for generating adversarial prompts through jailbreak techniques. Attacks include prompt injection, machine translation, reward incentives, role-playing, and obfuscation. In particular, we leveraged a superhero character for role-playing, Slovene language for machine translation, leetspeak for obfuscation, an uppercasing task for prompt injection, and a Best LLM Award prize for reward incentive. 

2. **`main.py`**: demonstrates how to execute the code and run experiments using the Ollama service, a model-serving platform used for running LLMs locally. To use Ollama locally, follow these steps:
   1. **Install Ollama**: You can download and install Ollama from [Ollama's official website](https://ollama.com/download).
   2. **Start the Ollama Service**: Open a terminal and run the following command to start the Ollama service:
   ```bash
   ollama serve
   ```
   3. **Run Ollama**: Once the service is running, you can use the following command to interact with the models:
   ```bash
   ollama start
   ```
After that you can customize the main.py file with your prompts, attacks to test, and models to evaluate from Ollama.

## How to cite
Cantini, R, Cosenza, G, Orsino, A, Talia, D, "Are large language models _really_ bias-free? Jailbreak prompts for assessing adversarial robustness to bias elicitation". Discovery Science 2024.

## Acknowledgements
This work has been supported by the "FAIR – Future Artificial Intelligence Research" project - CUP H23C22000860006.
