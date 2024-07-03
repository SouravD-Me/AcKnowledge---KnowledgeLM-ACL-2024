# AcKnowledge: Acquired Knowledge Representation by Small Language Model Without Pre-training

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

![Fundamental illustration of AcKnowledge: Representing acquired knowledge through user questions and feedback.](https://github.com/SouravD-Me/AcKnowledge---KnowledgeLM-ACL-2024/blob/main/AcKnowledge%20at%20a%20Glance.png)

## Table of Contents

- [Introduction](#introduction)
- [Theme](#theme)
- [Key Features](#key-features)
- [System Framework](#system-framework)
- [Performance Evaluation](#performance-evaluation)
- [Usage](#usage)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)
- [Contact](#contact)

## Introduction

Welcome to the repository for **AcKnowledge**, a groundbreaking framework designed to address the limitations of large language models (LLMs) in open-domain question-answering (QA) tasks. This project has been accepted at the ACL 2024 Workshop on Towards Knowledgeable Language Models.

AcKnowledge introduces a novel approach to knowledge representation using a small, non-pre-trained language model (SLM) that dynamically acquires and represents knowledge from the internet, bypassing the need for extensive pre-training. The framework leverages meta-learning and user feedback to ensure the accuracy and relevance of the information provided.

## Theme

Large language models (LLMs) are pre-trained on enormous amounts of text data and show acclaimed success in knowledge representation. However, there are two bottlenecks with this approach:
1. Pre-training data cannot be regularly updated once the models are deployed, limiting the model's ability to represent updated knowledge.
2. The consistently increasing size and computational resources make it difficult for non-commercial and individual researchers to fine-tune and scale these language models.

To address these issues, AcKnowledge proposes a framework wrapped around a small, non-pre-trained language model for an open-domain QA experiment. AcKnowledge learns relevant knowledge from the internet via meta-learning based on user questions and re-learns from user feedback if knowledge is misrepresented. This efficient knowledge representation framework avoids pre-training overhead while enabling updated information.

## Key Features

- **Dynamic Knowledge Acquisition**: Utilizes real-time web search and meta-learning to acquire new information efficiently.
- **User Feedback Integration**: Enhances answer reliability and accuracy through iterative learning based on user feedback.
- **Cost-Effective**: Operates without the need for extensive pre-training, making it accessible to non-commercial and individual researchers.
- **Competitive Performance**: Demonstrates competitive performance against similarly sized state-of-the-art LLMs on gold standard QA datasets.

## System Framework

AcKnowledge comprises several key components that work in tandem to facilitate dynamic knowledge retrieval and adaptation:
1. **Answer Retrieval from Internet Search**: Uses Latent Dirichlet Allocation (LDA) for topic extraction from user questions, followed by a targeted online search to retrieve relevant passages.
2. **Meta-Learning for Search Results**: Employs the Model-Agnostic Meta-Learning (MAML) algorithm to adapt the language model to the retrieved passages and improve answer accuracy.
3. **Language Model Development**: Builds on the transformer architecture, with a multi-layer encoder and decoder to process input keywords and generate corresponding answers.

## Performance Evaluation

Extensive benchmarking against similar language models in open-domain QA tasks demonstrates AcKnowledge's competitive performance. The framework's ability to adapt to new information without relying on pre-training showcases its potential for efficient QA.

## Usage

**Note**: The source code is currently not available as we are addressing the reviewers' comments to modify the work. The source code will be added very soon. Please keep an eye on this space for updates. Feel free to fork the repository and watch for new releases.

To use AcKnowledge, follow these steps (once the code is available):

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/AcKnowledge.git
    ```
2. Install the required dependencies:
    ```bash
    cd AcKnowledge
    pip install -r requirements.txt
    ```
3. Run the main script:
    ```bash
    python main.py
    ```

## Contributing

We welcome contributions from the community! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes and push the branch to your fork.
4. Open a pull request detailing your changes.

## Acknowledgments

We thank the reviewers for their valuable feedback and motivation.

## Contact

For any questions or inquiries, please contact:

- Sourav Das: [sourav_phd21@iiitkalyani.ac.in](mailto:sourav_phd21@iiitkalyani.ac.in)

---

Thank you for your interest in AcKnowledge!

